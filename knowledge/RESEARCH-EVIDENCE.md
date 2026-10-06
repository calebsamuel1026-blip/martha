# Cold email evidence base

Why this exists: Martha should write cold email the way it has measurably worked for other companies. No guessing. Every rule below is tied to a public source, and every source is graded. Martha is your sales agent across projects; this file is shared by all of them.

Other files cite a rule as `EVIDENCE: R<n>` and a source as `EVIDENCE: S<nn>`. The ids are stable. Do not renumber them.

## How Martha uses this file

1. **Precedence:** your rulings (projects/<project>/CONTEXT.md and the optional COPY-RULES.md) > your own outcomes on a decisive A/B arm (n >= 30 per arm AND Beta-Binomial P(best) >= 0.95) > the rules below by grade > opinion. Until one of your arms is decisive, the research rules stand.
2. **Grades:**
   - **A** = a large platform dataset (1M+ emails) with the sample disclosed, read on the publisher's own page.
   - **B** = a primary dataset that is smaller, older (before 2024), confounded, or about opens only.
   - **C** = a case study with numbers, or a secondhand summary that discloses n.
   - **D** = unsourced, opinion, or numbers that don't add up.
   Every vendor here sells sending tools or agency services. All of the data is observational; none of it is a randomized test unless it says so.
3. **The base rate is the real-world anchor.** Belkins (S05, A, 7.5M emails, 2025) measured a **0.45%** reply rate per email sent, **0.60% for construction**, **0.72% for companies with 0-10 staff**, and **0.57% for owners/founders**. Platform "averages" of 3-4% (Instantly, Hunter, Saleshandy) count replies per sequence and come from self-selected users. Compare your per-email rate to Belkins, not to a per-sequence average.
4. A rule tagged **[S##]** cites the source table in section 3. Confidence is the evidence grade combined with how many independent sources agree.

## 1. Rules

### Subject line
- **R1. Use 2-5 words and stay under 45 characters.** [S08 A: 2-4 words 46% opens vs 10 words 34%; S12 C: 1-4 words best; S13 A: 4-5 words best; S02 A: 5-6 words; S16 B: 3-4 words]. Confidence **high** (5 sources agree). Opens only; no source shows a reply effect from length alone.
- **R2. Personalize the subject with their context (company short name, city, their specific issue), never a bare first name.** [S08 A: personalized subjects 7% vs 3% reply, 46% vs 35% opens; S17 B: +30.5% replies; Lavender (secondhand): first-name subjects cost replies]. Confidence **medium**.
- **R3. Question vs statement is a coin flip, so test it rather than argue it.** [S08: question subjects tied for best opens; Lavender (secondhand): questions lower opens]. Confidence **low**.
- **R4. No salesy subjects: no "!", no ALL CAPS, no emoji, no urgency words, no "quick question".** [S12 C: salesy styling cuts opens up to 17.9%; S02 A: "quick question" 2.5% reply vs 2.9% baseline; S08 A: urgency/jargon under 36% opens]. Confidence **high**.

### Body
- **R5. Aim for 50-100 words, and under 80 when nothing required gets cut.** [S01 A: best under 80; S13 A: under 80 for the first email; S10 B: replies drop sharply past 100 words (executives); S16 B: 50-125 best; S12 C: 13+ sentences nearly halve replies]. **Counter-evidence:** S03 A (Hunter, 34M emails) found length nearly flat, from 4.5% at 20-39 words to 3.7% at 100-119 words, and S27 C (lemlist) puts bookings near 120 words. Confidence **medium**: the effect is real but small, so it never justifies cutting an element your project's copy rules require.
- **R6. Write at a grade 3-5 reading level, in short sentences.** [S16 B: 3rd-grade emails got 36% more replies than college-level, 40M emails, not cold-only, 2016]. Confidence **medium**.
- **R7. Use two or more verified, specific personal attributes, never merge tags alone.** [S02 A: 2 attributes 5.6% vs 0 attributes 3.6% reply (+56%); S11 B (Gong, 30k emails, 2023): individual- or company-based personalization doubles to triples replies; S14 A (Lavender, 231k emails, 2026): personalized emails +50-250% vs templates; S17 B: +32.7% from body personalization]. Confidence **high**.
- **R8. Opener: their situation or loss first, not a compliment and not us.** [S11 B: the problem relevant to the reader drives replies; S24 B (Upworthy, 105k headline tests): each negative word +2.3% clicks, but these were headlines, not email; S16 B: slightly negative sentiment +10-15% vs neutral]. Confidence **low-medium**. A widely repeated "timeline hook beats problem hook 2.3x" figure **has no disclosed source** [S23 D], and pages that repeat it are circular. Don't treat it as evidence.
- **R9. Ask 1-3 questions at most. The CTA question counts as one.** [S16 B: 1-3 questions get 50% more replies; 8+ questions cost 20%]. Confidence **medium**.
- **R10. Plain text: no images, no HTML, no tracking pixel, no links on touch 1.** [S02 A: tracking off 7.4% vs on 4.4% reply; S04 B: HTML emails bounce about 6.7x more than plain text, 2.2M emails, 2025, confounded; S26 C: calendar links on the first touch cut replies; S28 official: Google sender rules]. Confidence **high**.

### Ask
- **R11. Touch-1 CTA = one soft interest or value ask that's answerable in one word. Never a meeting, time slot, or calendar link.** [S09 A (Gong, 304,174 emails): the interest CTA was the best cold CTA, measured as a meeting within 10 days; per secondhand summaries, interest ~30% vs specific time ~15% vs open-ended ~13%; S13 A (Saleshandy, 53.1M, H1 2026): one clear soft CTA gets +78% positive replies; S10 B (Gong 2026): executives answer value offers (benchmarks, insights) more than calendar asks; S21 C: a home-services agency used a "worth a 15-minute look" style ask]. Confidence **high**.
- **R12. Offer-of-value ("want the breakdown? reply yes") vs pure interest ("worth a look?") is unresolved.** Both are soft. Gong supports each one at a different stage. Test it (T3). Confidence **low** on which is better, **high** that both beat a meeting ask.
- **R13. Social proof (results for similar customers) lifts replies in vendor data** [S11 B: industry-specific social proof +88% replies; S22 C: a social-proof P.S. was part of a 9.8% to 18% reply swing in a 206-prospect test with two changes]. Use only real, permissioned results listed in the allowed-proof section of projects/<project>/CONTEXT.md. If the project has none, or the owner bans it, the rule is simple: no social proof. Never invent it.
- **R14. Urgency through deadlines: no cold-email data shows a deadline line changes reply rates.** The only numbers found are open-rate claims from tool blogs without samples. Use a deadline only when it is real; that rule stands on law and honesty, not on data. Confidence: **no evidence either way**.
- **R15. Price in the email: no controlled data exists** (several searches found none). Follow your project's rule. A common, defensible default is no price in the first cold email. Confidence: **no evidence**.

### Sequence
- **R16. Send the first touch plus 3 follow-ups (4 emails), with gaps of about day 3, day 10 and day 17.** [S02 A: 1 email 3.3% vs 3 emails 6.8% reply; S01 A: 58% of replies come from step 1 and 42% from later steps, 4-7 steps best; S06 A (Belkins, 7.5M, 2025): steps 2-6 bring 58.6% of replies, and **step 3 alone books 35.6% of email-sourced meetings**, more than steps 1 and 2 combined; S13 A: 44% of positive replies come from follow-ups, FU1 alone 26.4%, 4-6 follow-ups over 20-21 days; S17 B: one follow-up +65.8%]. Confidence **high**.
- **R17. Send a follow-up as a short reply in the same thread.** [S01 A: a step 2 structured as a reply gets about +30%]. Confidence **medium** (one source, n not split out).
- **R18. Never send a follow-up that only says "just checking in". Each one restates the outcome or adds one new verified fact.** Practitioner consensus only, with no numbers found. Confidence **low**.

### Timing and volume
- **R19. Send on weekdays, 8 AM-12 PM in the recipient's time zone, with Tuesday to Thursday slightly best.** [S07 A (Belkins, 7.5M, Jan-Nov 2025): reply 0.54% in the morning vs 0.47% in the afternoon vs 0.40% at night; **meetings 0.4% in the morning vs 0.1% for every window after noon**; Wed/Thu 0.48% vs Fri 0.44% vs Sat 0.35%; S13 A: Tue 9-10 AM best; S02 A: day of week had no meaningful effect]. Confidence **medium-high** for time of day, **low** for day of week.
- **R20. Send 20-49 emails per inbox per day, to small and tight segments.** [S02 A: 20-49/day 5.7% reply, and peak results stay under 100/day; lists of 21-50 recipients 6.2% vs 500+ 2.4%; S13 A: campaigns under 200 prospects 15-20% vs 500-1,000 8%]. Confidence **medium** (segment size is confounded with personalization).

### Sender (not copy, but the largest measured effect)
- **R21. Send from a custom business domain on a business mail provider, not a free webmail address.** [S02 A: custom domain 5.2% vs freemail 2.5% reply (+108%); Google Workspace 5.9%; S18 A (Snov.io, 10.1M, 2026): free domains bounce 3.87% vs custom 1.15%]. Confidence **high**. This is an account decision for the owner, not a copy decision.

### Spanish-language outreach
- **R22. No public cold-email data compares Spanish vs English to US small businesses.** The closest source is CSA Research "Can't Read, Won't Buy" [S25 B]: 76% of online **consumers** prefer to buy with information in their own language (2020, 8,709 consumers, 29 countries). The B2B edition is paywalled. Spain-market reply rates in search results come from vendor blogs with no sample (D). **Rule:** default to English. Write in Spanish only when the business's own site or listing is Spanish-first (SPANISH-SELLING.md), and treat it as a small directional test, not a rule. Confidence **low**.

## 2. Auditing a project's copy against the rules

Per project, keep a short table like this in your own notes (not in this file):

| Element | Your current copy | Rule | Verdict (agrees / disagrees / test) |
|---|---|---|---|
| Subject length and style | | R1, R4 | |
| Subject personalization | | R2 | |
| Body length | | R5 | |
| Personalization depth | | R7 | |
| Opener | | R8 | |
| Reading level, questions | | R6, R9 | |
| Plain text, no links touch 1 | | R10 | |
| CTA | | R11, R12 | |
| Price, urgency, social proof | | R13-R15 and your rulings | |
| Follow-ups | | R16-R18 | |
| Send time, volume | | R19, R20 | |
| Sender domain | | R21 | |

Where the evidence and your rulings disagree, write the conflict down, name the source and its grade, and let the owner decide. Nothing in this file overrides a ruling.

## 3. Sources

| id | Source | Publisher, date | n | Type | Grade |
|---|---|---|---|---|---|
| S01 | instantly.ai/cold-email-benchmark-report-2026 | Instantly, data Jan 1-Dec 18 2025 | "billions" of interactions | vendor benchmark | A (n vague) |
| S02 | hunter.io/the-state-of-cold-email | Hunter, 2026 report on 2025 data | 31M emails + survey | vendor benchmark | A |
| S03 | hunter.io/blog/cold-email-word-count | Hunter, 2022-2024 data | 34M emails | vendor benchmark | A |
| S04 | hunter.io/blog/is-html-harming-your-cold-email-deliverability/ | Hunter, 2025 | 2.2M emails | vendor, says it is confounded | B |
| S05 | belkins.io/blog/cold-email-response-rates | Belkins, 2025 data | 7,530,489 emails, 34,393 replies | agency benchmark | A |
| S06 | belkins.io/blog/sales-follow-up-statistics | Belkins, 2025 data | 7.53M emails | agency benchmark | A |
| S07 | belkins.io/blog/choosing-the-best-timing-for-your-emails-how-should-you-do | Belkins, Jan-Nov 2025 | 7.5M emails | agency benchmark | A |
| S08 | belkins.io/blog/b2b-cold-email-subject-line-statistics | Belkins + Reply.io, 2024 | 5.5M emails | agency benchmark, mostly opens | A (opens) |
| S09 | gong.io/blog/this-surprising-cold-email-cta-will-help-you-book-a-lot-more-meetings | Gong Labs, 2020, updated 2026 | 304,174 emails | vendor study; cold-stage % only secondhand | A |
| S10 | gong.io/blog/do-execs-really-reply-to-cold-email-here-s-what-the-data-says | Gong, 2026-01-29 | 1M+ exec cycles; n per finding not given | vendor | B |
| S11 | gong.io/blog/4-data-backed-ways-to-increase-your-email-reply-rate-and-book-that-meeting | Gong, 2023-07-07 | 30,000+ emails, 250+ companies | vendor | B |
| S12 | Gong 85M-email guide (gated); via third-party summaries | Gong, undated | 85M (claimed) | third-party summary | C |
| S13 | saleshandy.com/blog/cold-email-statistics/ | Saleshandy, Jan-Jun 2026 | 53.1M emails, 60k sequences | vendor benchmark | A |
| S14 | lavender.ai/blog/the-cold-email-benchmark-report | Lavender, 2026-02-04 | 231,818 emails | vendor | A (few numbers visible) |
| S16 | blog.boomerangapp.com/2016/02/7-tips-for-getting-more-responses-to-your-emails-with-data/ | Boomerang, 2016 | 40M emails, not cold-only | vendor | B (old, mixed) |
| S17 | backlinko.com/email-outreach-study | Backlinko + Pitchbox, 2019 | 12M outreach emails | third-party study | B (old) |
| S18 | snov.io/blog/what-affects-email-deliverability-snovio-report/ | Snov.io, May 2026 | 10,105,581 emails | vendor | A (deliverability) |
| S19 | woodpecker.co/blog/cold-email-statistics/ | Woodpecker, 2026 | mostly cites others; own n not given | vendor roll-up | D |
| S20 | Sales.co study via apollo.io and others | Feb 2026 | 2M emails | secondhand; quoted rates don't multiply out | D |
| S21 | borks.io/blog/agency-30-clients-90-days-cold-email | Borks (cold-email agency) | 81,000 sends to HVAC/plumbing/roofing (1-15 staff) -> 3,320 positive -> 146 meetings -> 30 clients | vendor case study | C |
| S22 | mailshake.com/blog/cold-email-ab-test/ | Mailshake, 2026-02-01 | 206 prospects | vendor case study, 2 changes at once | C |
| S23 | thedigitalbloom.com/learn/cold-outbound-reply-rate-benchmarks/ | The Digital Bloom | not disclosed | roll-up, hook data unsourced | D |
| S24 | Nature Human Behaviour 2023 (Upworthy headlines), via Nieman Lab | Robertson et al., 2023 | 105k headline variants | peer-reviewed, headlines not email | B (transfer) |
| S25 | csa-research.com "Can't Read, Won't Buy" | CSA Research, 2020 | 8,709 consumers (B2B edition gated) | research firm | B (consumer) |
| S26 | community.clay.com calendar-link thread | Clay community | 200k emails (claimed) | practitioner | C |
| S27 | lemlist.com/blog/cold-email-copywriting | lemlist, 2026-08-10 | "millions" | vendor | C |
| S28 | support.google.com/a/answer/81126 | Google | n/a | official sender guidelines | official |
| S29 | thegaryhalbertletter.com: The Boron Letters (1984) and The Gary Halbert Letter issues (1986-2005), digested in HALBERT.md | Halbert estate, free site | none disclosed; his own figures for one famous letter disagree with each other | practitioner craft | D |
| S30 | Copywriter summaries of Halbert's methods (listed in SOURCES.md, Halbert section) | various | none | secondhand | D |

(S15 is intentionally unused.)

Not found despite searching: any controlled test of price vs no price, deadline vs no deadline, or Spanish vs English in B2B cold email; any home-services-specific per-email benchmark with a disclosed n.

## 4. Running A/B tests

Shared stats for any test Martha proposes:
- Each arm gets a Beta(1,1) prior. Bounces and auto-replies are excluded from n.
- **Primary metric = positive reply**: interested, asks for the breakdown, the price or a call.
- Call a winner at P(best) >= 0.95 with n >= 300 delivered per arm.
- Futility: at 1,500 per arm with P(best) < 0.80, call a tie and keep the simpler arm.
- Guardrail: pause an arm if its opt-out or complaint rate reaches 2x control or bounces pass 3%.
- Run tests as factorial cells where your sending setup allows, so volume isn't wasted.
- Statistical reality: at about 0.5% positive replies, a true 2x lift (0.5% to 1.0%) needs about 1,600 delivered emails per arm for an even chance of reaching P(best) >= 0.95, and about 3,700 per arm for an 80% chance. Use the 300-per-arm floor mainly to stop arms that are clearly worse.

Test ideas the evidence supports (proposals; adapt per project):

| # | Change | Arms | Metric to watch | Evidence | Confidence |
|---|---|---|---|---|---|
| T1 | **Personalized subject** | A = generic subject. B = the same subject with their short name or city, at most 45 chars; fall back to A when it won't fit. No first names. | positive reply (secondary: any human reply) | S08 A, S17 B | medium-high |
| T2 | **Shorter first touch** | A = current length. B = 75 words or less: cut optional lines first, keep whatever your copy rules require and the CTA. | positive reply; guard: opt-out rate | S01 A, S13 A, S10 B; counter S03 A (small effect) | medium |
| T3 | **CTA: value offer vs pure interest** | A = "Want the breakdown for {{company}}? Reply 'yes' and I'll send it." B = "Worth a look?" | positive reply; secondary: breakdown-to-call rate | S09 A, S10 B, S13 A | low on the winner, high that both beat a meeting ask |
| T4 | **Send time** | A = weekdays 8:00-11:30 recipient-local. B = 12:00-16:00. | positive reply and **calls booked** (meeting gap is about 4x the reply gap) | S07 A, S13 A | medium-high |
| T5 | **FU1 adds one new verified fact, as a short same-thread reply** | A = a follow-up that restates. B = under 50 words, same thread, opens with a second verified fact about them, same one-word CTA, no "quick". | positive replies to FU1 | S01 A, S13 A, S02 A; the "new fact" part is D | medium on the format, low on the content |

**Outside copy, but often bigger than any test above (the owner's decision):** a business-domain inbox sending 20-49 first touches per day [R20, R21].

## 5. Copy-craft module: Gary Halbert (HALBERT.md)

HALBERT.md is a paraphrased digest of Halbert's public letters (principles, a conflicts register and test hypotheses). This section only grades it and maps it onto the rules above.

- **Grade D means craft and test ideas only:** how to research, write, edit and format, plus hypotheses. Never evidence that something lifts replies, and never above your rulings, your own decisive outcomes or any A to C rule here.
- **Where Halbert agrees with a graded rule, cite the R-id, not S29.** Plain, personal look with no brochure feel = R10, R4, R21. Very simple writing = R6. Specific details about the reader, customized per segment = R7 and R2 (context, not first names). Reader's situation first = R8. One exact, low-friction action = R11. Follow-ups that restate the case = R16, R17, R18. Test small, then roll out, keep the winner = section 4.
- **Where Halbert conflicts, the graded rules win.** His name-in-the-headline idea vs R2: R2 wins. Long copy with the full argument in every piece vs R5 (A): cold email stays short; long copy is only a landing-page test. "Act now" urgency: R14 found no cold-email data either way; only honest deadlines are allowed and pressure-style urgency is banned. Testimonials as standard proof vs R13: only real, permissioned results, and only if your project allows them.
- **Test ideas** in HALBERT.md are proposals. Any that runs uses section 4's stats.
