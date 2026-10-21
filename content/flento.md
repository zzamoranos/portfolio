<!--
  Flento case study: editable content draft (new style).
  Page: flento.html · Edit freely; the page gets rebuilt from this file.
  Conventions: "## " = section label, "### " = section headline, "#### " = sub-heading,
  "> " = callout / problem statement, [Image: path — caption] = where an image goes,
  [Suggested visual: what — why] = a recommended image to add (not made yet).
-->

Tags: Flento · Internship · Mobile · Unreleased

# Simplifying client management for fitness trainers

Adding a client in Flento took one step, then left trainers with a contact list. I redesigned how trainers add, understand and schedule clients, so every new client starts with a baseline to track and a session on the calendar.

[Image: assets/case-studies/flento/01-schedule.png — Flento schedule showing today’s training sessions in time order]
[Image: assets/case-studies/flento/02-setup-step-3.png — Guided client setup, step 3 of 8: the client’s habits and training experience]
[Image: assets/case-studies/flento/05-client-list.png — My Clients list showing each client with their fitness goal]

[Suggested visual: Hero could become a before/after: the old one-step contact form next to the new guided setup and booked session. Shows the whole story in one frame. Check NDA]

- **8 steps** — Guided client setup, replacing a one-step contact form
- **3 flows** — Redesigned to high fidelity, from setup to first booked session
- **3 competitors** — Benchmarked across 8 capabilities

- **Role:** UX Design Intern, owning client management
- **Team:** Flento’s UX design team
- **Timeline:** Jan to May 2024 (5 months)
- **Skills:** User research, usability testing, information architecture, prototyping
- **Platform:** Mobile (iOS), Figma

> *This project is under NDA, so some research and process details are summarized. Happy to walk through more in conversation.*

## The problem

### Trainers had their clients’ information, but no way to read it

Flento is Voiceflip’s all-in-one platform for gyms, studios and independent trainers. It already handled bookings, messaging, invoicing and payments. But none of it came together around the client, which left trainers asking:

- Who am I training today?
- Is this client actually making progress?
- What should I do after adding someone new?

[Suggested visual: The old “after adding a client” screen: a contact form that drops into a plain list. Lets readers see the dead end trainers hit]

**Why it matters.** Keeping a member costs about a fifth of what it takes to win a new one (IHRSA). A trainer who spots disengagement early can step in. One looking at a contact list finds out when the client cancels.

## Key findings

### Clients stay when they can feel their progress, and Flento gave trainers no way to show it

- *Insight 01* · **Progress goes unseen** — Clients are 35% more likely to cancel within six months when progress isn’t communicated (IHRSA, 2024). Flento captured nothing at setup to measure progress against.
- *Insight 02* · **Setups stop at contact details** — Trainers didn’t know deeper customization existed, so most profiles never got past name, email and phone.
- *Insight 03* · **Client context is scattered** — Messages ran across Instagram, email, WhatsApp and text. Goals and injuries sat on separate screens with no clear way in.

[Suggested visual: A small “scattered context” graphic: messages across Instagram, email, WhatsApp and text, goals and injuries on separate screens, all pointing at one trainer]

> **Design problem I worked with**
> How might we give trainers a clear picture of every client, and a clear next step, so fewer clients slip away?

## Key solutions

### Three flows that connect setup to training

#### 01 See the day at a glance

*Addresses Insight 03*

Today’s sessions, in time order, with each client on their slot and free time marked between. A trainer knows who’s next without opening a profile.

**Why it works.** The day’s commitments show up front, instead of being pieced together across screens.

[Image: assets/case-studies/flento/01-schedule.png — Today’s schedule]

#### 02 Set up clients in guided steps

*Addresses Insights 01 and 02*

Adding a client is now eight short steps, from training habits to body measurements, with a progress indicator and a skip-to-the-end option. Every client starts with a baseline to measure progress against.

[Suggested visual: A strip of all 8 setup steps as small thumbnails, so readers see the full flow and the progress indicator at once]

**Why it works.** Progressive disclosure keeps each step light, and the skip option keeps busy trainers in control.

[Image: assets/case-studies/flento/02-setup-step-3.png — Step 3: habits]
[Image: assets/case-studies/flento/03-setup-step-6.png — Step 6: body measurements]

#### 03 Go straight from setup to a booked session

*Addresses Insights 02 and 03*

Once a client is added, the flow asks the trainer to schedule their next sessions instead of dropping them into a list. The client list then shows each person with their goal, so context stays in view.

**Why it works.** The old flow had no next step after setup. This one ends with a session on the calendar.

[Image: assets/case-studies/flento/04-add-training-dates.png — Add training dates]
[Image: assets/case-studies/flento/05-client-list.png — Client list with goals]

## Research & process

### Trainers weren’t missing features. They couldn’t find them.

#### 01 Benchmark what trainers already compare us to

I mapped Flento against Trainerize, Everfit and Nike Training Club across eight capabilities, from scheduling and payments to messaging and client achievements. Trainerize and Everfit were closest, so they became the benchmark. [Suggested visual: Your competitive analysis table: Flento vs Trainerize, Everfit and Nike Training Club across the 8 capabilities, with checkmarks. It was in your original draft and is a strong research visual]

Two questions guided the rest:

1. Which features do trainers rely on most to keep clients happy and stay ahead of admin?
2. How could client data help trainers make decisions that improve retention?

Why members leave came down to two things: they stop seeing results, or their sessions stop feeling engaging.

#### 02 Audit before adding

Before designing anything, I audited the existing wireframes. Setup ended at a contact form, the new client landed in a general list, and nothing signalled that a detailed client view existed. Trainers found out later that goals, injuries and preferences lived somewhere else.

- **Unclear path.** Trainers didn’t know deeper customization existed, so setups stayed incomplete.
- **No cues.** Nothing prompted them to add more after creating a client.
- **Low discoverability.** Client details sat on separate screens with no logical order.

[Suggested visual: The existing wireframes with the three audit issues annotated on them]

#### 03 Where should richer client data live?

Options considered:
- **A separate analytics area** — + Room for deep data; − One more place to go, far from daily work
- ✅ **Final pick:** **Build on the existing client flow** — + Data sits next to the actions trainers already take; + Nothing new to learn

So I reorganized client management around a trainer’s day instead of around screens:

[Suggested visual: IA before/after diagram: the old structure organized by screen vs the new one organized by a trainer’s day (Plan → Onboard → Follow through)]

| Moment | What the trainer sees | Screen |
|---|---|---|
| Plan | Today’s sessions in time order | Schedule |
| Onboard | Step-by-step setup, from habits to measurements | Guided client setup |
| Follow through | A prompt to book training, then clients with their goals | Add dates, client list |

## Outcome

### Flento wound down before the redesign shipped

The startup stopped operating before this reached production, so there’s no launch data. The work ended as high-fidelity designs in Figma. These are the measures I’d have tracked, one per flow:

| Metric | What it would show | Flow |
|---|---|---|
| Completed client profiles | Whether trainers set clients up past contact details | Guided setup |
| Time to first booked session | How quickly a new client gets on the calendar | Setup to booking |
| Retention past the first months | Whether clients with complete profiles keep training | All three |

## Takeaways

### What I’d carry into the next CRM

- **Audit before adding** — Trainers weren’t missing features. They couldn’t reach the ones that existed, which turned the brief from building into restructuring.
- **Design for the business behind the user** — A trainer’s tools are their livelihood. I judged each screen by whether it saved admin time or helped keep a client.
- **Define success before designing** — Without agreed measures, the project ended with no way to show impact. Next time, I’d set them with the team up front.

---

**Read next:** Making PAT explain itself — Redcan, where one onboarding brief became two product bets.

<!--
  TO CONFIRM
  - NDA: OK to show these app screens publicly?
  - "3 competitors" / "8 capabilities" stats: Nike Training Club was in the comparison; confirm it counts.
  - The "where should client data live" options are framed from your note that the team built on the
    existing client flow rather than adding a separate analytics area. Adjust if the trade-offs were different.
  - Missing visuals from your original draft: competitive analysis table, existing wireframes.
-->
