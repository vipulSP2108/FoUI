---
title: "IITGN Medical Centre — Field Visit Guide"
subtitle: "FUX Final Project · Group 9 · Topic 10: Medical Waste Management"
author: "Group 9 · Foundations of User Experience · Semester 1, 2026–2027 · IIT Gandhinagar"
date: "November 2026"
geometry: "top=25mm, bottom=25mm, left=22mm, right=22mm"
fontsize: 11pt
linestretch: 1.4
colorlinks: true
linkcolor: "black"
urlcolor: "black"
header-includes:
  - \usepackage{fancyhdr}
  - \usepackage{booktabs}
  - \usepackage{xcolor}
  - \usepackage{mdframed}
  - \usepackage{titlesec}
  - \usepackage{enumitem}
  - \pagestyle{fancy}
  - \fancyhf{}
  - \fancyhead[L]{\small Group 9 · FUX Field Visit Guide}
  - \fancyhead[R]{\small IITGN Medical Centre · Nov 2026}
  - \fancyfoot[C]{\thepage}
  - \renewcommand{\headrulewidth}{0.4pt}
  - \setlength{\parskip}{4pt}
  - \titlespacing*{\section}{0pt}{14pt}{6pt}
  - \titlespacing*{\subsection}{0pt}{10pt}{4pt}
  - \titlespacing*{\subsubsection}{0pt}{8pt}{2pt}
---

\newpage

# Part A — Before You Go: Background Context to Know

This section gives you enough domain knowledge to have intelligent conversations at the facility and ask meaningful follow-up questions.

---

## A1. Why This Visit Matters (The Big Picture)

The IITGN Medical Centre recently completed a major renovation and spatial redesign of its facility. This renovation is academically significant because every facility move causes **spatial disorientation, broken mental models, and new workflow bottlenecks** for staff who had years of muscle memory in the old space.

Your visit has two simultaneous goals:

**Goal 1 — Document the current reality.** Map exactly what exists now: where bins are, what they look like, how staff actually use them (not how they're supposed to).

**Goal 2 — Gather evidence for the AI-AMWS proposal.** Collect pain-point data that justifies the four features of your proposed AI system: peak surge prediction, dynamic bin sizing, visual LED guidance at the bin, and smart custodial routing.

---

## A2. What You Already Know About the Old Facility (Do NOT mention this to staff)

The old facility had the following documented problems — these are your *internal baseline*. As you walk around the new facility, you are silently checking whether these same problems persist, got worse, or were actually solved:

| Old Facility Problem | What to Check in New Facility |
|---|---|
| Yellow & Red bins blended into cream/beige walls — low contrast | Is the wall colour behind bins now better? Do bins stand out? |
| Faded stickers, handwritten polybag labels | Are stickers professionally printed and durable? |
| Treatment Room bins overflowed 15:00–17:00 daily | Is bin sizing appropriate for each room's volume? |
| Staff hesitated 2–4 seconds at bins during rush | Do you observe hesitation in the new layout? |
| Sharps container at awkward height/angle | Is the sharps box easy to reach without bending? |
| Patients/visitors put food waste in medical bins | Does the new layout separate general & medical waste more clearly? |
| Housekeeping had no overflow alerts — rigid schedule | Is the cleaning routine still rigid/scheduled or has anything changed? |
| Bins stuck in corners, away from procedure points | Are bins reachable from where procedures actually happen? |

---

## A3. The Four CPCB Bin Colours — Know These Cold

Under Indian Bio-Medical Waste Management Rules 2016:

| Bin Colour | Accepts | Common Errors to Watch For |
|---|---|---|
| **Yellow** | Anatomical waste, soiled cotton, bandages, expired medicine | Food wrappers, used tissues, general plastics being thrown in |
| **Red** | Contaminated plastics: gloves, IV tubing, syringes (no needle) | Sharps, glass vials, anatomical waste being thrown in |
| **Blue** | Glass vials, ampoules, metallic implants | Plastic items, general rubbish |
| **White (Translucent)** | Sharps: needles, blades, scalpels, broken glass | Anything non-sharp being shoved in |
| **Black/Green** | General non-medical waste only | Medical/infectious items — highest cross-contamination risk |

---

## A4. Key UX Concepts to Keep in Mind During Observation

You are evaluating this facility through the lens of **Don Norman's Action Cycle**:

- **Affordance** — Does the bin's shape/colour make it obvious what goes in?
- **Signifier** — Do the labels/posters communicate the right thing clearly?
- **Mapping** — Is the bin positioned where you naturally walk after a procedure?
- **Feedback** — When you throw something in, does anything confirm you did it correctly?
- **Gulf of Execution** — How much mental effort does a staff member need to identify the correct bin?
- **Gulf of Evaluation** — After disposal, can the user easily tell if they did the right thing?

You are also watching for **Rasmussen's slips and mistakes**:

- **Skill-based slips** — Expert nurses on autopilot throwing things into the wrong bin by habit/proximity, not thinking.
- **Rule-based mistakes** — Staff who know the rules but misapply them (e.g., putting syringes with needles into Red instead of White).
- **Knowledge-based mistakes** — New visitors or students with no training who have no idea what colour code means what.

---

\newpage

# Part B — Observation Protocol (Silent Data Collection)

Do this *before* approaching anyone for interviews. Spend at least 60–90 minutes just watching.

---

## B1. Rooms to Visit and What to Record in Each

For every room, fill out the following data points mentally or in a notebook:

**Bin Inventory per Room:**

```
Room Name: ____________________________
Room Function: ________________________

Bins Present:
  [ ] Yellow   Condition: ___________   Wall colour behind it: ___________
  [ ] Red      Condition: ___________   Wall colour behind it: ___________
  [ ] Blue     Condition: ___________   Wall colour behind it: ___________
  [ ] White    Condition: ___________   Mounted on: [ ] Wall  [ ] Trolley  [ ] Floor
  [ ] Black    Condition: ___________

Lighting type:  [ ] Natural  [ ] LED Ceiling  [ ] Fluorescent  [ ] Mixed
Lighting quality at bin location:  [ ] Bright  [ ] Adequate  [ ] Dim  [ ] Shadowed

Distance from main procedure point to nearest bin: _______ steps / _______ metres
Is the bin visible from the procedure point WITHOUT turning around?  [ ] Yes  [ ] No
Does the bin have a foot pedal?  [ ] Yes  [ ] No   Does it work?  [ ] Yes  [ ] Stiff  [ ] Broken

Signage quality:
  [ ] No signage
  [ ] Handwritten/sticker only
  [ ] Printed poster on wall
  [ ] Bilingual (English + Gujarati/Hindi)
  [ ] Pictogram-based

Mis-segregation observed:  [ ] None  [ ] Occasional  [ ] Frequent
Type of mis-segregation seen: _______________________________
```

---

## B2. Disposal Event Observation Log

For each disposal event you silently observe, note the following (use a tally sheet):

| # | Staff Type | Time | Room | Hesitation? | Head Turn? | Bin Used | Correct? | Notes |
|---|---|---|---|---|---|---|---|---|
| 1 | | | | Y / N | Y / N | | Y / N | |
| 2 | | | | Y / N | Y / N | | Y / N | |
| 3 | | | | Y / N | Y / N | | Y / N | |
| 4 | | | | Y / N | Y / N | | Y / N | |
| 5 | | | | Y / N | Y / N | | Y / N | |
| 6 | | | | Y / N | Y / N | | Y / N | |
| 7 | | | | Y / N | Y / N | | Y / N | |
| 8 | | | | Y / N | Y / N | | Y / N | |
| 9 | | | | Y / N | Y / N | | Y / N | |
| 10 | | | | Y / N | Y / N | | Y / N | |

**Hesitation** = pause of more than 2 seconds before disposal.
**Head Turn** = staff looked at the bin label or polybag before or after disposal.
**Staff Types:** Dr = Doctor, Nu = Nurse, HK = Housekeeping, Pa = Patient, Vi = Visitor

---

## B3. Photos to Take (Capture All of These)

Take these *before* speaking to anyone so the environment is undisturbed:

| Shot | What to Capture | Why It Matters |
|---|---|---|
| **P1** | Wide shot of Triage room showing cot + all surrounding bins together | Shows spatial ergonomics and reach distance |
| **P2** | Close-up of signage poster on wall — full frame including wall colour | For contrast ratio and legibility analysis |
| **P3** | Sharps container — show its height, angle, and what's around it | For ergonomic reach and affordance analysis |
| **P4** | Public corridor bins near reception/waiting area | Visitor mental model and cross-contamination risk |
| **P5** | Inside any bin lid/aperture showing polybag colour and fill level | To check if polybag matches bin colour |
| **P6** | Floor plan sketch or corridor layout (rough hand-drawn is fine) | For spatial mapping in the report |
| **P7** | Any signage that feels unclear, oddly placed, or confusing | Direct UX evidence of affordance failure |
| **P8** (Optional) | Housekeeping trolley/cart showing polybag stock | To see if replacement bags are the correct colour |

> **Safety & Ethics:** No photographs of patients, staff faces, or medical procedures. If a staff member asks you to stop photographing, comply immediately.

---

\newpage

# Part C — Interviews: Staff Nurses & Doctors

---

## C1. How to Approach (Read This First)

**Start with:** *"Hi, I'm a student from IITGN. We're doing a user experience study on how the medical waste management system works in this facility, specifically to understand staff experience and identify ways it could be improved. Would you have 5–10 minutes to share your experience?"*

**Key things to do:**
- Use the word **"experience"** not "problems" — it's less threatening.
- Let them finish answering before probing. Don't interrupt.
- If they say something interesting, ask: **"Can you tell me a bit more about that?"**
- Never argue or correct them even if their answer is technically wrong — you are studying their mental model, not testing their knowledge.
- Thank them specifically at the end: *"This is really helpful — especially what you said about [X]. Thank you for your time."*

---

## C2. Core Interview Questions for Staff Nurses

These are your primary questions. Don't fire all of them — read the conversation and pick the most relevant ones.

**Opening (get them comfortable):**

1. *"How long have you been working at this Medical Centre — including the old facility?"*
   - Follow-up if they mention the old facility: *"How was the experience there compared to here?"*

2. *"What does your usual workflow look like during a procedure — from start to finish, including how you dispose of waste?"*
   - Let them walk you through the whole process. Listen for where bins appear in the story.

**Core Questions — Waste Disposal UX:**

3. *"When you're in the middle of a procedure and need to dispose of something — how do you decide which bin to use?"*
   - **This is the most important question.** Are they reading labels? Going by colour? Going by habit/position?
   - Follow-ups:
     - *"Does it ever take a moment to remember which bin is which?"*
     - *"Has there ever been a time when you weren't 100% sure which bin something should go into?"*

4. *"Which colour bin do you find yourself using most often? And which one do you feel least confident about?"*

5. *"Are there situations where you feel like the bin is not quite in the right place for what you need to do?"*
   - Follow-ups:
     - *"Like, do you ever have to walk more than a few steps to reach it?"*
     - *"Is there any point in a procedure where the nearest bin is the wrong colour?"*

6. *"Have you ever noticed a bin getting full — like almost overflowing — and had to work around it?"*
   - Follow-ups:
     - *"How often does that happen? Daily? Weekly?"*
     - *"What do you do in that situation — wait, tell someone, use a different bin?"*
     - *"Are there specific times of day when it gets worse?"* (expect: afternoon 3–5 PM is a common answer)

7. *"If a bin is too full, do you have a way to let housekeeping know immediately, or do you just hope someone notices?"*

8. *"Can you tell me about a time when you — or someone around you — accidentally put something in the wrong bin?"*
   - If they're hesitant: *"It's completely normal, it happens everywhere. We're not testing anyone — we're trying to understand what causes it so the design can be improved."*
   - Follow-ups:
     - *"What do you think caused that? Was it rushing? The bins looking similar? Unclear labels?"*
     - *"What happened after? Was it fixable, or did it cause a problem?"*

9. *"When you approach a bin to dispose of something, do you feel you get any kind of confirmation that you used the right one? Or do you just trust it?"*
   - If they say "I just trust it": *"Would it help if the bin somehow indicated you got it right?"*

10. *"If you could change one thing about the way waste bins are set up in this room, what would it be?"*
    - This is their design insight — it's gold. Listen carefully.

**On Training & Knowledge:**

11. *"When you first joined this facility, how did you learn which waste goes in which bin? Was there formal training, or did you pick it up from colleagues?"*
    - Follow-ups:
      - *"Do new staff or interns sometimes make mistakes because they're not trained yet?"*
      - *"How often does training happen — was there any refresher after the renovation?"*

---

## C3. Core Interview Questions for Doctors

Doctors are usually busier — keep this to 5 minutes max. Focus on the most critical questions:

1. *"During a consultation or procedure, when and how do you typically dispose of waste — like used gloves, prescription wrappers, sharps?"*

2. *"Is the bin placement in your cabin convenient, or have you wished it was positioned differently?"*

3. *"Have you noticed a situation where a bin was full and you had to improvise?"*

4. *"Do you ever feel uncertain which bin something should go into — particularly for items that feel like they could go in more than one category?"*

5. *"If the bins had some kind of visual indicator — say, a light that told you if you're about to put something in the right one — would that actually be useful, or would it be unnecessary?"*
   - This is a probe for your AI-AMWS LED guidance feature. Watch their reaction.

---

\newpage

# Part D — Interviews: Housekeeping / Custodial Staff

---

## D1. How to Approach

Housekeeping staff are often overlooked in research but carry the most critical safety burden. Show genuine respect.

**Start with:** *"Namaste. Main IITGN ka student hoon. Hum medical waste system ke baare mein study kar rahe hain — aapka kaam bahut important hai is process mein, aur aapka experience samajhna bahut helpful hoga."*  
*(In English: "Hello. I'm an IITGN student. We're studying the medical waste system — your work is very important to this process and understanding your experience would be very helpful.")*

If they're more comfortable in Gujarati or Hindi, use it. The warmth matters more than the language.

---

## D2. Core Questions for Housekeeping Staff

**On Their Daily Routine:**

1. *"Can you walk me through what you do from the moment you arrive until you finish your first round of waste collection?"*
   - Let them describe the entire workflow. Note every room they visit and the sequence.

2. *"How many times a day do you collect waste from the bins? Is it at fixed times, or whenever you notice something?"*
   - Follow-ups:
     - *"Is there ever a situation where you come to a bin and it's already overflowing?"*
     - *"What do you do when a bin is overflowing?"*

3. *"Are there certain rooms or certain bins that fill up much faster than others?"*
   - **This is key data.** Map their answer to rooms.
   - Follow-ups:
     - *"And are there bins that you check and they're barely used?"*
     - *"Does this vary by time of day or day of the week?"*

**On Notifications & Communication:**

4. *"If a bin becomes full between your scheduled rounds, does anyone alert you? Or do you only know when you do your next check?"*
   - Follow-ups:
     - *"Would it be useful if you got a message on your phone when a bin is almost full?"*
     - *"How would that change your work — would it make it easier?"*

5. *"How do you know which rooms to go to first? Is there a fixed order, or do you decide based on what you know?"*

**On Physical Challenges:**

6. *"Which bins are the hardest to handle — physically? Like, is there any bin that's hard to reach, too heavy, or awkward to seal?"*

7. *"When you replace a bag, how do you know which colour bag to put in? Do you always have the right colour in stock, or is there sometimes a mismatch?"*
   - **A mismatch (wrong colour polybag in a bin) is a critical UX failure point.**
   - Follow-ups:
     - *"How often does that happen?"*
     - *"Has a wrong-coloured bag ever been used in a bin by mistake?"*

8. *"Have you ever found items in a bin that clearly don't belong there — like sharps in a general bin or food wrappers in a medical bin?"*
   - Follow-ups:
     - *"Which bins does this happen in most often?"*
     - *"Do you have to do anything special when you find that — like report it, handle it differently?"*

**On Safety:**

9. *"Has there ever been a situation where you felt unsafe while handling the waste — like a sharp poking through a bag, or a heavy overfull bag?"*
   - This is sensitive. If they're hesitant: *"You don't need to give specific details — even just knowing if it has or hasn't happened is helpful."*

10. *"If there were a system that told you exactly which bins need emptying right now and guided you room by room, would that help you? Or would it feel like extra pressure?"*
    - You're testing your AI custodial routing idea. Listen carefully to their reaction — especially any concerns.

---

\newpage

# Part E — Interviews: Administrative / In-Charge Staff

---

## E1. How to Approach

Aim for the facility in-charge, head nurse, or a senior administrative contact. This person has the bird's-eye view.

**Start with:** *"I'm a UX research student from IITGN. We're studying the waste management workflow of this facility for an academic project. Would you be open to sharing some of the operational aspects — like collection schedules, complaint frequency, and compliance processes?"*

---

## E2. Core Questions for the Admin / In-Charge

**On Volumes & Patterns:**

1. *"Roughly how many patients does the facility see on a typical day? And are there specific days or periods that are significantly busier?"*
   - Push gently: *"Like, are Mondays busier? Or before exam season, do more students come in?"*
   - **This directly validates your AI peak-day prediction feature.**

2. *"Does the amount of medical waste generated fluctuate significantly — like certain months or events causing a big spike?"*
   - E.g., vaccination drives, campus sports meets, dengue/flu seasons.

**On Operational Processes:**

3. *"Can you walk me through the full chain — from when waste is generated by a nurse to when it finally leaves the facility?"*
   - Look for: who seals it, where it's stored temporarily, how long it sits before pickup, who the external agency is.

4. *"How often is waste collected from individual rooms? Is there a set schedule or is it need-based?"*

5. *"Is there a process in place for staff to flag when a bin is full — or is it just part of the housekeeping routine?"*

6. *"Has there ever been a compliance issue or audit flag related to waste management — like a bin being found in the wrong area, or waste being stored too long?"*

**On Training & Awareness:**

7. *"Is there a formal training process for new staff on waste segregation? How often is it refreshed?"*

8. *"Are there recurring mistakes that come up during inspections or audits — things staff consistently get wrong?"*

**On the Renovation:**

9. *"Since moving to this new facility — have there been any noticeable changes in how waste is managed, either positive or negative?"*
   - Follow-ups:
     - *"Did any new problems emerge that weren't there in the old facility?"*
     - *"Has staff adapted well to the new layout in terms of knowing where bins are and what they're for?"*

10. *"If you could add one operational improvement to the current waste management system — what would it be?"*

---

\newpage

# Part F — Closing the Visit

---

## F1. After the Interviews

Before leaving each conversation:

- **Thank them specifically.** Reference something concrete they said: *"Thank you especially for the point about polybag colours — that was something we hadn't thought about in detail."*
- **Ask if there's anyone else** you should speak to: *"Is there anyone else on the team — perhaps from housekeeping or the nursing side — who you'd recommend we speak with?"*
- **Ask for consent to follow up:** *"If we have any follow-up questions while writing our report, would it be okay to come back or drop a message?"*

---

## F2. What to Do Immediately After the Visit (Do This the Same Day)

**Within 2 hours of leaving, write up:**

1. **Floor plan sketch** — rough hand-drawn layout of each room with bin positions marked.
2. **Observation summary** — total disposal events seen, hesitation rate, mis-segregation instances.
3. **Top 3 pain points** you observed that weren't expected (surprises are valuable).
4. **Quotes worth capturing verbatim** — anything a staff member said that was particularly insightful. Write it down word-for-word while it's fresh.
5. **Photo labels** — rename each photo immediately with a descriptive name (e.g., `triage_room_yellow_bin_wall_contrast.jpg`).

---

## F3. Follow-Up Questions Based on Common Answers

If you hear these answers, here are your intelligent follow-ups:

| If They Say... | Your Follow-Up |
|---|---|
| *"We just follow the schedule"* | *"Has there ever been a situation where the schedule wasn't enough — a bin was full before the next round?"* |
| *"Staff are well trained"* | *"Can you tell me about a recent instance where even a trained staff member had a moment of uncertainty?"* |
| *"The bins are clearly labelled"* | *"If I didn't know anything about medical waste and walked in here as a patient — would I know which bin to use?"* |
| *"We never really have overflow issues"* | *"What about during vaccination camps, sports events, or flu season — does it ever get stretched then?"* |
| *"The old facility was actually better in some ways"* | *"That's really interesting — can you tell me more about what specifically was better there?"* |
| *"I don't think a smart system would help"* | *"Completely fair. What would your concern be — cost, complexity, something breaking down?"* |
| *"We do get some mis-segregation"* | *"Which bin does it happen in most? And which category of item — like plastics in sharps, or general waste in medical bins?"* |
| *"It's mostly visitors who cause problems"* | *"Are there any bins specifically for visitor areas? And is there anything visible that tells visitors what's acceptable?"* |

---

\newpage

# Part G — Quick Reference Cards (Tear-Out Format)

---

## CARD 1 — Key Numbers to Collect

```
[ ] How many rooms in the facility?               _______
[ ] Total number of bins counted:                 _______
[ ] Yellow bins:  ___  Red: ___  Blue: ___  White: ___  Black: ___
[ ] Average footfall per day (from admin):        _______
[ ] Busiest time of day (from staff):             _______
[ ] How many times/day is waste collected:        _______
[ ] How long before external agency pickup:       _______
[ ] Any rooms with NO medical waste bins:         _______
[ ] Any room with WRONG coloured polybag:         _______
[ ] Disposal events observed:                     _______
[ ] Hesitation events observed:                   _______
[ ] Clear mis-segregation events observed:        _______
```

---

## CARD 2 — Your AI-AMWS Probe Questions (Sprinkle Naturally Into Conversations)

These help you gather evidence for your design proposal without revealing your full plan:

| Feature You're Testing | Question to Ask |
|---|---|
| **Peak surge prediction** | *"Are there days or times when the waste load is significantly heavier than normal? Can you predict when those will happen?"* |
| **Dynamic bin sizing** | *"Are some bins always getting full while others in the same area barely fill up?"* |
| **LED visual guidance at bin** | *"If the bin had a light that guided you to the correct one based on what you're holding — would that feel useful or gimmicky?"* |
| **Custodial mobile alert** | *"If you got a message on your phone the moment a bin hit 75% full — would that change how you plan your rounds?"* |
| **Admin analytics dashboard** | *"Would it help to have a live view of which bins across all rooms are nearing capacity — like a facility-wide map?"* |

---

## CARD 3 — Signs of a Good UX vs. UX Failure (Use While Observing Silently)

| Good UX Signal | UX Failure Signal |
|---|---|
| Staff dispose without looking at label | Staff pause and look at label before disposal |
| Bins visible from across the room | Bins hidden behind doors, curtains, or furniture |
| Bin is within arm's reach of procedure | Staff must walk more than 2–3 steps to reach it |
| Polybag matches bin colour | Wrong-coloured or generic white/clear bags used |
| Sharps box at chest-to-eye height | Sharps box on floor, or at awkward angle |
| Posters are pictogram-based and bilingual | Posters are text-only or English-only |
| No foot-pedal struggling observed | Staff using hands or feet improperly |
| Clean, legible stickers on bin body | Peeling, faded, or handwritten labels |

---

*End of Field Visit Guide — Group 9, FUX Final Project 2026–2027*

*Do not leave this document in the facility or share it with staff.*

---

