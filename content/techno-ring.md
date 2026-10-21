<!--
  Techno Ring case study: editable content draft (new style).
  Page: techno-ring.html · Edit freely; the page gets rebuilt from this file.
  Conventions: "## " = section label, "### " = section headline, "#### " = sub-heading,
  "> " = callout / problem statement, [Image: path — caption] = where an image goes,
  [Suggested visual: what — why] = a recommended image to add (not made yet).
-->

Tags: Techno Ring · Concept · Mixed reality · School project

# Designing a mixed-reality therapy companion

A speculative wearable that brings therapy, community and calm into a student’s own room. As the team’s Insights Gatherer, I ran two rounds of testing that took a confusing low-fi concept to a prototype that scored 75 on the System Usability Scale.

[Image: assets/case-studies/techno-ring/01-hero-onboarding.png — Techno Ring onboarding in mixed reality: a green glass panel floating in a living room, offering solo therapy, group sessions and space transformation]

- **75** — SUS score, above the 68 benchmark for “good” usability
- **8** — Moderated sessions across 2 ethics-cleared rounds
- **4/4** — Hi-fi testers called the visual design calming

- **Role:** Insights Gatherer: research planning, user testing, synthesis and design iterations
- **Team:** Saima Desai (Architect, design system), Katrina Lau (Project Navigator), and me
- **Timeline:** Summer 2024, about 5 weeks (low-fi in July, hi-fi by Aug 1)
- **Context:** GBDA 301: Global Digital Project, University of Waterloo
- **Tools:** Figma, FigJam, Figma Slides

## The problem

### Students need support, but getting it feels slow and intimidating

University students, especially international students adjusting to a new country, carry heavy academic and emotional pressure. Many don’t know where to start with mental health support, and booking therapy feels slow and intimidating.

The brief was speculative: design for ten years out, when phones are no longer the most convenient device, wearables are far more advanced, and XR is part of everyday life. So we asked what therapy looks like when the interface lives in your room, not your pocket.

[Suggested visual: A one-line visual of the speculative premise: phone → wearable ring → interface projected into the room. Helps readers who skim past the brief]

> **How might we…**
> - make cognitive behavioural therapy more effective and convenient?
> - extend the reach of support available to university students?

**Constraints.** No real XR hardware, so everything had to be prototyped in Figma. About five weeks. And the interface had to stay legible over *any* real-world background.

## Key findings

### A promising concept, buried under confusion

We built two personas, each with a journey map from first hearing about Techno Ring to recommending it: **Alexis**, a first-year international student facing culture shock and homesickness, and **Rayna**, a domestic student who struggles to keep up her CBT coping strategies.

[Suggested visual: Two small persona cards for Alexis and Rayna (photo-free, just name, situation, need). Easier to scan than the full journey map]

[Image: assets/case-studies/techno-ring/02-journey-map.png — User journey map for Alexis]

Then we put a low-fi prototype in front of four students (think-aloud plus a post-test interview). They wanted three things: therapy that felt personal, booking that fit their schedule, and to feel heard and part of a community. What got in the way:

- *Insight 01* · **Icons said nothing** — People couldn’t describe what the icons did.
- *Insight 02* · **Next steps went missing** — Onboarding never showed where you were or what came next.
- *Insight 03* · **The words kept changing** — Terms shifted between screens, so the copy was hard to scan.
- *Insight 04* · **New features had no on-ramp** — Nothing explained unfamiliar ideas like group therapy.

[Suggested visual: Annotate a low-fi screen with the four insights numbered on it (unclear icon, missing next step, inconsistent term, unexplained group therapy). More convincing than a list]

[Image: assets/case-studies/techno-ring/04-pain-points.png — Four pain points from low-fi testing]

> **Key insight**
> The idea wasn’t the problem. The interface kept asking people to guess, and therapy is the last place anyone should have to.

## Key solutions

### Three calm experiences in one glass-like interface

#### 01 Guided onboarding

*Addresses Insights 02 and 03*

Pick what’s on your mind (anxiety, homesickness, culture shock), a session length and a therapist, then review and edit everything before you book. Every step works with a tap or your voice, and a progress bar shows where you are.

[Suggested visual: The hi-fi onboarding sequence as a short strip: topics → session length → therapist → confirm & edit. This flow has no screen on the page yet]

**Why it works.** The confirm-and-edit step made people feel safe: “People make mistakes, it’s good the product accounts for this.”

#### 02 Solo and group therapy

*Addresses Insights 01 and 04*

Sessions include live captions, a privacy blur so people nearby can’t see your screen, saved notes, one-tap rebooking, and a shared calendar for scheduling groups. Group therapy now opens with a three-step intro: a supportive space, confidentiality, and shared goals.

[Suggested visual: The 3-step group therapy intro screen, and a before/after of the therapist card (new order: name, credentials, sessions, reviews)]

[Image: assets/case-studies/techno-ring/11-solo-session.png — Solo therapy session]
[Image: assets/case-studies/techno-ring/10-session-recap.png — Session recap and notes]
[Image: assets/case-studies/techno-ring/12-group-therapy.png — Group therapy call]

#### 03 Space transformation

Turn your room into somewhere calmer by choosing an ambiance, a location and a soundscape. A short, clearly timed 1–10 check-in closes the loop, so people know what happens after “Continue.”

[Image: assets/case-studies/techno-ring/13-space-transformation.png — Space transformation feedback]

## Research & process

### Designing for glass, not screens

Mixed reality changed the visual rules. We grounded our principles in Apple’s visionOS guidance and XR research, then let testing tell us where they broke.

#### 01 Immersive, or easy to read?

The first prototype wrapped content in a curved, immersive panel. It looked futuristic, but people struggled to scan it.

Options considered:
- **Curved, immersive panel** — + Feels like the future; − Hard to scan and read
- ✅ **Final pick:** **Flatter, scannable layout** — + Faster to read; + Room for a progress bar, voice input and a confirm step

[Image: assets/case-studies/techno-ring/05-lofi-iterations.png — Low-fi first vs. second iteration]

#### 02 What colour is text on glass?

Our starting rule came from visionOS: white text on glass, never light on light. Hi-fi testing broke it. White text was hard to read on light panels, and switching between white and black partway through felt inconsistent.

[Suggested visual: Before/after on glass: white text on a light panel (hard to read) vs dark text on the same panel. The clearest proof of designing for XR]

✅ **Final pick:** Match the text to the panel, with dark text wherever the glass is light, and hold that rule consistently across every flow.

#### 03 Calm you can see

We chose a matcha-green and cream palette to read as calm wellness, and built components for every state, from navigation to captions, translation and privacy blur. It became the clearest win in testing: “Giving wholesome matcha wellness vibes.”

[Image: assets/case-studies/techno-ring/06-style-guide.png — Brand style guide]
[Image: assets/case-studies/techno-ring/07-components.png — Design system components]

#### 04 Second round, four methods

We retested the hi-fi prototype with four students: think-aloud across five tasks, a post-test interview, an A/B preference test, and the System Usability Scale. Every finding mapped to a change:

| Flow | What we heard | What changed |
|---|---|---|
| Onboarding | White text hard to read on light glass | Dark text where the panel is light |
| Solo therapy | The red “session ending” warning felt alarming | Soften its colour and tone *(next iteration)* |
| Group therapy | Unclear what group therapy is | A 3-step intro before joining |
| Group therapy | Therapist cards hard to scan | Name, credentials, sessions, reviews, in that order |
| Space transformation | Unclear what happens after “Continue” | A short, clearly timed feedback form |

[Image: assets/case-studies/techno-ring/09-before-solo-session.png — Before: the old “session ending” warning]

## Impact

### From confusing to calm, with a 75 SUS

[Suggested visual: Simple bar: your 75 SUS against the 68 benchmark. One glance, no reading]

- **75** — Average SUS score across 4 hi-fi testers, above the 68 benchmark
- **8** — Moderated sessions across 2 rounds, cleared by the University of Waterloo Research Ethics Board
- **4/4** — Hi-fi testers described the visual design as calming, clean or visually appealing

Testers also placed Techno Ring squarely with Gen Z to millennial users, the audience our personas described.

## Takeaways

### What I learned as the team’s Insights Gatherer

- **Interviews aren’t the insight** — The useful changes came from coding transcripts, clustering themes, and tracing every design change back to something a person said.
- **Design for a room you don’t control** — In XR, every colour, text and layering choice has to hold up against someone’s real living room.
- **Imagine far, ship near** — We pictured life ten years out and still built something people could click through and critique today.

#### What I’d do differently

- **Lock in the design system first.** Most of our inconsistencies, like text colour and alignment, came from building screens before the rules were settled.
- **Iterate in smaller loops** instead of a few big updates.
- **Test on real hardware,** or at least a headset passthrough mock. Legibility on glass is hard to judge on a laptop.

---

**Read next:** Simplifying client management for fitness trainers — Flento, a CRM redesign that turned a contact form into a guided client setup.

<!--
  TO CONFIRM
  - Teammates are named (Saima Desai, Katrina Lau): OK with them to publish?
  - "Key insight" callout is new wording that sums up the low-fi findings; edit if it doesn't sound like you.
  - Slides are 960px wide; higher-res Figma exports would look sharper.
-->
