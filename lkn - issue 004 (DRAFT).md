**How Rules Actually Change: The Rule Lifecycle Behind AI Governance**  

> *Most AI governance fails between “we should change this rule” and anything actually changing. A simple, domain-agnostic rule lifecycle makes that gap visible – and fixable.*

---

We’ve already got too many AI principles, policies, and “responsible AI” frameworks.

We don’t have a good answer to a more basic question:

> When reality changes, **how** do our rules change – and why do they so often fail to?

In an earlier piece I called this the **metabolism of rules** – how quickly and clearly a rule system notices the world has changed, updates its assumptions, and gets new rules all the way to the people and systems that use them.

This article goes one level deeper.

It focuses on the **rule lifecycle**: the small set of stages every rule must pass through if you want governance to keep up with AI, automation, and a fast environment. In a later piece I’ll map the full rule ecosystem around those rules — the users, systems, makers and decision authorities they sit inside — but you don’t need that detail to use the lifecycle lens.

You don’t need to believe in any one framework to see the pattern. If you’ve ever thought:

- “We talked about changing this ages ago; nothing happened.”  
- “We updated the policy and behaviour didn’t move.”  
- “When this went wrong, we couldn’t show who knew what, when.”

…you’ve lived a broken rule lifecycle.

---

## 1. The quiet failure between “we should change this” and anything changing

Most organisations don’t fail at seeing problems.

People on the ground notice:

- new AI tools creeping into workflows  
- models drifting  
- rules clashing  
- external regulations shifting  
- incidents that show “the current rules are wrong for this situation”

Some of those signals even get written down:

- risk logs  
- audit findings  
- working group notes  
- ethics board recommendations  
- model review reports

The quiet failure happens in the gap between:

> **“We should change this rule”**  
> and  
> **“this rule has actually changed how people and systems behave.”**

In that gap, three things go wrong:

1. **Signals don’t turn into structured proposals.**  
   They stay as emails, comments, “for noting” items.

2. **Proposals don’t reach real decisions.**  
   They get stuck in committees, roadmaps, or “next quarter” piles.

3. **Decisions don’t turn into clear, enforced expectations.**  
   Policies are updated on paper, but rule users and systems don’t change.

I call the result **governance debt**: rules accrete and drift faster than they can be updated or retired. AI just makes this impossible to hide, because AI-enabled systems can move faster and fail at scale.

To fix that, we need to stop thinking of “governance” as a bookshelf of PDFs and start treating it as a **lifecycle** that either exists – or it doesn’t.

---

## 2. The rule lifecycle: two coupled cycles, minimal skeleton

Under the Open Meta-Governance Standard (OMGS) – a draft open specification I’ve been developing – governance is described in terms of a simple **rule ecosystem**:

- **rule users** and **rule resources** inside a rule environment,  
- surrounded by **rule makers** and **decision makers**,  
- all influenced by external factors (markets, laws, technologies, shocks).

Inside that ecosystem, governing rules comes down to two coupled cycles:

1. **Proposing changes to rules** – how reality turns into proposals  
2. **Implementing changes to rules** – how proposals turn into binding, lived rules

I’ll unpack that rule ecosystem model — the actors, resources and flows between them, with example diagrams — in a separate piece. In this article we just need the lifecycle skeleton that runs inside it.

These cycles are not optional “nice to haves”. They’re the **minimal skeleton** you need if you want rules to respond to reality.

### 2.1 The proposing cycle (from reality to rule submission)

On the proposing side, four things must exist:

1. **Environment change**  
   The world moves, whether you watch it or not:
   - rule users behave differently  
   - rule resources (systems, models, assets) are used in new ways  
   - external factors (markets, laws, technologies) shift  
   This is the raw material. If nothing changed, you wouldn’t need rule change.

2. **Monitoring**  
   Rule makers systematically observe environment and external activities and compare them with rule content:
   - “What’s actually happening vs what our rules assume?”  
   No monitoring → **rules go blind**. You rely on luck and whistleblowers.

3. **Analysis**  
   Rule makers interpret those signals:
   - what has changed?  
   - which rules or assumptions are now wrong, incomplete, or mis-scoped?  
   No analysis → you get **random, reactive changes** or endless “noted” items.

4. **Reporting → Rule submission**  
   Analysis is converted into a **rule submission**: a structured proposal a decision maker can legitimately act on:
   - “Here’s what changed.”  
   - “Here’s how it affects current rules.”  
   - “Here’s the change we propose and why.”  
   No reporting/submission → issues never enter the formal rule pipeline.

You can compress these steps in practice, but you can’t remove any of them without breaking something.

---

### 2.2 The implementation cycle (from decision to lived behaviour)

On the implementation side, four more stages are essential:

5. **Decision**  
   A decision maker with formal authority approves, modifies, rejects, or defers a rule submission.  
   No decision → nothing is actually binding; everything is “in discussion”.

6. **Announcement**  
   The rule system formally declares:
   - what has been adopted  
   - when it takes effect  
   - what it replaces or retires  
   - who and what it applies to  
   This is how the rule ecosystem learns “this is now a rule”.  
   No announcement → **nobody knows the rule has changed**, even if a decision was made.

7. **Communication**  
   Communication makes rules findable, understandable, and usable for **rule users**:
   - not just “we published this update”  
   - but “in your role / system / context, here’s what this means and what you do differently”  
   You can have rules properly announced but completely incomprehensible.  
   No real communication → rule users are left guessing or stuck in meetings.

8. **Enforcement**  
   Enforcement is the subset of administrative activities that act on rule users to **reduce misalignment** between:
   - **rule activities** (what people and systems actually do), and  
   - **rule content** (what the rule says should happen)  
   Done well, enforcement is about alignment and outcomes, not punishment.  
   No enforcement → rules stay performative; compliance is optional.

You can change how these stages are implemented. You can’t skip them.

---

## 3. The proposing cycle: when reality moves faster than your rules

Let’s make this concrete.

### 3.1 Environment change – the world moves, with or without you

Examples:

- An AI model trained on old data starts behaving oddly as behaviour patterns change.  
- A new class of AI assistants shows up in the organisation; people quietly use them in workflows never designed for automated reasoning.  
- A housing, welfare, or lending rule interacts with rising cost-of-living in a way that consistently harms people it was meant to help.

Exec questions:

- What are the **environment activities** we care about (behaviour, decisions, model uses, transactions)?  
- What **external factors** (laws, standards, tech, markets) impact them most?

You don’t control environment change. You control whether you **notice** it.

---

### 3.2 Monitoring – who actually watches reality against your rules?

Monitoring is not “we have dashboards”; it is:

- ongoing observation of environment and external activities,  
- compared against rule content and its assumptions.

Examples:

- Monitoring AI outputs and usage patterns against documented guardrails.  
- Tracking complaints, incident reports, and edge cases where rules produce unfair or absurd outcomes.  
- Watching external regulatory updates that invalidate internal rules.

Exec questions:

- Who, by role, is tasked with **Monitoring** for this rule set?  
- What do they look at, and how often?  
- Where do monitoring outputs actually go?

No monitoring → your rules are flying instrument-blind.

---

### 3.3 Analysis – turning signals into understanding

Analysis is where rule makers interpret what Monitoring sees:

- “Is this drift or noise?”  
- “Does this external change contradict our current rules?”  
- “What failure patterns are emerging?”

Examples:

- Analysing a cluster of AI incidents to see if an entire class of uses is mis-governed.  
- Assessing whether a welfare eligibility rule now excludes the people it was meant to protect.  
- Reviewing how a new AI regulation interacts with existing corporate policies.

Exec questions:

- Who does **Analysis** on monitored signals – which team, with which disciplines?  
- Do they have enough context to understand both the domain and the rules?  
- Are their outputs treated as advice, or as inputs to a change process?

No analysis → you get random reactions and “fire drill” changes.

---

### 3.4 Reporting → Rule submissions – getting into the decision queue

Reporting is where Analysis becomes a **rule submission**:

- a structured proposal that sets out:
  - what changed in the environment/external factors  
  - how current rules are misaligned  
  - what change is proposed and why

Examples:

- A submission to restrict certain AI uses to specific contexts unless new safeguards are in place.  
- A submission to retire overlapping policies and consolidate them into a simpler, clearer rule.  
- A submission to add explicit triggers and review criteria to a critical rule.

Exec questions:

- In our org, what *counts* as a **rule submission**?  
- How many “we should change this” ideas die before reaching that form?  
- Where do submissions go, and who owns them?

No reporting/submissions → problems circulate as opinions, not as objects decision makers must grapple with.

---

## 4. The implementation cycle: from decisions to lived rules

Once a submission exists, a different set of failures often kick in.

### 4.1 Decision – who actually turns submissions into rules?

Here we’re talking about **decision makers**, not just “people in the room”.

Examples:

- A risk committee that must approve changes to AI usage policies.  
- A regulator or board that must adopt changes to binding rules.  
- An internal standards body that can approve or reject new control requirements.

Exec questions:

- For this rule set, who are the **decision makers** by role?  
- Do submissions have clear paths and SLAs to a decision?  
- How many sit “under review” for months with no outcome?

No decision → governance debt builds by default. Submitted changes become a graveyard.

---

### 4.2 Announcement – telling the ecosystem the rule has changed

Decision without Announcement is a ghost change.

Announcement is the formal act of making the rule change visible *inside* the rule ecosystem:

- what has changed,  
- when it’s effective from,  
- what it replaces or retires,  
- who and what it applies to.

Examples:

- Publishing a new AI usage policy with effective date and scope, and clearly flagging which previous directives are now deprecated or retired.  
- Issuing a revised eligibility rule with a clear statement about applicability and transition.

Exec questions:

- When we approve a change, how is that **announced** in a place rule users recognise as authoritative?  
- Can a rule user see, in one place:
  - what governs them now,  
  - what changed,  
  - when,  
  - and who authorised it?

No announcement → nobody can tell which rules are “real” now.

---

### 4.3 Communication – making rules understandable and usable

Announcement is “this is now a rule”. Communication is “here’s what that actually means for you.”

Examples:

- Translating a new AI policy into role-based guidance:
  - concrete examples of allowed and prohibited uses,  
  - simple checklists for common tasks,  
  - FAQs on edge cases.  
- Providing implementation notes for engineering teams:
  - what needs changing in systems, logs, workflows, approval flows.

Exec questions:

- For each critical rule, what concrete **Communication** do rule users see?  
- Is it written for their context, or are they left to interpret policy text alone?  
- Can two teams explain the rule the same way?

You can have flawless Announcement and still have zero real Communication. That’s how rules become theatre.

---

### 4.4 Enforcement – alignment, not punishment

Enforcement in OMGS is not about satisfying the urge to “hang someone”. It’s about:

> Acting on rule users to reduce misalignment between **rule activities** (what’s happening) and **rule content** (what should happen).

Examples:

- Quietly working with teams to correct AI usage patterns before harm escalates.  
- Applying sanctions only after clear Communication and opportunities to correct.  
- Requiring remedial actions when monitoring shows consistent non-compliance.

Exec questions:

- Where, and how, do we actually **enforce** these rules?  
- Is enforcement predictable and proportional, or episodic and political?  
- Do we use enforcement to learn and align the system, or just to signal blame after scandals?

When enforcement becomes purely punitive, people:
- hide problems,  
- avoid raising issues,  
- and governance loses legitimacy.

---

## 5. Where the lifecycle breaks in practice

You can probably already see where your own system breaks. Here’s a structured way to name it.

### 5.1 Environment & Monitoring failures

Patterns:

- No named owner for Monitoring.  
- Dashboards that show “activity” but never compare it to what rules assume.  
- External changes (laws, standards, tech shifts) not tracked against rule content at all.

Result: rules drift off into fantasy while reality moves on.

---

### 5.2 Analysis & Reporting failures

Patterns:

- Monitoring generates noise, but nobody has the mandate or time to do real Analysis.  
- Analysis happens informally; nothing is packaged as a rule submission.  
- Reporting is treated as “for noting” instead of “for decision”.

Result: issues circulate as concerns, not as objects that must be accepted or rejected.

---

### 5.3 Decision & Announcement failures

Patterns:

- Submissions sit in inboxes and committees with no SLA to a decision.  
- Decisions are made informally but never recorded as such.  
- Announcements are buried: nobody can see what rules are actually current.

Result: everyone feels like “someone up there decided something”, but the rule ecosystem never stabilises.

---

### 5.4 Communication & Enforcement failures

Patterns:

- Policy changes emailed once, then lost.  
- No practical guidance for rule users:
  - no role-based explanation,  
  - no system-change checklist,  
  - no examples.  
- Enforcement only appears when something goes wrong in public:
  - selective punishment,  
  - no systematic alignment.

Result: rules are experienced as arbitrary, reactive, and unfair – the opposite of legitimacy.

---

## 6. What leaders can actually *have* if they use this lifecycle

You don’t need to “implement OMGS”. You can simply use this lifecycle as a lens and get a few concrete artefacts you don’t have today.

### 6.1 A one-page rule ecosystem + lifecycle map

For one critical domain (e.g. AI usage, safety-critical decisions, privacy), you can put on a single A3/A2:

- key **rules** and **rule resources** (systems, models, data),  
- the **rule users** they govern,  
- the **rule makers** and **decision makers**,  
- and the lifecycle flows:
  - Monitoring → Analysis → Reporting → Decision → Announcement → Communication → Enforcement.

That map becomes:

> the governance picture you walk into a meeting with,  
> instead of a stack of policy PDFs.

I’ll show an example of what this kind of map looks like in the future rule ecosystem piece, but you don’t need to wait for that to sketch a rough version in your own domain.

---

### 6.2 A live dashboard of rule administration activity

Without creating more bureaucracy, you can start tagging the governance work you already do:

- Monitoring events, analyses, submissions, decisions, announcements, communications, enforcement actions.

Once that’s logged in a structured way, you can see:

- rules with lots of Monitoring but no Reporting,  
- submissions piled up between Reporting and Decision,  
- decisions that were never Announced or Communicated,  
- rules with zero Enforcement activity despite obvious misalignment.

That’s the shortest path to seeing where your **governance debt** really lives.

---

### 6.3 A visible pipeline of rule submissions

Treat rule submissions as first-class objects and track them:

- `Submitted → Under analysis → Ready for decision → Decided → Announced → Communicated → Enforcement in progress`.

Leaders can then ask:

- “Why are these high-risk submissions stuck between Reporting and Decision?”  
- “Why have these decided changes not yet been Announced or Communicated?”

It turns “we’re working on it” into a visible flow.

---

### 6.4 An incident review lens that doesn’t humiliate you

For each significant incident or AI issue, you can ask:

- Where did environment change show up (or not)?  
- Did Monitoring see it?  
- Was there any Analysis?  
- Did anyone produce a rule submission?  
- Did it reach a Decision?  
- Was there an Announcement?  
- Did Communication actually reach rule users?  
- Was Enforcement attempted – and in what spirit?

That doesn’t make failures painless, but it lets you say:

> “We failed at these specific stages of the lifecycle, and here’s how we’re fixing those stages – not just this one rule.”

---

### 6.5 Templates and scaffolding

To make this easier, I’m publishing some lightweight templates in the OMGS (Open Meta-Governance Standard) repository:

- a **rule lifecycle register**  
- a **rule submission log**  
- a **rule ecosystem map** skeleton

They’re not prescriptive. They’re scaffolding you can adapt to your own environment.

---

## 7. Where lifecycle stops – and why rule content needs its own standard

The lifecycle and ecosystem lenses give you:

- a way to see **who sits around rules**,  
- a way to see **how rules move in time**,  
- and a way to **reconstruct** what happened under pressure.

They do not magically fix **rule content** itself.

A perfect lifecycle can’t save a rule that is:

- so vague you can’t tell when it’s broken or satisfied,  
- so internally inconsistent that no Monitoring or Enforcement can be wired to it,  
- so context-free that rule users can’t see themselves in it at all.

If you want Monitoring, Analysis, Announcement, Communication and Enforcement to work, rules have to be:

- **monitor-ready** – you can attach real observation and metrics to them,  
- **machine-ready** – expressible in a form AI systems and orchestration layers can work with,  
- **rationale-visible** – you can see why they exist and what they’re trying to protect.

That’s where **rule content standards** come in.

In a later piece, I’ll look at what it means to write rules in a lifecycle- and machine-ready way: content patterns that make governance operational, not just aspirational – for humans, and for AI systems that will increasingly share this workload.

---

## 8. Closing invitation

If you’re running AI governance, policy, risk, or architecture and any of this feels uncomfortably familiar, don’t start with a program.

Start with a slice.

Pick one rule set that really matters – in AI, safety, benefits, credit, whatever your critical domain is. Sketch:

- the **ecosystem** around it (users, resources, makers, decision makers, external factors), and  
- the **lifecycle** it actually goes through (or fails to) across Monitoring, Analysis, Reporting, Decision, Announcement, Communication, Enforcement.

If you want a starting point rather than a blank page, the OMGS draft and the templates in the open repo are there to steal from and adapt.

And if you do try this and can share anonymised maps or failure patterns, I’m interested in seeing them. That’s the kind of material that should shape the next iterations of open meta-governance – not just more principles on paper, but lifecycles that actually move. Some of that learning will flow back into the OMGS draft itself and into the future rule ecosystem piece, where I’ll show full actor–resource maps and example diagrams.
