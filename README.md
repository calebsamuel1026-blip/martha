# Martha

Martha is a sales agent for [Claude Code](https://claude.com/claude-code). She writes cold emails, follow-ups, replies to prospects, LinkedIn connection notes and DMs, call scripts and objection handling. She sounds like a sharp, friendly person who knows the trade: plain words, short sentences, one idea and one ask per message, no hype, and no claim she can't back.

She is made of two parts:

- **Three agent files** (`agents/`):
  - `martha`: the writer. She reads her playbooks, writes the message, runs a mechanical pre-return gate (counted length, sourced numbers, opt-out present, no unfilled placeholders) and scores the draft against a rubric.
  - `martha-judge`: a strict, blind grader for the improvement loop. It scores and never writes copy.
  - `martha-coach`: writes one small, evidence-backed patch to Martha's knowledge per improvement cycle.
- **A knowledge folder** (`knowledge/`): the playbooks Martha reads before every task.

| File | What it covers |
|---|---|
| `PLAYBOOK.md` | Voice, conversation spine, thread card, channel rules, objection library, red lines, pre-return gate |
| `LESSONS.md` | What real results taught her (starts with a few general lessons; you add yours) |
| `SALES-FRAMEWORKS.md` | Gap Selling, Sandler, Voss, Challenger, SPIN, ethical Cialdini: when to use each |
| `COLD-OUTREACH.md`, `SUBJECT-LINES.md`, `FUNNEL-STAGES.md` | Cold email evidence, subject lines, what to reveal at each funnel stage |
| `REPLY-PLAYBOOK.md`, `DISCOVERY-CALL.md` | Answering replies fast, 15-minute call flow |
| `VOICE-OF-CUSTOMER.md`, `SPANISH-SELLING.md` | How buyers talk; selling in Spanish respectfully |
| `HORMOZI.md`, `HALBERT.md`, `BELFORT.md` | Principles summarized in our own words, honesty-filtered. Martha never imitates or claims to be these people. |
| `RESEARCH-EVIDENCE.md`, `SOURCES.md` | Public benchmarks with source ids; the reading list |
| `RUBRIC.md`, `IMPROVE.md` | 10-criterion scoring rubric; the blind holdout improvement loop |
| `projects/` | One folder per business you sell for (template plus a fictional example) |

## Install

**Option A: as a Claude Code plugin.** This repo is its own plugin marketplace. In Claude Code:

```
/plugin marketplace add calebsamuel1026-blip/martha
/plugin install martha@martha
```

The agents `martha`, `martha-judge` and `martha-coach` then appear in `/agents`. Plugin commands change between Claude Code versions; if these don't work, see `/plugin` help or use option B.

**Option B: plain files.**

1. Clone or download the repo anywhere, e.g. `~/martha`.
2. Copy the three files in `agents/` into `~/.claude/agents/` (all projects) or `<your-project>/.claude/agents/` (one project).
3. Leave `knowledge/` where it is.

## Point Martha at her knowledge (MARTHA_HOME)

Every path in the agent files is written as `<MARTHA_HOME>/knowledge/...`. `<MARTHA_HOME>` is the folder where you cloned this repo (the one that contains `knowledge/`).

Martha looks for it in this order:
1. The `MARTHA_HOME` environment variable.
2. A plugin install under `~/.claude/plugins/` (she searches for `knowledge/PLAYBOOK.md`).
3. She asks you.

The easiest setup is to set the variable in your Claude Code settings (`~/.claude/settings.json`):

```json
{
  "env": {
    "MARTHA_HOME": "/home/you/martha"
  }
}
```

On Windows use a path like `"C:/path/to/martha"`. You can also set it in your shell profile. For the improvement loop, tell the main session the folder so it can pass the path to the judge and coach. Those two agents only have read and edit tools, so they can't look up environment variables.

## Add a project

Martha only claims what a project file says. Before using her for a business:

1. Copy `knowledge/projects/_TEMPLATE/` to `knowledge/projects/<your-project>/`.
2. Fill in `CONTEXT.md`: what you sell, the outcome buyers want, the gaps you look for, prices and terms, live offers with real end dates, allowed proof, red lines, voice, CTAs by stage, and your own copy rules (optional, or in a separate `COPY-RULES.md`).
3. See `knowledge/projects/example-window-cleaning/CONTEXT.md` for a fully filled-in, fictional example.
4. Ask for work by project name: "Martha, write a first-touch cold email for <your-project> to this prospect: ...". Give her the facts you verified about the prospect. She won't invent any.

Keep real prospect data, logs and eval answers out of the repo. If you turn on logging, put `log/` and `knowledge/evals/<project>/` in `.gitignore`.

## Improve her over time

`knowledge/IMPROVE.md` describes a blind, holdout-gated loop:
1. Martha answers practice cases.
2. `martha-judge` scores them blind.
3. `martha-coach` writes one patch backed by evidence.
4. The patch stays only if the holdout score rises.

Start from `knowledge/evals/EVALS.example.jsonl`. When you get real results (replies, bookings, opt-outs), add them to `LESSONS.md` in its format. Real outcomes beat practice scores.

## Honest limits

- **She drafts, you send.** Martha doesn't send email, texts or LinkedIn messages. You stay responsible for what goes out and for following CAN-SPAM, TCPA, GDPR or other local law and platform terms. Nothing here is legal advice.
- **Garbage in, garbage out.** Her copy is only as specific as the facts you give her about the prospect and as true as your `CONTEXT.md`.
- **No scripts ship with this repo.** The improvement loop is run by hand or by asking the main Claude Code session to do the bookkeeping. With fewer than about 20 holdout cases, its results are weak evidence.
- **The research ages.** Benchmarks in `RESEARCH-EVIDENCE.md` come from public studies and vendor reports, some of them self-interested. Treat them as starting points and test against your own results.
- **Book summaries are principles, not substitutes.** `HORMOZI.md`, `HALBERT.md` and `BELFORT.md` are short paraphrased notes with attribution. Read the originals (listed in `SOURCES.md`) for the real thing. Martha is not affiliated with, endorsed by, or imitating any of these authors.
- **She is an AI.** If a prospect sincerely asks, she says so. Keep it that way.

## License

MIT. See `LICENSE`. Author: Caleb Cruz.
