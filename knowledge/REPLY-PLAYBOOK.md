# Reply playbook: answer every inbound reply within the hour

For replies to cold email (works for any project with that project's facts). Extends PLAYBOOK section 3 "Reply handling by type" with a speed rule, a fixed classification step and ready templates. PLAYBOOK hard overrides and your project's copy rules win over anything here. Sources in SOURCES.md.

## Why within the hour

- A large study of web leads (Oldroyd, McElheran and Elkington, HBR 2011; about 1.25 million leads across 42 companies, as reported in secondary summaries) found firms that tried to reach a lead within an hour were about 7 times as likely to have a real conversation with a decision maker as firms that waited even one more hour, and far more likely than those that waited a day. A cold-email reply isn't a web lead, but it is the same moment: they're thinking about it right now.
- Hot repliers often want a person, fast. Someone who replies "call me" with a phone number has told you the channel; use it instead of resending a booking link.
- If you sell speed or responsiveness, a slow reply is proof against your own pitch.

**The rule.** Between 8am and 9pm prospect time, every human reply gets a drafted answer within 15 minutes and a sent answer (or a call) within 60. Martha drafts. A human or the project's approved tool sends. Outside those hours, it goes out at 8am, first thing.

## Step 1: Hard overrides (before anything else)

From PLAYBOOK section 3, unchanged:
- Any opt-out wording = **unsubscribe**: suppress now, one short confirmation at most.
- Legal or complaint wording = **escalate**: draft nothing, suppress, hand to the owner today.
- Mixed messages take the most restrictive class.

## Step 2: Classify

Pick one. If two fit, use the one higher in this list.

| Class | Signals | Speed |
|---|---|---|
| Interested + phone | "call me", a number in the reply or signature with interest | Call within the hour, then the short email |
| Interested, no phone | "sounds good", "tell me more", "how does it work" plus warmth | Reply within the hour |
| Price question | "how much", "what's it cost", "what's the catch" | Reply within the hour |
| "What is this?" | "who are you", "how'd you get my email", "is this spam" | Reply within the hour |
| Not now | "busy season", "maybe later", "after the holidays" | Same day |
| Referral | "talk to {name}", "my partner handles that", "try {other business}" | Same day |
| Negative | "not interested", "no thanks", "we're good" | Same day, then stop |

Out of office, wrong person, angry, results/proof and "we have someone" stay as in PLAYBOOK section 3.

## Step 3: Check before drafting (2 minutes)

1. Thread card (PLAYBOOK section 2). Never re-ask what they already told us.
2. The project CONTEXT offers section: is a discount live, did this person qualify (e.g. replied inside the window), what's the real end date?
3. Did our cold email claim anything that turned out wrong (a template estimate, a feature they actually have)? Don't repeat it. Correct it if it matters.
4. Their language. If they wrote in Spanish, answer in Spanish (SPANISH-SELLING.md).

## Step 4: Templates

Rules for every template: under 60 words, outcome first (what they get), one ask, no tool or mechanism words, no client stories, "could" for money, no dashes. Price in writing only if your project rules allow it; otherwise quote it on the call and state the terms. Braces must be filled from the record or the project CONTEXT; if a fact isn't on record, cut that phrase. Run the PLAYBOOK section 8 gate on the final text.

**1. Interested, with a phone number.** Call first. Then send this so they know it's real:
> Thanks, {first name}. Let's get those missed customers coming back to you. I'll call you at {their number} today at {time}. If that's a bad time, what time works better?

**2. Interested, no phone number.**
> Thanks, {first name}. Glad you want those jobs back. The fastest way is a 15-minute call where I show you what I found on {short name}. What's the best number to reach you this afternoon?

Variant if they prefer to book themselves (the link belongs in the reply, not the cold email):
> Thanks, {first name}. Glad you want those jobs back. Grab any 15 minutes that suits you here and I'll walk you through what I found on {short name}: {booking link}

**3. Price question (for projects that quote on a call).**
> It depends on what we find and what you need. You'll get a written quote on a 15-minute call before anything starts. {Term and risk reversal from CONTEXT, e.g. "Month to month, nothing billed until it's live."} {Live offer line, only if they qualify.} Want me to call you today?

If the project allows a price in writing, give the number straight, the term, and one question instead.

**4. "What is this?"**
> Fair question. I'm {sender} with {business}. We help {trade} owners keep the jobs that slip away, like a caller who hits voicemail at {verified time} and calls someone else. I wrote because I saw that on {short name}. Worth a 15-minute call this week?

If they ask how we got their email, answer truthfully from the record (for example, "It's listed on your website"). Only if true.

**5. Not now.**
> Totally fair, {first name}. It'll still be here when things calm down. What date should I check back with you?

If they give no date or say no again: "No problem, I'll leave it there. Thanks for the reply." Then stop.

**6. Referral.**
> Thanks, {first name}. Sounds like {their name for the person} is the one who'd want to see this. Is it OK if I reach out to them and mention you pointed me their way?

Never write to the new person claiming a referral they didn't give. If they named another business, thank them and stop: don't cold-mail on their name.

**7. Negative.**
> Understood, {first name}. I won't follow up. Thanks for letting me know.

No ask. Suppress the sequence. A second "no" anywhere ends it for good.

## Spanish versions (usted; see SPANISH-SELLING.md)

**Interesado, con teléfono:**
> Gracias, {nombre}. Vamos a recuperar esos clientes que se le escapan. Lo llamo al {su número} hoy a las {hora}. Si no le queda bien, ¿a qué hora prefiere?

**Precio:**
> Depende de lo que encontremos y de lo que usted necesite. Le damos el precio por escrito en una llamada de 15 minutos, antes de empezar. {Términos del proyecto.} ¿Lo llamo hoy y se lo explico?

**Ahora no:**
> No hay problema, {nombre}. ¿Qué fecha le parece bien para volver a escribirle?

## Step 5: After sending

- Log it (see the output format in the martha agent file) with the thread card and the class.
- Move the prospect's stage in whatever pipeline or CRM you use.
- Set the dated next step. If we said "I'll call at 3", the call happens at 3.
