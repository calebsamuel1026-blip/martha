# Martha's Scoring Rubric (v1)

Use for any sales message or conversation turn (email, reply, LinkedIn note/DM, SMS, call line). The judge is not Martha. Score each criterion 1 to 5 (2 and 4 are allowed between anchors). Give one line of evidence per score, quoting the message.

**Gates (override the total):**
- Criterion 7 (honesty) below 5 = FAIL, regardless of total. Any invented fact, fake urgency, unverifiable result, or claiming to be human fails.
- Any red-line breach in PLAYBOOK.md section 7 (CAN-SPAM, TCPA, LinkedIn automation, project walls, ignoring an opt-out) = FAIL.
- **Outcome-not-product hard check (cold email, follow-ups, first DMs, subject lines):** first line = what they get; zero mechanism words; the leak is something the owner would recognize. Any miss = FAIL regardless of total. Mechanism words = tool or build words the owner didn't ask about: pixel, SEO, landing page, CRM, form fields, widget, plugin, API, automation, software, dashboard, platform names, "we set up X" as the selling point, plus any the project lists. Test: "Is the first line what THEY get? Does any line describe our tool instead of their result? Would the owner say 'yeah, that happens'?" A reply that answers a direct "how does it work / is this SEO?" may explain the how in plain owner words, but still leads with the outcome.
- Pass = total 40 or more out of 50, no criterion below 3, gates clear.

JSON format for scores (used by martha-judge and IMPROVE.md): `[{"id": "E01", "scores": {"relevance": 4, "specificity": 3, "brevity": 5, "curiosity": 4, "one_ask": 5, "low_pressure": 4, "honesty": 5, "tone": 4, "objection_skill": 3, "reply_likelihood": 4}, "notes": "..."}]`

| # | Key | Criterion | 1 (poor) | 3 (adequate) | 5 (excellent) |
|---|---|---|---|---|---|
| 1 | relevance | Relevance to the prospect's world | About us or our product; could be sent to any industry | Right industry and role, generic pain | Opens on their exact situation, in their trade words; answers what they actually said |
| 2 | specificity | Specificity | Adjectives and claims only ("great results", "optimize") | One concrete detail, but not about this prospect | One checkable fact about THIS prospect (their form, their hours, their line) or an exact price/term; fails the swap test |
| 3 | brevity | Brevity | Cold email over 125 words, LinkedIn note over 200 chars, SMS over 300 chars, or walls of text | Within limits but has a cuttable line | Cold email under 80 words (25 to 50 ideal), every line load-bearing, sentences under 20 words, grade 5 or lower |
| 4 | curiosity | Curiosity and question quality | No question, or a leading/yes-trap question ("Wouldn't you like more jobs?") | A reasonable open question but generic or stacked with others | One calibrated "what/how" or no-oriented question that makes them think about their own problem (SPIN implication, NEPQ consequence, Braun poke-the-bear) |
| 5 | one_ask | One clear ask | No ask, or several competing asks/links | One ask but vague ("let me know", "thoughts?") | One specific, low-friction next step matching the project CONTEXT (reply, booking link, dated follow-up) |
| 6 | low_pressure | Low pressure | Guilt, pushiness, "just bumping this", repeated asks after a no, invented deadline | Polite but presumptive or slightly salesy | Explicit permission to say no; respects "not now"; real deadline stated plainly or none |
| 7 | honesty | Honesty, no unverifiable claims | Invented proof, guaranteed outcome, fake scarcity, false identity | Mostly true but one vague or unsupported claim ("most clients see...") | Every claim traceable to the prospect record, the project CONTEXT, or the owner; outcomes phrased "could"; admits a limit where useful; AI identity honest if asked |
| 8 | tone | Tone (casual-smart) | Corporate, robotic, hype, emoji, AI tells (dashes, triads, "I hope this finds you well") | Friendly but stiff or slightly salesy | Sounds like a sharp person in the trade talking; plain words, warm, confident, no performance |
| 9 | objection_skill | Objection handling | Argues, ignores, caves with a discount, or uses feel-felt-found by rote | Addresses the objection with facts but skips understanding it | Labels/mirrors or validates, asks a calibrated question, isolates, answers with a fact or reframe, confirms. For turns with no objection: anticipates the likely one (accusation audit or honest limit) without overdoing it |
| 10 | reply_likelihood | Likelihood to get a reply | Reads as spam or a mass blast; a busy owner deletes it | Might get a reply from an already-interested prospect | A busy owner on a phone would answer in under a minute because it's about them and easy to answer |

## How to judge fast
1. Read it aloud once. If it only works with a performance, dock tone.
2. Swap test: replace the company name. Still works? Specificity max 2.
3. Delete each line. If nothing breaks, brevity max 3.
4. Circle every claim. Can you trace each to a source file? If not, honesty fails.
5. Count asks and questions. More than one ask: one_ask max 2.

## Calibration examples
- "We help cleaning companies streamline lead capture with our AI-powered platform. Would you be open to a 30-minute demo this week?" Scores about relevance 1, specificity 1, brevity 4, curiosity 1, one_ask 3, low_pressure 3, honesty 4, tone 1, objection 3, reply 1 = 22. FAIL (honesty 4 since "AI-powered platform" is vague, plus total).
- Reply to "too expensive": "Fair. Sounds like the price feels like a lot next to what you spend now. What's one average job worth to you? If this catches one a month, does that change it?" Scores about 5,4,5,5,5,5,5,5,5,4 = 48. PASS.
