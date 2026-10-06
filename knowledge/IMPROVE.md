# Martha improvement cycle (protocol v1)

**Goal:** keep training Martha so her messages get better over time.
**What counts as better:** a higher score from a blind judge on **holdout cases the coach has never seen**. A patch stays only if it raises the holdout score. Train scores, self-scores and judge praise for a change made on the same cases don't count. Real reply outcomes (logged sends vs replies) override everything in this file.

You run this from a normal Claude Code session. Martha, martha-judge and martha-coach are separate subagents (`martha`, `martha-judge`, `martha-coach`). Never let one agent play two roles. No scripts ship with this repo: the steps below are manual, or you can ask the main session to do the bookkeeping (shuffling, averaging, backups) for you. Run one project at a time and never mix projects' cases.

Working folder per cycle: `<MARTHA_HOME>/knowledge/evals/<project>/cycle-NNN/`.

## Set up once

1. **Write eval cases.** Copy `evals/EVALS.example.jsonl` to `evals/<project>/EVALS.jsonl` and write 30 or more realistic scenarios for your project (cold email, follow-up, each reply class, an objection, a call line). Use made-up prospects or anonymized real ones; never paste personal data.
2. **Split.** Mark about 1 in 4 cases `"split": "holdout"` and move them to `evals/<project>/EVALS-HOLDOUT.jsonl`. Pick them at random, not by hand. No holdout id or scenario text may appear in any knowledge file. Never move a holdout case into train.
3. **Protected files.** RUBRIC.md, the eval files and the three agent files are never edited during a cycle. Note their hashes (e.g. `sha256sum`) at the start of each cycle and check them at the end.

## The 10 steps of one cycle

0. **Open.** Create the cycle folder. Copy every knowledge file to `cycle-NNN/backup/`.
1. **Real outcomes first.** If you have logged sends and replies (`log/messages.jsonl` in your own copy), read them first. A clear real result (30+ sends per group) becomes a LESSONS.md entry before any eval work, and real human replies can become new anonymized eval cases.
2. **Martha answers.** Give a fresh `martha` agent a brief of about 20 train cases (a fresh random sample each cycle) and, separately, the full holdout set. Start each brief with "EVAL MODE" so she doesn't log. Save her outputs as `answers-train.json` and `answers-holdout-before.json`. Don't edit her answers.
3. **Blind judge.** Build a judge pack: RUBRIC.md, the auto-fail list (see martha-judge), and every answer as an item with an opaque id (J001...), shuffled, with no hint of which run or version wrote it. Keep the id-to-case key in a separate file the judge never sees. Give only the pack to a fresh `martha-judge` agent. Save its JSON as `judge-1.json`.
4. **Record.** Un-blind the scores with the key. Apply binding machine checks yourself (word count over the cap, missing opt-out). Record per-criterion averages, pass rate and auto-fails for train and holdout separately in `history.jsonl`.
5. **Weakest.** Find the 2 lowest train criteria, the train cases scoring 3 or less on them, and their judge notes. Write `weakest.json`. Holdout notes are never shown to the coach.
6. **Coach patches.** No guessing: every patch must cite its evidence, either a real outcome or a rule id from RESEARCH-EVIDENCE.md, written in the PATCH line as `EVIDENCE: <id>`. Give a fresh `martha-coach` agent `weakest.json`, the train answers and the cycle number. It makes exactly ONE small patch (a rule or an example, 1 to 6 lines, in one knowledge file) and returns `PATCH | ROOT CAUSE | EXPECTED EFFECT | DIFF`. If it proposes "be better", cites nothing, or edits more than one file, reject it and ask again once; if it still can't, skip the patch this cycle.
7. **Martha re-answers the holdout.** Give the same holdout brief to a fresh `martha` agent (it reads the patched files). Save as `answers-holdout-after.json`.
8. **Paired blind judge.** Shuffle the before and after holdout answers into ONE pack, so the judge can't tell which version wrote what and judge drift can't fake a gain. Give it to a fresh `martha-judge`, save as `judge-2.json`, and un-blind.
9. **Gate.** ACCEPT only if all of these hold:
   - the holdout average rose by at least **+0.20**,
   - **no criterion dropped by more than 0.10**,
   - the **auto-fail count did not rise**,
   - no protected file changed.
   Otherwise REVERT: restore the knowledge files from `backup/`. With fewer than 20 holdout cases, treat even an ACCEPT as weak evidence.
10. **Log.** Append one entry to `evals/<project>/IMPROVEMENT-LOG.md` in your own copy: date, weakest criteria, the patch line, files changed, holdout before and after, and the decision.

## Rules that keep it honest

- **No grading her own homework.** The coach never sees holdout cases, holdout answers or holdout notes. Nobody in the loop edits RUBRIC.md, the eval files or the agent files. Changing the rubric is the owner's call, made outside a cycle, followed by a new baseline.
- **One patch per cycle.** If more than one file changed or the patch is large, the cycle doesn't count. Revert and redo step 6.
- **Holdout freshness.** Once a holdout case has been used to decide many patches, it slowly turns into train data. Every 5 accepted cycles, or whenever you make new rulings, add at least 5 fresh holdout cases.
- **Real outcomes win.** A lesson from real sends (30+ per group) overrides any eval-derived rule it conflicts with. The coach must not patch against it.
- **Nothing is sent.** Eval mode never logs real messages and never sends anything.

## Optional: sparring

Every few cycles, have one agent play a skeptical prospect persona (busy owner, price shopper, "we already have someone") and another play Martha, in a short live conversation. Use what you see as ideas for the coach, never as a gate decision. Sparring is practice evidence only.
