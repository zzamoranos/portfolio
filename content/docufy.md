<!--
  Docufy (Karbon Digital) case study: editable content draft (new style).
  Page: karbon.html · Edit freely; the page gets rebuilt from this file.
  Conventions: "## " = section label, "### " = section headline, "#### " = sub-heading,
  "> " = callout / problem statement, [Image: path — caption] = where an image goes,
  [Suggested visual: what — why] = a recommended image to add (not made yet).
-->

Tags: Karbon Digital · Internship · Enterprise · AI

# Designing Docufy from zero

Docufy is Karbon Digital’s AI document assistant. I joined as its first product designer, when the only design file was a page of brand colour notes. In twelve weeks I helped decide what the MVP should be, designed it across web and mobile, and built the design system the company now uses for its other products.

[Suggested visual: Hero: the web home (three-part layout) beside a mobile workspace screen and a peek of the component library, with placeholder text. Shows product + system in one frame. Check NDA]

- **0 to 1** — MVP scoped and designed from a blank Figma file
- **1 system** — Shared across web, mobile and code
- **Company-wide** — Design system adopted for future products

- **Role:** Product Designer (intern), first designer on the product
- **Team:** CXOs, a design advisor, an AI product designer, a PM, engineers and research
- **Timeline:** May to Aug 2025 (12 weeks)
- **Skills:** Product strategy, design systems, product design, visual design

> *Much of this project is under NDA, so some process is summarized and screens use placeholder text. Happy to walk through more in conversation.*

## The problem

### In high-stakes work, a fast summary isn’t worth much if you can’t trust it

Legal, finance and research teams spend their days in long forms, reports and regulatory filings. They want to move faster, but not at the cost of getting something wrong.

AI summaries looked like the answer. In practice, they flattened the details that mattered, so people went back to the original to double-check. The time they saved went straight into verifying.

[Suggested visual: A small “summary vs source” illustration: a generic AI summary on one side, the original document with the lost structure (sections, clauses, figures) on the other. Makes the problem tangible without real client data]

Docufy’s bet was to help teams understand documents, not just shorten them. I joined at the very start, which meant two jobs at once: figure out what the first version should be, and build the foundation everything else would sit on.

> **How might we…**
> help enterprise teams understand and act on complex documents, without losing the structure, context and trust they depend on?

## Key findings

### Speed wasn’t the problem. Trust was.

With no time for a full research round, I pieced together the picture from product discussions with the CXOs, personas and a market gap analysis of existing document tools. The same four problems kept coming up:

[Suggested visual: Your persona cards (or one, simplified) and the market gap analysis as a 2×2 or comparison grid. Shows where Docufy fits against existing tools]

- *Insight 01* · **Context gets lost** — AI tools pull out the data but drop the structure around it, so people rebuild that context before they can act.
- *Insight 02* · **Every field reads differently** — A “summary” means one thing to a lawyer and another to an analyst. Treating all text the same misses what matters in each.
- *Insight 03* · **People check everything twice** — With no sources or reasoning shown, users verify every answer against the original, and the work doubles.
- *Insight 04* · **Too many places to look** — Documents live across formats and tools, so people spend more time managing them than reading them.

> **Key insight**
> People didn’t need AI to think for them. They needed it to show its work, so they could trust it and move on.

## Product strategy

### Deciding what the first version had to prove

With twelve weeks and a small team, we couldn’t build everything. The real design question was what the MVP needed to prove first, and what could wait.

#### 01 Turn insights into product bets

I translated the findings into four bets that every feature had to support. If a feature didn’t serve one of them, it waited for v2.0.

- *Bet 01* · **Keep the source in view** — Answers sit next to the document they came from, so checking is a glance, not a hunt. *(Insights 01, 03)*
- *Bet 02* · **Organize around projects, not files** — Context should build up over time instead of resetting with every upload. *(Insights 01, 04)*
- *Bet 03* · **Connect, don’t export** — Insights should flow into the tools teams already use, instead of becoming one more place to check. *(Insight 04)*
- *Bet 04* · **Earn enterprise trust from day one** — Access is controlled by the company before anyone sees a document.

[Suggested visual: A simple map: the four insights on the left, the four bets in the middle, the MVP features they led to on the right. Shows the reasoning chain at a glance]

#### 02 Scope the MVP

I wrote the MVP scope document and ranked features by user value against effort. It became the team’s shared reference for what was in, what was out, and why. When deadlines got close, I simplified features instead of cutting whole flows. When an idea pushed the product’s direction forward, I made the case to expand it.

[Suggested visual: A slice of the MVP scope doc or a now / next / later board, showing what made the cut and what moved to the v2.0 roadmap]

#### 03 Sequence the build

Options considered:
- **Design web and mobile equally from the start** — + Consistent from day one; − Slows everything down, and engineering waits on both
- **Mobile first** — + Forces simplicity; − Most document work happens at a desk
- ✅ **Final pick:** **Web first, mobile in parallel** — + Engineering starts on the core flows early; + Mobile adapts proven patterns instead of inventing new ones

Once the web flows held up, I refined them for mobile with a clearer hierarchy, fewer taps to get anywhere, and denser but still readable screens.

#### 04 Plan beyond the MVP

At the end of the internship I wrote a product roadmap for v2.0, so the features we’d deliberately held back had a clear place to go and the team could keep building without me.

> **Why it matters**
> Scoping was where the product was really decided. Every “not yet” kept the MVP focused on the one thing it had to get right: trust.

## Process

### Lean, because the MVP couldn’t wait

I loosely followed the double diamond, steered by company goals and what motivates our users. Building from zero meant moving fast, so I kept the early stages short and got ideas in front of the team sooner.

[Image: assets/case-studies/docufy/01-process.png — Process overview: Discovery, Define, Design, Develop, with the activities under each (from the original case study)]

- *01 · Discovery* · **Understand the space** — Product discussions, problem framing, user personas, and a market gap analysis.
- *02 · Define* · **Decide what to build first** — Synthesized findings, journey maps, the MVP scope document, and feature prioritization.
- *03 · Design* · **Explore, then commit** — User flows, then low- to mid-fidelity wireframes, iterated and prototyped with the team every cycle.
- *04 · Develop* · **See it through** — Accessibility checks, documentation, dev handoff, QA testing, and the v2.0 roadmap.

**Testing without a research budget.** There wasn’t time or budget for formal user testing, so I grounded decisions in established usability patterns (clear hierarchy, visible state, feedback on every action), tried flows the way people would actually use them, and ran a round of internal testing, fixes and feedback with every release.

## Design system

### From a page of colour notes to the system the company builds on

There were no design files, just the founders’ notes on brand colours. Since web, mobile and engineering were all moving at once, the system couldn’t be an afterthought. I built it first, so every screen after that came from the same parts.

[Suggested visual: A system overview board: foundations (colour, type, icons) → components (with states) → tokens in code. The single most important visual for this section]

#### 01 Principles

Four rules shaped every decision in the system:

- **Built for reading.** Docufy is a text-heavy product, so legibility comes before decoration.
- **Accessible by default.** Every colour pair passes WCAG contrast, and every component has visible focus and error states.
- **One product, two platforms.** Web and mobile share the same foundations, even when layouts differ.
- **Same language as code.** Names and tokens match what engineers use, so nothing gets lost in handoff.

#### 02 Foundations

- **Colour.** I turned the founders’ hex codes into named colour styles and tuned their saturation and brightness to pass WCAG contrast. Pure black became #121212 (following Material guidance), which is easier on the eyes across long reading sessions.
- **Icons.** I consolidated on Material Icons, which were the easiest to read at small sizes.
- **Type.** I tightened letter-spacing on titles and loosened it on body text, so long passages stay comfortable to read.

[Suggested visual: Colour tokens before/after: the founders’ raw hex codes → named, WCAG-checked colour styles, with #000000 → #121212 called out]

#### 03 One typeface for two platforms

The team had used each platform’s default font, so the app looked different on iOS and Android.

[Suggested visual: Before/after type specimen: the same screen on iOS and Android with mismatched defaults, then with SF Pro / Inter and the adjusted tracking]

Options considered:
- **Keep platform defaults** — + No extra work; − Looks different on every device
- **Bring in a custom typeface** — + Distinctive brand voice; − Slower to load, licensing cost
- ✅ **Final pick:** **SF Pro on iOS, Inter on Android** — + Inter is close to SF Pro, free and fast; + Easy to read in text-heavy screens

#### 04 Components

Buttons, inputs, modals and dropdowns, each built with variants for hover, focus and error states, and Auto Layout so they resize cleanly from desktop to mobile. Designers could build a new screen from parts, instead of starting from scratch.

[Suggested visual: Component sheet: buttons, inputs, modals and dropdowns with hover, focus and error states. Proves the system, not just describes it]

#### 05 Connected to code

I mirrored Figma’s naming in the React component library, and synced colour, spacing and type tokens from Figma Variables to React through Style Dictionary. A change to a colour in Figma could flow straight through to code, so design and engineering never drifted apart. I documented the system so the team could keep using it after I left.

[Suggested visual: Pipeline diagram: Figma variables → Style Dictionary → React tokens. A small, credible “I think about engineering” signal]

> **Outcome**
> The system became the foundation for Karbon Digital’s future products, not just Docufy.

## Key solutions

### Four flows that set up the MVP

Each flow maps back to one of the product bets, and each is built entirely from the design system.

[Suggested visual: One screen per flow (placeholder text): access-code onboarding; home layout with its three zones annotated (navigation / actions / anchored chat + document); mobile workspaces (create, delete, upload); marketplace of connected tools. Your Framer page already has most of these]

#### 01 Onboarding with a company access code

*Bet 04 · Earn enterprise trust from day one*

An admin invites each person, who enters their company’s access code to create an account.

**Why it works.** Enterprise teams worry about where their documents go. Access stays inside the company from the first screen.

#### 02 A home that stays put

*Bet 01 · Keep the source in view*

Navigation on the left, actions along the top, and the chat beside the document in the middle.

**Why it works.** The source is always one glance away, so checking an answer doesn’t mean leaving the page.

#### 03 Workspaces organized by project

*Bet 02 · Organize around projects, not files*

Each workspace keeps its documents, past chats and insights together, so context builds as a project grows. On mobile, people can create workspaces and upload files on the go.

**Why it works.** People think in projects, not files. Grouping by project keeps everything for one piece of work in one place.

#### 04 A marketplace of connected tools

*Bet 03 · Connect, don’t export*

Instead of copying summaries into other apps, teams connect Docufy to the tools they already use.

**Why it works.** It meets people where they already work, instead of adding one more place to check.

## Takeaways

### What designing from zero taught me

- **Strategy is mostly saying “not yet”** — Having a vision meant naming what we didn’t know, convincing stakeholders, and holding back features that didn’t serve the MVP’s one job.
- **Build the system before the screens** — With web, mobile and engineering all moving at once, a shared foundation was what let us move fast without things falling apart.
- **Ownership means making the call** — With no existing design, I had to set direction without all the answers. My mentor pushed me to lead, and I got better at explaining trade-offs and trusting my judgment when priorities shifted.
- **Speak in outcomes** — When timelines got tight, design got pushback. Tying each decision back to users and business goals made the conversations easier, and the decisions better.

---

**Read next:** Designing a mixed-reality therapy companion — Techno Ring, a speculative mental-health experience for university students.

<!--
  TO CONFIRM / ADD
  - Any outcomes: did the MVP ship, who used it, team or user feedback? (strongest addition)
  - "Company-wide" / "adopted for future products": matches your Framer note that the system became the foundation for future initiatives?
  - Typography: is it SF Pro on iOS specifically, or "platform default + Inter"?
  - NEW, please check:
    · The four "product bets" are my framing of how your findings shaped the MVP. Rename or cut any that don't match how the team actually decided.
    · "Ranked features by user value against effort": is that how you prioritized? Swap in the real method if different.
    · "Web first" options: the two alternatives are framed from your note that the MVP centred on desktop; adjust if they weren't really on the table.
    · "Design system principles" are drawn from your decisions (contrast, legibility, Figma ↔ React naming); edit wording to taste.
    · "I documented the system so the team could keep using it": confirm documentation covered the design system.
    · Stat "1 system — shared across web, mobile and code" replaced "12 weeks"; swap back if you prefer the timeline stat.
  - "Key insight" callout and the "Why it works" lines are inferred; adjust if the reasoning was different.
  - Visuals to add (check NDA): onboarding, home layout, workspaces (mobile), marketplace, design system.
-->
