# Cold outreach knowledge base for Martha

Scope: benchmark studies, deliverability rules, public datasets. Paraphrased only. Full source list is in SOURCES.md.
Your project's rules in projects/<project>/CONTEXT.md (and optional COPY-RULES.md) always win. Where the evidence below disagrees with a project rule, flag it as an A/B test; never change the rule silently.

Two lanes are covered:
- [S] Sales: cold email to a business or buyer about an offer. Commercial email, so CAN-SPAM applies.
- [P] Personal outreach: one-to-one personal asks (advice, a short chat, an introduction). Not commercial, but the same deliverability rules apply.
- [B] Both.

## Read this first: how far these numbers travel
- Almost every study below is B2B sales email sent through tools like Instantly, Woodpecker, Mailshake or Belkins. A one-to-one personal ask, or a local service pitched to a small business owner, is a different context. Treat the numbers as direction, not forecast.
- Vendor studies are observational. Senders who write short emails also tend to have cleaner lists and better targeting, so "short wins" may be partly a skill effect. Hunter and BusySeed say this about their own data.
- Headline numbers vary 2x to 4x between studies (average reply rate runs from 1.2% to 8.4%). Differences come from definitions (reply vs positive reply), list quality and which senders each vendor has.
- The only personal outreach source with a real sample (NACE Journal, 541 students, 2020) is about outcomes of personal outreach, not email format. Career-blog reply-rate figures without methodology are NOT used as facts.

## A. Findings by topic

| Topic | Finding (paraphrased) | Source, sample, year | Confidence |
|---|---|---|---|
| Baseline reply rate | Platform average 3.43%, top quartile 5.5%+, top 10% 10.7%+ | Instantly, platform-wide data, 2025 | Medium (platform mix) |
| Baseline reply rate | Average 1.2%; which sending group sent it explained more than which content segment | BusySeed, 287,790 emails, 2026 | Medium |
| Baseline reply rate | 5.8% average in 2024, down from 6.8% in 2023 | Belkins, 16.5M emails, 2024 | Medium |
| Body length | Under 80 words for first touch; strong senders 50 to 90 words, average senders 150+ | Instantly 2025; Mailshake 2026 guide | Medium |
| Body length | Reply rates fall once an email passes about 100 words; best band 50 to 100 | Gong Labs, exec sales study, 2026 | Medium |
| Body length | Best response band 50 to 125 words; under 25 words did about as poorly as very long emails | Boomerang, 40M emails, 2016 | Medium (old, general email) |
| Body length | Emails under 100 words had the lowest bounce rate; 500 to 1,000 words the highest | Snov.io, 10.1M emails, 2026 | Medium (bounce, not reply) |
| Reading level | Third-grade reading level beat college level by 36% and high-school by 17% | Boomerang, 40M emails, 2016 | Medium |
| Questions | 1 to 3 questions: 50% more likely to get a response than zero; 8+ questions did worse | Boomerang, 2016 | Medium |
| CTA type | Asking about interest beat asking for a meeting in cold outreach; once a deal was live, specific times won | Gong Labs, 304,174 emails, 2020 | Medium-high |
| CTA type | A single yes/no question works best; problem-first beats solution-first | Instantly 2025 | Low-medium |
| Pitching | Pitching in cold email cut replies by up to 57% | Gong Labs via secondary summaries | Low (secondary) |
| CTA content | Offering something concrete (a benchmark, an insight) beat a calendar request for executives | Gong Labs exec study, 2026 | Medium |
| Subject line | 1 to 4 words get the best opens; caps, exclamation marks and emoji hurt | Gong Labs, 85M emails (relayed through summaries) | Low-medium |
| Subject line | 3 to 4 words best; an email with no subject did much worse | Boomerang, 2016 | Medium |
| Subject line | 36 to 50 characters did better in link-building outreach | Backlinko and Pitchbox, 12M emails, 2019 | Low-medium (different context) |
| Subject line | Length had no real effect on opens or replies | Yesware, 500,000 emails, older study (secondary) | Low |
| Personalization | Personalized body +32.7% response; personalized subject +30.5% | Backlinko and Pitchbox, 2019 | Medium |
| Personalization | Trigger-based personalization beat name-and-company, which beat none | Secondary roundup | Low |
| Personalization | Emails graded A by Lavender's score lifted reply about 27% | Lavender, 231,818 emails, via secondary summary | Low-medium |
| Proof elements | Emails quoting a percentage statistic had the lowest reply rate (0.8%) vs 1.3% with no proof element and 1.5% with a case-study number | BusySeed, 2026 (observational) | Low-medium. Supports a one-number-per-email rule. |
| Follow-ups | 58% of replies come from email one, 42% from follow-ups; 4 to 7 steps, 3 to 4 days apart | Instantly 2025 | Medium |
| Follow-ups | With at least one follow-up, reply 13% vs 9% without; 2 to 3 follow-ups optimal | Woodpecker, 20M+ emails | Medium |
| Follow-ups | Reply rate highest on email one and falls each step; by step 4, spam complaints and unsubscribes rise sharply | Belkins, 16.5M emails, 2024 | Medium |
| Follow-ups | Steps 2 to 6 produced most replies, but each step's own rate was tiny | Belkins, 7.53M emails, 2025 | Medium |
| Follow-ups | One follow-up raised responses 65.8%; multiple contacts at one organization +93% | Backlinko and Pitchbox, 2019 | Medium |
| Follow-up tone | Follow-ups that read like a reply beat formal reminders by about 30% | Instantly 2025 | Low-medium |
| Send day | Wednesday strongest; weekdays beat weekends | Backlinko 2019; Instantly 2025 | Medium |
| Send day | Weekends and early morning did better | Yesware, older study (secondary) | Low |
| Consistency | Steady sending patterns: +15 to 20% replies | Instantly 2025 | Low-medium |
| Plain text vs HTML | HTML cold emails bounced about 6.5x more than plain text; not a controlled test | Hunter, 2.2M emails, 2025 | Low-medium (confounded) |
| Links and tracking | Tracked-link emails showed lower bounce and higher opens; confounded by sender type | Snov.io, 2026 | Low |
| Attachments | Bounce 2.98% with attachments vs 1.86% without | Snov.io, 2026 | Medium (association) |
| Spam words | Emails with common spam words bounced more (3.43% vs 1.53%) | Snov.io, 2026 | Medium (association) |
| Spam words | Clean copy from a poor-reputation domain still landed badly; reputation and engagement dominate | Single test cited by deliverability blogs | Low |
| Sender type | Free-mail domains bounced 3.87% vs paid 1.68%; custom domains 1.15% | Snov.io, 2026 | Medium |
| Daily volume | Safe cold volume around 30 per day per mailbox | Snov.io, 2026 | Medium |
| Daily volume and warm-up | Free consumer mailbox: published cap 500 recipients a day, practical 20 to 50 cold a day; paid workspace ramp 20 to 30, 40 to 60, 70 to 100 over weeks 1 to 3 | Woodpecker sending-limits guide (practitioner estimate) | Low-medium |
| Warm-up | 5 to 10 emails a day at first, rising over 4 to 6 weeks; keep bounce under 2% | Instantly 2025 | Medium |
| List quality | Bounce above about 2% triggers behavioural blocks before volume limits | Woodpecker; Instantly | Medium |
| Authentication | DMARC-valid senders opened somewhat more often | Snov.io, 2026 | Low-medium |
| Cold personal outreach | People who started contact themselves were about twice as likely to land an internship; informational interviews went with much higher odds of further offers | O'Keefe and Posner, NACE Journal, 541 respondents, 2020 | Medium (self-reported survey) |
| Positive replies | Top reps answer positive replies within about 60 minutes in work hours | Gong, via Mailshake 2026 guide | Low |

### Where studies conflict
1. Follow-ups: Woodpecker and Instantly say follow-ups add 40%+ of replies; Belkins 2024 says more follow-ups lower the average and raise complaints. Likely reconciliation: follow-ups add replies in total, but each step adds fewer and carries rising complaint risk. Two follow-ups sits in the safe middle.
2. Subject length: Gong and Boomerang say 1 to 4 words; Backlinko says 36 to 50 characters; Yesware says no effect. Only Backlinko is outreach-specific, and it is link-building. Default short. See SUBJECT-LINES.md.
3. Send day: Wednesday (Instantly, Backlinko) vs weekend or early morning (Yesware) vs no effect (Woodpecker). No agreement; test.
4. Tracking: common advice says drop tracking pixels; Snov data shows tracked sends with better opens. Confounded both ways. Default: no pixel.
5. Attachments: filters dislike them (Snov, Hunter). If a project wants something attached on email one, see rule 17.
6. CTA: interest-based beats a meeting ask in cold B2B sales (Gong). If a project's whole ask IS a call, frame it as interest, not a calendar slot. See rules 8 and 9.

## B. Deliverability rules

### What the providers require
| Provider | Rule (paraphrased) | Applies to a small one-to-one sender? |
|---|---|---|
| Google (Feb 2024, tightened from Nov 2025) | All senders: SPF or DKIM, valid reverse DNS, TLS, standard message format, spam rate under 0.3% and ideally under 0.1%. Bulk senders (about 5,000+ a day to Google mailboxes): SPF, DKIM and DMARC aligned, plus one-click unsubscribe on marketing mail. | Basics yes. Bulk rules no at 20 to 100 a day. Mail sent from a free Google consumer address is authenticated by Google itself. |
| Yahoo | SPF or DKIM for everyone; bulk senders both plus DMARC; spam rate under 0.3%; unsubscribes honored within 2 days. | Basics only. |
| Microsoft (consumer mailboxes, from May 2025) | Over 5,000 a day needs SPF, DKIM and DMARC, aligned. | Not triggered at small volume. |

### What actually decides inbox vs spam for a small one-to-one sender
1. Spam complaints. At 50 emails a day, a single spam report is 2% of that day, far above the 0.3% line. A tiny sender has no cushion.
2. Bounces. Keep hard bounces under 2%. Guessed addresses are the fastest way to wreck a young sending pattern. Free-mail domains bounce more than twice as often as custom ones (Snov).
3. Sudden volume. Jumping from near zero to 100 a day is the classic trigger for behavioural limits.
4. Near-duplicate content at scale. Spam systems flag groups of messages that look alike even if not byte-identical. Template skeletons with only the name swapped are the risk. Write each email around one real, specific detail, and check drafts for repeated sentences across a batch.
5. Replies. Real replies are the strongest positive signal. Send only to people likely to answer.
6. Format. Plain text, no images, no tracking pixel, no HTML styling.
7. Links and attachments. Each one adds filter risk; for a new sending pattern, minimise.
8. Spam trigger words. Mostly a myth as a standalone cause, but avoid the obvious ones (free, guarantee, act now, $$$) anyway.

### Recommendations for a small sender (new or free mailbox, 20 to 100 one-to-one a day)
1. Ramp: week 1 at 10 to 20 a day, week 2 at 20 to 30, week 3 at 30 to 40, hold at 40 to 50 for the rest of the first month. Test 60 to 100 only if bounces are under 1% and no warning has appeared. 100 a day from a free mailbox is above what these sources call safe. If the ramp is too slow, add a channel (referrals, LinkedIn notes within LinkedIn's terms) instead of raising volume.
2. Spread sends across the working day (for example 8 to 10 an hour) and keep the daily count steady.
3. Warm the account with real conversation before ramping: a few genuine back-and-forth emails a day for a week or two. Replies are the best positive signal (practitioner consensus, not a measured figure).
4. Verify every address before it goes into a batch. Use a firm's email format only when confirmed from a page or a verification tool. One bounce in 20 is already 5%. Stop the day's batch if two bounces appear.
5. Plain text only. No image signature, no pixel, no "view in browser", no URL shorteners. Name, business, phone is enough. At most one link, and none in email one if possible.
6. Attachments are the biggest single risk. Safest to riskiest: (a) no attachment on email one, offer to send it, attach only after a reply; (b) a small text-based PDF under 200 KB with a plain filename; (c) a hosted link.
7. Never send the same body to several people at one organization on the same day, and never CC or BCC. Keep contacts at one organization a few days apart.
8. Watch for throttling: "message blocked" or 4xx/5xx errors, bounces citing reputation or rate, or test emails landing in spam. If any appear, stop 48 hours and halve the daily cap.
9. Seed-test weekly: send a normal email to two accounts you control on different providers and check where it lands. Domain tools like Postmaster Tools need a domain you own, so on a free consumer address seed tests and bounce counts are your only instruments.
10. Honor "stop" requests at once and mark the contact do-not-contact. Spam reports from one person can hurt later mail to their whole domain.
11. Keep the sending identity stable. No rotating display names, no second identity, no "send as" tricks.
12. Log per day: sent, bounced, replied, any block message. Rule of thumb: reply rate under 3% after 60 sends, or any bounce rate over 2%, means stop and fix targeting before sending more.
13. Compliance: CAN-SPAM covers commercial email. One-to-one personal outreach is not commercial; sales outreach is. Sales emails need a real sender identity, a valid physical postal address (a registered mailbox is fine) and an easy opt-out. Keep personal outreach and sales on separate senders. Texts and calls fall under the TCPA; do not cold text or autodial without consent.

## C. Ranked rules for Martha's cold emails

"Conflict" means the evidence disagrees with a project rule in projects/<project>/CONTEXT.md. The project rule wins; Martha proposes a test and records the proposal for the owner.

1. [B] Send only to people you can verify and who plausibly answer. List quality beats copy (bounce above 2% blocks you before any copy matters).
2. [B] One-to-one, human-looking, plain text. No HTML, images, tracking pixels, or more than one link.
3. [B] Keep first touch short: under 100 words, ideally 50 to 90 (Gong, Instantly, Mailshake, Boomerang). If a project allows longer story-shaped emails, test a shorter variant of the same story, at least 30 sends per arm.
4. [S] Sales first touch: 50 to 90 words, one problem, one yes/no question.
5. [B] Simple reading level: short sentences, common words, around grade 3 to 6 (Boomerang). Fix anything above grade 8.
6. [B] Personalize the first line with something real and specific that you read on their own page. Generic AI-style personalization underperforms (secondary sources). Personalized body +32.7% (Backlinko).
7. [B] One hook, one thread, at most one number per email. Percentage statistics had the lowest reply rate in the largest recent sample (BusySeed).
8. [P] The ask: lead with interest and leave timing open ("if you have a few minutes in the coming weeks, I'd be grateful to hear how you did X"). Avoid a fixed "15 minutes on Tuesday" ask on a first touch. Test ending on one question vs a statement; Boomerang suggests the question may win.
9. [S] Sales ask: interest CTA first ("worth a look?", "is this on your radar?"), not a calendar link. Switch to specific times once they reply with interest (Gong). Per project, the exact CTA lives in projects/<project>/CONTEXT.md.
10. [B] Subject: 2 to 5 words, plain, no hype punctuation. See SUBJECT-LINES.md.
11. [B] Follow-ups: two at most for personal outreach (5 to 7 business days apart), up to three for sales (3 to 4 days apart). Each adds exactly one new thing and reads like a reply, not a reminder. Complaints climb by step 4, so stop there.
12. [B] Contact several people at one organization, spaced apart, each in a fresh thread that does not mention the others (Backlinko: +93%).
13. [B] Never follow up in the same hour as a first send, and never follow up with someone who replied or opted out.
14. [B] Timing: weekday mornings in the recipient's time zone, Tuesday to Thursday by default. Evidence is split, so test: half the batch 7:30 to 9:30 am, half late afternoon; compare after 100 sends.
15. [B] Reply fast to anyone who answers: within a few hours, ideally under an hour in work hours.
16. [B] No pitching language or buzzwords ("platform", "AI-powered", "leverage", "passionate", "solution"). Sell the outcome, not the product.
17. [B] Attachments on email one add filter risk (Snov). If a project wants one, test "attached" vs "happy to send it if useful" over 60 sends each. Track inbox placement (seed tests), reply rate and bounce, not only replies. Get the owner's OK before running it.
18. [B] Never "Hope this finds you well", "just checking in", "bumping", or "following up" as the whole message.
19. [B] Never claim shared identity (school, heritage, team, town) unless their own page says it. A wrong assumption costs more than any lift.
20. [B] Log every send: date, recipient role and organization type, hook used, subject, word count, attachment yes/no, send hour, outcome (reply, positive reply, bounce, no reply). Below about 50 sends per variant, treat differences as noise. Change one variable at a time.

## D. Public datasets (none contains real one-to-one cold emails labeled with replies)

The closest by outcome label are XCampaign (opens only) and the cold-email benchmark set (summary rates only). There is no public corpus of cold emails with text and reply outcomes, so Martha's real training signal will be your own logged sends.

| # | Dataset | URL | Rows | License | Labels | Use |
|---|---|---|---|---|---|---|
| 1 | XCampaign (CIKM 2025) | https://huggingface.co/datasets/zidcenek/XCampaignDataset | about 14.9M interactions | CC BY 4.0 | opened, time to open | Timing only; no email text. |
| 2 | Enron-Spam (SetFit) | https://huggingface.co/datasets/SetFit/enron_spam | 33,716 | not stated, research use | spam or ham | Spam-likeness check on drafts. |
| 3 | EnronSpam (AlignmentResearch) | https://huggingface.co/datasets/AlignmentResearch/EnronSpam | 62,284 | not stated | spam or ham | Same source, other splits. |
| 4 | Enron email corpus | https://huggingface.co/datasets/corbt/enron-emails | 517,401 | not stated | none | Tone of normal business email. |
| 5 | Enron original (CMU) | https://www.cs.cmu.edu/~enron/ | about 500,000 | research use (verify) | none | Source of #4. |
| 6 | SpamAssassin public corpus | https://spamassassin.apache.org/old/publiccorpus/ | about 6,000 | Apache-hosted, no formal license | ham and spam, 2002 to 2005 | Classic benchmark; dated. |
| 7 | Spambase (UCI) | https://archive.ics.uci.edu/dataset/94/spambase | 4,601 | CC BY 4.0 | spam or not | Feature reference, no raw text. |
| 8 | SMS Spam Collection (UCI) | https://archive.ics.uci.edu/dataset/228/sms+spam+collection | 5,574 | CC BY 4.0 | spam or ham | SMS; low relevance. |
| 9 | Phishing Email Dataset | https://huggingface.co/datasets/zefang-liu/phishing-email-dataset | 18,650 | LGPL-3.0 | phishing or safe | Safety-filter texture. |
| 10 | Spam, ham and phish 300k | https://huggingface.co/datasets/locuoco/the-biggest-spam-ham-phish-email-dataset-300000 | 365,448 | MIT | spam, ham, phish | Only if training a spam scorer. |
| 11 | B2B Cold Email Benchmark 2026 | https://huggingface.co/datasets/b2bdataindex/cold-email-benchmarks-2026 | market-level rows | CC BY 4.0 | open and reply ranges by market | Summary rates from one vendor; sanity check only. |
| 12 | Cold Email Outreach (weloSai) | https://huggingface.co/datasets/weloSai/ColdEmailOutreach | 2,000 | not stated | none; looks synthetic | Style study only. Low trust. |
| 13 | Email campaign analytics (mindweave) | https://huggingface.co/datasets/mindweave/email-campaigns | 4,025 sample | CC BY-NC 4.0 | simulated events | Dashboards only. |
| 14 | Marketing-Emails (marketeam) | https://huggingface.co/datasets/marketeam/Marketing-Emails | 16,440 | MIT | none | Marketing style study. |
| 15 | Fake email campaign | https://huggingface.co/datasets/MacLeanLuke/fake-email-campaign | 10,000 | OpenRAIL | synthetic | Not evidence. |

## E. Gaps and next steps
- Several primary reports sit behind forms (Gong 85M-email guide, Lavender studies) and were read through secondary summaries. Mark any figure from them "unverified" until the original is read.
- Run the tests above (length, ask as a question, attachment) only after the owner OKs each, and only within the ramp in section B.
- For a stronger signal, the realistic route is your own send log (rule 20) plus a short question to the people who reply.
