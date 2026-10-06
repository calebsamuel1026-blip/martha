# Subject lines (Martha)

Why this exists: a plain, product-named subject sent to strangers can get almost no human clicks or replies. Subjects need to earn the open, and that means training on bolder subjects without crossing into deception.

Scope: every project and every cold or follow-up email. Project rules (projects/<project>/CONTEXT.md, optional COPY-RULES.md) win over this file on facts, capitalization and CTAs. LESSONS.md wins over this file when your own logged results disagree.

**The one rule above all:** bold is allowed, deceptive is banned. A subject can surprise, poke or provoke. It can never promise something the body doesn't deliver, pretend to be a reply, or look like it came from a platform, a bank or a regulator. US law: the FTC's CAN-SPAM guide says the subject must accurately reflect the content of the message, and each violating email can carry a penalty of up to $53,088 (FTC, CAN-SPAM Act compliance guide: https://www.ftc.gov/business-guidance/resources/can-spam-act-compliance-guide-business).

## 1. What the evidence says

Read these as directional. Most are vendor datasets of opens, and opens are inflated by Apple Mail Privacy Protection and bots (GMass; Smartlead). The real metric is **human clicks and replies**. Where studies disagree, that means: test it. Sources are listed in SOURCES.md.

| Topic | Evidence | What Martha does |
|---|---|---|
| Length | Belkins and Reply.io, 5.5M cold emails (2024): 2 to 4 words best, 10 words worst, 1 word also weak. Lavender: 1 to 3 words best; 4 words cut replies. Mobile clients cut off around 33 to 43 characters; Mailchimp advises under 40. | 2 to 7 words, **45 characters hard cap**, the words that matter in the first 30. |
| Questions | Conflict. Belkins: questions tie for best. Lavender: questions lower opens. | Allowed. A question must be one the reader would answer "yes, that's me" to, in their words. Test against a statement. |
| Capitalization | Belkins: small, noisy differences between ALL CAPS, title, lowercase and sentence case. Lavender claims the opposite pattern. | No real case effect, so the **project rule wins** (set it in CONTEXT.md; sentence case is a safe default). Never ALL CAPS words. Merge fields like `{company}` are often ALL CAPS legal names: title-case them or leave them out. |
| Salesy vs internal | Gong (85M cold emails, via a secondary summary): salesy language cut opens about 18%; subjects that look like internal notes ("trial delays", "hiring ops") beat pitches. Lavender: internal emails are short, descriptive and boring; copy that. Classic direct-response advice agrees: unknown sender plus sales subject gets binned unopened. | Default style: looks like a note from a person who knows the reader's world. No offers, prices, "free", "%", "!" in a cold subject. |
| Personalization | Belkins: personalized subjects did better on opens and replies. But lemlist found a first-name token alone made no notable difference, and Lavender saw first names cost replies. Mailchimp (very large sample): localization lifted opens more than names. | Personalize with **context** (their trade, town, size, their pain), not a first-name token. A merge field must render cleanly for every row or fall back. |
| Numbers / specificity | Conflict. Belkins: no effect. Lavender: numbers cut opens. Longer, specific lines can lift replies even when opens fall. | Use a number only when it is THEIR number (their crews, their town) or a real figure in the body. Never a made-up stat. |
| Negative / loss words | Nature Human Behaviour, 2023 (Upworthy headline tests, 105k variants): each negative word raised click rate about 2.3%; each positive word lowered it about 1%. Sad words beat angry or scary ones. | Name the loss or annoyance the reader already feels ("missed", "not your fault", "while you're on a job"). Never invent a loss they haven't had. No fear-mongering. |
| Urgency words | Mailchimp: "urgent"/"important" lifted newsletter opens; "reminder", "last chance" hurt. Belkins: "ASAP"/"now" did poorly in cold email. | Banned in cold email unless literally true. A stranger's "urgent" is false urgency and reads as phishing. |
| Emoji | lemlist: lower opens and fewer replies with emoji (small sample); Reply.io reported a lift. Google bans emoji that mimic verification badges in sender names. | No emoji in B2B or trade cold email. |
| Fake Re:/Fwd: | Google's sender guidelines: don't use "Re:" or "Fwd:" unless the message really is a reply or forward (https://support.google.com/a/answer/81126). | Banned on a first touch. A real follow-up in the same thread may keep "Re:" because it IS a reply. |
| Spam words | Litmus: static spam-word lists are mostly a myth; reputation, authentication, complaints and engagement drive placement. Google: keep user spam reports under 0.1%, never reach 0.3%. | The real risk is a subject that makes people hit "spam" (bait, fake alerts) or looks promotional. Plain text, one link, no images, a subject that matches the body. |
| Copywriters | The daily-email school (Ben Settle, Daniel Throssell): subjects promise a story or a small entertainment, with a curiosity gap the body closes; trust in the sender beats cleverness. Laura Belgray: write like a person; specific and a little odd beats polished business speak. | Curiosity is allowed only when the body pays it off in the first two lines. A story subject must be a true story from the sender's real life. |

**Five takeaways**
1. Short, plain, person-to-person beats clever-salesy. 2 to 7 words, under 45 characters.
2. Personalize with context (their trade, town, size, pain), never a bare name token.
3. Loss and annoyance words pull more clicks than happy words, but only about a loss they have really had.
4. Questions, numbers and case are coin flips across studies. Test them; don't argue them.
5. Deception is both illegal and bad for placement: fake Re:, fake alerts, false urgency, bait-and-switch.

## 2. Templates (fill the slots; every slot must be true for this reader)

`{pain}` = the annoyance in their words. `{outcome}` = what they get. `{trade_object}` = the thing they touch every day (phone, van, estimate, schedule). `{town}`, `{n}` = their real data. Mechanism in brackets. Examples use the fictional Brightpane Window Co. (window cleaning, Maple Falls) pitching local businesses, or a generic trade.

**Safe (plain, internal-looking)**
1. `{trade_object} question` (internal) e.g. "Storefront glass question"
2. `About your {trade_object}` (internal; only if the body is about their specific one)
3. `{town} {trade} question` (local + internal) e.g. "Maple Falls storefront question"
4. `{pain}?` in two to four words (pain question) e.g. "Missed calls after 6?"
5. `{verb}ing the {trade_object} all day?` (their habit, question)
6. `Fixing a {problem}` (descriptive, matches a body that explains how)
7. `{outcome} for {trade}s` (plain outcome)
8. `A {trade} who {did the thing}` (identity; the sender must truly be that)

**Bold (curiosity, loss, story, pattern interrupt)**
9. `Good {things} {happen} while you {sleep/drive}` (loss of what they can't watch)
10. `I got tired of {pain}` (true founder story)
11. `{Pain event} that wasn't your fault?` (sides with them)
12. `Stop {habit}` (command / pattern interrupt)
13. `{n} {units}, one {bottleneck}` (specificity from public data) e.g. "3 crews, one phone line"
14. `What {verb}s while you {absent}` (curiosity gap)
15. `The {thing} nobody {does}` (gap; only if the body names it)
16. `Your {thing} at {time}` (only if you really observed it, e.g. you called at 7:40 pm and got voicemail)
17. `{Thing} is costing you {loss}?` (loss question; never a statement unless measured)
18. `{n} {jobs} a {period} you could keep` (number + "could"; only with a real, sourced number)
19. `Why I {did the thing}` (story; must be true)
20. `{common habit} vs {your way}` (contrast, no competitor names)

**Boldest still honest (contrarian, emotional, odd)**
21. `The {thing} never sleeps. You do.` (contrast)
22. `Your {rating/review} isn't always your fault` (contrarian, takes their side)
23. `Hate the {trade_object}?` (negative emotion word)
24. `Don't {common advice}` (contrarian; the body must defend it)
25. `{Odd specific detail from their world}` alone, e.g. "Streaks at 4 p.m." (odd-specific, in the Settle/Belgray spirit)
26. `Sorry about the {annoyance}` (apology hook; only if the body owns something)
27. `This is not a {thing they expect}` (expectation break; must be true)

## 3. Risk ladder

| Rung | What it looks like | Allowed? |
|---|---|---|
| **Safe** | Plain, internal-looking, descriptive. "Storefront glass question" | Yes. Default control. |
| **Bold** | Curiosity gap the body closes in line 1 or 2; loss or annoyance words; true first-person story; command; public-data specifics; a contrarian take you can defend. | Yes. Most test arms live here. |
| **Boldest-still-honest** | Emotional words (hate, missed), odd specifics, siding with the reader against a platform's rules in general terms. | Yes, with a second read: would they feel tricked after line 2? If maybe, drop it. |
| **Too far (banned)** | Fake "Re:"/"Fwd:" on a first touch. Anything that looks like a platform, marketplace, regulator, bank, bill, payment, security or account alert ("Your account", "Action required", "Order cancelled", "Invoice #"). False urgency or deadlines ("Final notice", "Expires today" when it doesn't). Claims about their account you didn't verify ("Your rating dropped"). Results you can't prove. Brand names that imply a partnership. ALL CAPS, "!!!", emoji. "Urgent"/"important" from a stranger. | Never. CAN-SPAM, Google's sender guidelines, and it trains people to hit spam. |

Gray-zone test: say the subject out loud, then read the first two lines. If the reader would think "oh, that's what it meant", fine. If they'd think "that was a trick", it's too far.

## 4. Checklist (run on every subject before returning it)

1. 45 characters or fewer, counted. Key words in the first 30.
2. Matches the body: the first two lines pay off the subject. Note which email it belongs to.
3. Every claim true for every reader it renders for. No "your X dropped" unless you checked their X.
4. Not a fake reply, forward, alert, invoice, account or platform notice. Doesn't impersonate any brand. Big-platform brand names left out of cold subjects unless tested.
5. Project case rule followed (from CONTEXT.md). No ALL CAPS words, no "!", no emoji.
6. No offer words in a cold subject: free, % off, price, deal, trial, limited, guaranteed.
7. Merge fields render cleanly for every row (ALL CAPS legal names title-cased or dropped; plural/singular handled; blank values fall back to a no-merge subject).
8. Outcome, not product (RUBRIC gate): no tool words (extension, software, AI, automation, plugin, app).
9. In their words (VOICE-OF-CUSTOMER.md), not yours. Swap test: if a rival could send it unchanged, sharpen it.
10. Logged with an id so clicks and replies can be matched later. Judge tests on human clicks and replies, never opens.

## 5. Testing rules

- One variable at a time: same body, same send window, subject only. Split each email's sends evenly between control and challenger.
- If a project sends without a tracking pixel, opens are invisible. Judge winners on human clicks (bot-filtered) plus replies. With a base near zero, run each arm to at least 300 delivered before calling it, and call it only when the gap is several events, not one.
- Watch spam complaints and unsubscribes per arm. A bold arm that raises complaints loses even if it wins clicks.
- Record results in LESSONS.md with counts. The evidence above is vendor data; your own results override it.
