<!--
  Redcan case study: editable content draft.
  Page: redcan.html · Edit freely; the page gets rebuilt from this file.
  Conventions: "## " = section label, "### " = section headline, "#### " = sub-heading,
  "> " = callout / problem statement, [Image: path — caption] = where an image goes,
  [Suggested visual: what — why] = a recommended image to add (not made yet).
-->

Tags: Redcan · Internship · Enterprise · AI

# Redcan: reframing onboarding

As Redcan’s first designer, I was asked to redesign onboarding for PAT, its platform for building government permitting demos. Research showed the real problem wasn’t getting started but understanding the product, so I reframed the brief into two bets: admin tools that explain themselves, and an AI toolkit that teaches developers while they build. Developer onboarding went from weeks to days.

[Suggested visual: Hero: the redesigned workflow editor next to the agent’s terminal running get-started — shows both bets (admin tools + toolkit) at a glance]

- **Weeks → days** — Developer onboarding time
- **1 brief → 2 bets** — Reframed from a first-run flow into a product strategy
- **Expert-validated** — Tested end to end by an outside domain expert

- **Role:** Product Design Intern, first design hire
- **Team:** A PM, an engineering team, and me as the only designer
- **Timeline:** May to Aug 2026 (16 weeks)
- **Skills:** Product strategy, user research, interaction design, AI tooling

## Context

### The first designer on a platform built by engineers

PAT is Redcan’s platform for building permitting and licensing demos for government clients: how a citizen applies for a permit, and how staff review it. Developers configure the forms, workflows and fees for each client. Its whole pitch is speed.

I joined an engineering-led team with one brief: redesign onboarding.

[Suggested visual: A simple diagram of how PAT works: client requirements → developer configures forms, workflows and fees → citizen applies → staff reviews. Gives non-technical readers the mental model in one look]

## The problem

### PAT was built to save time, and learning it ate that time back

New developers needed weeks before their first useful change. Admins couldn’t tell which workflow version was about to go live, built forms they couldn’t see, and kept finding internal IDs on screens that citizens would read.

[Suggested visual: “Before” screenshots, annotated: the old workflow header (status and Publish both green), a form built without a preview, an internal ID on a citizen screen. Proves the problem instead of describing it]

> **Problem statement**
> How might we help people understand PAT well enough to build with it, without someone beside them explaining it?

## Research

### I learned the product the way new hires needed to

I came in without a technical background, so research doubled as my own onboarding. I ran six 1:1 interviews with engineers across experience levels, had them think aloud through real build tasks, and clustered what I heard in FigJam.

[Suggested visual: Your FigJam affinity map, zoomed out or blurred. Shows the volume of research without exposing quotes]

One rule kept me honest: confusion only counted if more than one person hit it. When you’re new, “I don’t get this yet” and “this is badly designed” feel exactly the same.

- *Insight 01* · **Knowing the code isn’t knowing the product** — Senior engineers lowered their own proficiency ratings once the question meant building something end to end. Even the lead architect rated himself near the bottom of the scale.
- *Insight 02* · **It breaks at the seams** — No single feature was hard. People stalled where a task kind had to connect to a workflow and a permission policy.
- *Insight 03* · **The interface kept needing a narrator** — Navigation felt overwhelming, one engineer called the workflow editor “scary,” and a new workspace opened to an empty screen with no next step.
- *Insight 04* · **The docs had depth but no order** — Everyone called them comprehensive. Nobody could say which one to read first.

[Image: assets/case-studies/redcan/journey-map.png — Confidence dipped twice, and both dips came after setup had already worked.]

> **Key insight**
> People could set PAT up. What they couldn’t do was hold its model in their heads. A first-run flow would have polished the one part that already worked.

## Strategy

### The brief said onboarding. The evidence said comprehension.

A new onboarding flow was the obvious answer, and it would have missed. Setup already worked; confidence dropped later, when domain vocabulary arrived and configuration asked for decisions people couldn’t make yet. And it wasn’t one audience: admins struggled with screens that never explained themselves, while developers struggled with a model nobody had laid out in order.

Two failures, two audiences, so I proposed two bets instead of one flow:

[Suggested visual: One brief → two bets diagram: “redesign onboarding” splitting into Admin tools (for admins, staff, citizens) and Agent Skills Toolkit (for developers). The pivot is your strongest strategy moment, so make it visual]

- *Bet 01 · For admins, staff and citizens* · **Make every screen explain itself** — Audit every surface as the person who uses it, and fix the causes of confusion rather than adding help text on top.
- *Bet 02 · For developers* · **Teach PAT inside the agent** — Every engineer already used an AI coding agent daily. Instead of writing another doc, put the guidance where they already work.

**How I sequenced it.** Each bet started with its biggest risk. For the admin tools, that meant the decisions that would shape the system (what goes live, what a case is) before any polish. For the toolkit, it meant testing the hardest skill first, so we’d learn early if the idea held up. I brought the reframe to the PM and engineering with the interview evidence behind it, and we agreed on both bets before I designed anything.

> **My goal**
> PAT should feel finished to everyone who touches it: every page explains itself, advanced options wait until they’re needed, and nothing changes without the user’s say.

## Approach

### How I worked as the only designer

With one designer and a whole platform, I needed a way of working that kept decisions grounded and the team moving with me.

- *01 · Walk it as the user* · **Audit from the outside in** — I walked each surface as the person who uses it: an admin configuring, staff reviewing a case, a citizen applying. I noted every point where someone has to guess, and what they’re guessing about.
- *02 · Severity ≠ priority* · **Separate how bad from when** — Impact and frequency set how serious a problem is. Effort only came in when sequencing the build, so hard problems didn’t quietly drop down the list.
- *03 · Trade-offs, not answers* · **Decide in the open** — For structural decisions I laid out the options with their trade-offs and reviewed them with product and engineering before committing. Open questions went to them first.
- *04 · Throwaway first* · **Prototype fast, ship carefully** — I set up an AI-assisted pipeline the team adopted as its standard: Figma stays the source of truth, explorations start as throwaway prototypes, and Claude in Cursor turns a chosen design into code from existing components. Nothing reaches production without passing a gate, including accessibility (WCAG 2.1 AA) and a config-leakage check.

[Suggested visual: The design-to-code pipeline as a simple diagram: Figma (source of truth) → throwaway prototypes → Claude in Cursor via Figma MCP → gate (WCAG 2.1 AA, config leakage) → production]

## Bet 01 · Admin tools

### Four decisions that shaped the redesign

The audit turned into dozens of prioritized fixes for engineering. These four decisions shaped the rest.

#### 01 What’s about to go live?

Publishing a workflow changes what every applicant sees. But status and actions shared one row, and green meant both “Published” and the Publish button. People couldn’t tell which version was about to go out.

Options considered:
- **Recolor the controls** — + Cheapest fix; − The confusion just moves somewhere else
- **Add a confirmation modal** — + Prevents accidents; − Adds a step to a frequent action to patch a labeling problem
- ✅ **Final pick:** **Separate state from action** — + Fixes the cause; − Bigger header redesign

I split the header into a state zone and an action zone with their own colors, and merged two inconsistent preview controls into one mode with one exit.

[Suggested visual: Before/after of the workflow header, annotated: one row of mixed green status + Publish → separate state zone and action zone, plus the merged preview mode]

#### 02 What does “reopen a case” actually mean?

Staff asked for a way to reopen cases closed by mistake. It sounded like a button. Underneath were four open questions:

- Does a person set case status, or the workflow?
- Is a reopened case the same case, or a new one?
- Does the citizen hear about it?
- Does a manager sign off?

Drawing the screen first would have answered all four by accident. In government, telling a citizen their denied request is back under review is a transparency obligation.

✅ **Final pick:** I settled the model before the screen. I took the four questions to product and engineering, and pulled apart three things the request had bundled together: who can edit, who can see, and who gets notified.

[Suggested visual: Case-status model diagram: who can edit, who can see, who gets notified, with the reopen path. Shows you designed the system before the screen]

#### 03 Fix the form builder, or rebuild it?

Admins built forms field by field in a list and had to imagine the result. Validation meant writing regular expressions. In testing, this was the hardest task of the session by a wide margin.

Options considered:
- **Improve the field-first builder** — + Fast and low risk; − Admins still guess what the form looks like
- **Rebuild it preview-first** — + Matches the workflow editor’s select-and-edit pattern; − Too big for one term
- ✅ **Final pick:** **Both, in sequence** — + Admins get relief now; + The team has a clear target model

Field-editing fixes ship first, preview-first is the target, and regular expressions leave the user’s path entirely. The tester asked for the workflow editor’s pattern by name, which told me the product had already set the expectation.

[Suggested visual: Side-by-side: field-first builder (list of fields, regex validation) vs the preview-first target model (select a field on the live form and edit it)]

#### 04 Dozens of small bugs, or one pattern?

Raw IDs, placeholder text and internal jargon kept reaching real users, including a reference number nobody could read aloud over the phone. Filed one by one, each looked minor, and the ones nobody noticed would stay.

✅ **Final pick:** I named the pattern *config leakage* and made it a check before anything is promoted to production: nothing generated for the system’s convenience reaches a person. A named rule also catches the cases nobody has reported yet.

[Suggested visual: A “config leakage” example: a citizen-facing screen with a raw ID / placeholder circled, next to the pre-production checklist rule]

## Bet 02 · Agent Skills Toolkit

### Teaching PAT where developers already work

Every engineer I interviewed used an AI coding agent daily, and some had already suggested packaging repeated setup work as agent instructions. One more doc wouldn’t fix docs that had no order. A guided path inside the agent could.

I designed a set of skills named for what a developer is trying to do: `get-started`, `create-task-kind`, `build-mvp`, `rebrand`, `check-work` and `starter-template`. Each one handles the mechanics and explains the PAT concept behind it at the moment it matters.

[Suggested visual: Agent chat/terminal mockup of a developer running create-task-kind: the agent drafts the task kind, explains what a task kind is, and waits for an explicit “apply”. Shows all three principles in one frame]

- *Principle 01* · **Teach while carrying** — Understanding builds through real work, one concept at a time, right when it’s needed.
- *Principle 02* · **Draft first, apply on purpose** — Every skill works as a draft. Live configuration only changes after an explicit apply.
- *Principle 03* · **Nothing is optional** — In testing, the agent quietly skipped any step framed as optional. So planning and branding became decisions it has to record.

#### Designing for an AI user, too

I tested the riskiest skill first. The workflow skill loaded on fewer than half of our test prompts, and when it did, the agent usually avoided PAT’s workflow engine altogether. It was hitting the same friction the engineers had described. Rather than write it off as a failed test, the team carried the agent’s reasoning into the next phase as input for improving the engine.

## Validation

### An outside expert found the thing I wasn’t looking for

I ran a moderated session with a records-management professional from outside the team. He played citizen, staff, admin and finance through a municipal records request, then built a new application type from scratch. The hardest part was staying quiet.

He called the redesign a major step up from the earlier version. Binding a workflow to an application was the standout, done in seconds, and he rated the workflow builder competitive with tools he already uses. The form builder was the weak spot, which confirmed the move to preview-first.

[Suggested visual: A simple scorecard: what held (workflow binding, workflow builder, overall experience) vs what needs work (form builder → preview-first), shown as strong / mixed / weak rather than exact scores]

Two moments changed the plan:

- **He made a decision on a case by accident.** No confirmation, no undo, and he said he thought he’d broken something. I’d been hunting for places the interface hid state, and missed where it hid consequences. Decision safety jumped ahead of most of the backlog.
- **He wanted AI to do the building.** He guessed that a long form build would take moments if an agent could read the requirements doc directly, which backed the toolkit’s bet from the client side.

## Reflection

### Learning a technical product from the outside in

- **Reframe before you redesign** — The most valuable thing I did was question the brief. A polished onboarding flow would have shipped on time and fixed the part that already worked.
- **Being new is a research tool** — My own confusion was a signal, as long as I checked it against other people’s. That rule gave me the evidence to push back.
- **Name the pattern, not the bug** — Many issues were the same defect in different places. A named rule can be enforced; a pile of screen-level opinions can’t.

**Next up:** a usability session with non-technical users, confirmation and undo for staff decisions, and the next phase of the toolkit.

---

**Read next:** Designing an AI document assistant from zero — Docufy at Karbon Digital, from brand colour notes to an MVP and a company-wide design system.

<!--
  TO CONFIRM
  - Title: "Redcan: reframing onboarding". Other options in the same shape:
    "Redcan: onboarding, reframed" · "Redcan: from onboarding brief to product strategy" · "Redcan: making PAT explain itself".
    The Home card currently reads "Making an enterprise platform explain itself"; update it to match when the page is rebuilt?
  - "How I sequenced it" and "we agreed on both bets before I designed anything": does that match how buy-in actually happened?
  - Approach step 04 comes from your Process tab: confirm the tools (Figma Make, Claude Design, Claude in Cursor, Figma MCP, Mantine) and the gate checks, and that the team adopted it as standard.
  - Term dates: research plan says May 2025, session files are dated 2026.
  - How the "weeks to days" onboarding figure was measured.
  - Purpose of each skill, especially build-mvp and starter-template.
  - What Redcan is OK making public: quotes, internal details, the name PAT.
-->
