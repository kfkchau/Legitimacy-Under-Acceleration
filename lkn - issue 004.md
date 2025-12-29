## DRAFT - The Rule Ecosystem: The Missing Foundation of AI Governance 
> Whether you’re governing AI or anything else, you can’t keep rules legitimate if you don’t know who sees reality, who writes them, who decides, and who has to live under them.

Most AI governance stories sound tidy on slides.

- We have principles.  
- We have an AI policy.  
- We have a “human in the loop”.  
- We’re aligning with OECD, UNESCO, NIST, ISO, the EU AI Act.

If you sit inside the organisation trying to make that real, it feels different.

Ask a few basic questions:

- Who can say, “this rule is now wrong for this context”?  
- Who has the authority to retire or replace it?  
- Who actually lives under it every day?

You’ll get five different answers from legal, RAIO, product, ops and the front line.

If you’ve already survived one or two “unified governance frameworks” that never really landed, you don’t need more principles. You need to see the wiring.

This piece is about that wiring – the **rule ecosystem** behind your AI governance.

---

## 1. From rule metabolism to rule ecosystems

In an earlier article I called out **governance debt**: the backlog that forms when *rule intake outpaces rule metabolism*.

- New policies, standards and controls keep piling up.  
- Almost nothing gets retired.  
- Contradictions are handled in meetings and workarounds, not in the rulebook.

AI accelerates that debt. Rules can’t change at the tempo of reality.

That piece focused on **tempo** – how rules move (or don’t) through their lifecycle.

This one goes one step upstream: the **ecosystem** around each rule that decides whether metabolism can work at all.

You can’t design a healthy rule lifecycle if you don’t know **who** sits around the rule, and **how** they’re currently failing each other.

---

## 2. Rules don’t live in PDFs – they live in ecosystems

We talk about “rules” as if they were static artefacts: a policy, a regulation, a standard.

In practice, every serious rule sits inside a web of:

- people who **see reality changing**,  
- people who **write and maintain** the rule,  
- people with formal **authority** to adopt or retire it,  
- people and systems who **live under** it in daily work.

When that web is implicit, three things happen:

- rules accrete without ownership,  
- enforcement drifts and becomes discretionary,  
- changes happen ad hoc or only after a crisis.

AI didn’t invent this problem. Privacy law, health regulation, welfare systems and infrastructure approvals were already showing the cracks.

AI just pushes on **every weak joint at once**:

- more data, more automation, more coupling, more speed.

If you want AI governance that works outside of slide decks, you need a clear picture of the rule ecosystem you already have.

---

## 3. Four roles around every rule (and the hidden plumbing)

You can slice this ecosystem many ways. I use a simple four-role lens because it travels across domains and doesn’t require a re-org.

Around any serious rule, you’ll find:

### 3.1 Rule Environment – what’s actually happening

The **Rule Environment** is the facts on the ground:

- data, behaviour, incidents, edge cases, constraints, shocks.

For AI, that includes:

- model behaviour in production,  
- user workarounds and “shadow AI”,  
- adversarial inputs and weird prompts,  
- near misses in operations.

In other domains, it’s:

- Horizon-style anomalies in post office accounts,  
- repeated misclassifications in a benefits system,  
- infrastructure projects stuck in years-long queues.

The environment includes how **rule resources** and **rule users** behave in reality:

- rule resources: the systems, assets and objects the rules actually govern  
  (servers, models, data, forms, ships, planes, bank accounts, land, etc.)  
- rule users: how the people subject to the rules actually act under them.

This is where reality lives.

### 3.2 Rule Makers – who writes and maintains the rules

**Rule Makers** are the people who design, draft and maintain rules:

- policy teams, RAIO teams, standards authors, architects,  
- people who turn high-level principles into concrete obligations.

They decide:

- how to phrase the rule,  
- where it sits,  
- how detailed or vague it is,  
- what guidance sits next to it.

### 3.3 Decision Makers – who has formal authority

**Decision Makers** are the people or bodies who have the authority to:

- adopt a rule,  
- change it,  
- or retire it.

Executives, boards, regulators, risk committees, steering groups.

They don’t write the rule line-by-line. They decide:

- “do we do this at all?”,  
- “do we change it now?”,  
- “do we live with this trade-off?”

### 3.4 Rule Users – who lives under the rule

**Rule Users** are the people and systems who live under the rule in daily work:

- engineers and product teams,  
- caseworkers, clinicians, teachers, call-centre staff,  
- internal AI agents calling tools,  
- external users who feel the rule as friction or constraint.

They experience the rule as:

- “what I’m allowed to do,  
- what I’m expected to do,  
- and what I’ll get in trouble for.”

They are the ones the rule actually **applies** to – its targets and its intended beneficiaries.

### 3.5 The plumbing: rule resources and rule administration

Between these roles sit:

- the **rule resources** – the things directly governed by the rule:  
  systems, data, workflows, assets, contracts, devices, money, infrastructure;  
- the **rule administration** – the processes and tools for keeping rules alive:  
  how rules are registered, updated, communicated, enforced and logged.

Those are the channels the four roles use to interact:

- Environment signals captured in logs and incident systems,  
- Rule Makers drafting in policy tools and wikis,  
- Decision Makers approving via minutes and registers,  
- Rule Users interacting with portals, KBs, workflows and forms.

If you zoom out, you don’t need every technical detail.

What matters is:

> For any given rule,  
> who sees reality,  
> who writes,  
> who decides,  
> who lives under it –  
> and how they’re (not) talking to each other.

---

## 4. Where rule ecosystems fail: the four edges

Most governance failures don’t start from “no rule”.  
They start from **edges** between these roles not working.

### 4.1 Environment → Rule Makers: reality doesn’t become input

**What this edge should do**

Turn real-world signals into:

> “this rule may now be wrong, incomplete, or harmful.”

**How it fails**

- Signals sit in logs, tickets, complaints, local workarounds.  
- No one with rule-making power sees them, or sees them too late.  
- Staff learn that surfacing problems goes nowhere.

**AI example**

- Front-line staff repeatedly override an AI triage suggestion because it’s obviously wrong.  
- That pattern lives in exceptions and anecdotes, not in any formal channel to the people who wrote the AI usage policy.

**Non-AI example**

- Years of anomalies in a financial system or post-office accounts,  
- treated as individual errors, never as “this core assumption in the rule might be wrong”.

When Environment → Rule Makers is weak, your rulebook and reality slowly diverge.

---

### 4.2 Rule Makers → Decision Makers: fuzzy options, optics-driven decisions

**What this edge should do**

Turn “we have a problem” into:

- clear options,  
- with risks and trade-offs surfaced,  
- and a recommendation.

**How it fails**

- Rule Makers send up:
  - vague problem statements,  
  - over-long decks with no sharp options,  
  - or “we should probably do something about…”  
- Decision Makers:
  - underreact, overreact, or delay,  
  - make decisions that look driven by optics and short-term pressure  
    rather than by a clear, stable rationale,  
  - and the reasoning never gets written down.

**AI example**

- RAIO says “we should restrict this general-purpose AI tool” without concrete scenarios or options.  
- Executives oscillate between “ban it” and “full speed ahead” based on headlines, not structured choices.

**Non-AI example**

- Infrastructure approval processes everyone agrees are broken,  
- but proposals for change are either too abstract or too detailed,  
- so nothing moves.

When Rule Makers → Decision Makers is weak, governance feels arbitrary even to people inside.

---

### 4.3 Decision Makers → Rule Users: decisions no one can see

**What this edge should do**

Communicate change from a **source Rule Users recognise as legitimate**:

- what changed,  
- from when,  
- who decided,  
- what it means for specific roles and systems.

**How it fails**

- Decisions get buried in:
  - meeting minutes,  
  - intranet announcements,  
  - scattered emails.  
- Rule Users discover changes only when they trip over them.  
- Different teams live under different de facto versions of the rule.

**AI example**

- A leadership decision about where AI can/can’t be used lands as:
  - rumours,  
  - half-remembered Slack threads,  
  - local interpretations.  
- Engineers only find out at late-stage review that “this use isn’t allowed anymore”.

**Non-AI example**

- A migrant arriving in a new country is bound by thousands of pages of rules scattered across government websites.  
- They can miss out on benefits they’re entitled to – or fall into breach of obligations – not out of bad intent, but because the system never made the rules findable or legible to them.

When Decision Makers → Rule Users is weak, you get **paper governance**: rules exist, but they don’t govern behaviour.

---

### 4.4 Rule Makers → Rule Users: no “Tuesday translation”

**What this edge should do**

Translate rule text into:

> “What do I do differently on Tuesday?”

**How it fails**

- Policies are written in high abstraction:
  - “ensure fairness”,  
  - “respect privacy”,  
  - “act proportionately”.  
- In the rush to show “we take this seriously”, institutions produce complex, defensive documents optimised for optics and liability, not for clarity.  
- There are no short, concrete guides:
  - how to implement,  
  - what to log,  
  - what to escalate,  
  - what edge cases to watch for.  
- Teams build their own informal interpretations and folk rules.

**AI example**

- “Ensure fairness” becomes:
  - a bullet in a design doc,  
  - an ad-hoc bias check a week before release,  
  - wildly different practices across teams.

**Non-AI example**

- Privacy policies no one can connect to actual workflow decisions,  
- leading to over-blocking in some places and over-sharing in others.

When Rule Makers → Rule Users is weak, you get **governance by folklore**. Rules become something people work around, not with.

---

## 5. AI as a stress test for existing policy domains

If you work in privacy, health, welfare, finance, education, AI doesn’t just add a new thing to govern.

It stress-tests the **rule landscape you already have**.

- Policies that were “just about OK” at human tempo buckle at AI scale and speed.  
- Patches and exceptions multiply.  
- Gaps at the edges become visible and painful.

You have a choice:

- Treat AI as an exception bucket and bolt on:
  - extra forms,  
  - extra committees,  
  - extra one-off controls.  

or

- Use AI as the forcing function to:
  - confront contradictions in your existing rules,  
  - simplify and retire outdated controls,  
  - strengthen the four edges in your rule ecosystem.

AI will push you there anyway. The question is whether you go there deliberately or via crisis.

---

## 6. A practical rule ecosystem map (that plays nicely with what you already use)

This is where exhausted policy and architecture people usually tense up:

> “Is this another new framework that wants to replace everything we’ve built?”

No.

Think of the **rule ecosystem lens** as a thin semantic layer you can lay over whatever you already use:

- RACI matrices,  
- process maps,  
- policy registers,  
- architecture diagrams.

It doesn’t require new tooling or a re-org. It helps you see where responsibility actually sits and where the edges are failing.

Here’s a minimal pattern that works in AI and non-AI domains.

### 6.1 Map the four roles for a small set of critical rules

Start small:

- pick your 3–5 most critical AI-relevant rules or policies:
  - AI usage policy,  
  - AI in hiring, triage, underwriting, customer support,  
  - domain rules where AI is being introduced (privacy, risk, profiling).

For each rule, write down:

- Where does the **Environment** show up?
  - which logs, incidents, tickets, complaints, monitoring systems?  
- Who are the **Rule Makers**?
  - which teams actually draft and maintain the wording and guidance?  
- Who are the **Decision Makers**?
  - who can approve or retire this rule at team / product / org level?  
- Who are the **Rule Users**?
  - which teams and systems live under this rule in daily work?

You don’t need to be perfect. You just need a first honest pass.

### 6.2 Make the edges someone’s job – and find the bottlenecks

For each of the four edges, ask:

- Who is responsible for:
  - channelling Environment signals to Rule Makers?  
  - turning problems into options for Decision Makers?  
  - communicating decisions to Rule Users in one place they trust?  
  - maintaining short, concrete “Tuesday guidance” for Rule Users?

Express this in whatever notation you already use:

- a RACI,  
- a one-page map per rule,  
- an architecture or process diagram.

The point is not the diagram type. It’s that **someone owns each edge**.

Once you draw it, bottlenecks and failure points become visible:

- edges where no-one is clearly in charge,  
- roles carrying too many flows,  
- places where signals routinely die.

That’s the first structural diagnosis. In later work I use lifecycle and meta-governance lenses to go deeper, but most organisations don’t even have this first map.

### 6.3 Tie incident reviews to ecosystem edges – and make rules monitorable

Next time something goes wrong – AI or not – don’t just ask:

- “what went wrong in the system?”

Also ask:

- “which edge in the rule ecosystem failed first?”  
- “who saw what, and why didn’t it flow to the right place?”  
- “was this a rule failure, or an ecosystem failure?”

And a harder question:

- “Could this rule ever have been monitored properly, or is it written so vaguely that no-one could tell if it’s working?”

Good rules are **monitor-ready**:

- they imply observable conditions,  
- you can wire them to metrics or logs if you choose to.

Bad rules are **feel-good**:

- they’re impossible to instrument,  
- impossible to tell if you’re complying,  
- impossible to tie to outcomes.

Over time, asking these questions builds:

- a pattern library of weak edges,  
- and a case for changing structure and rule design, not just adding more controls.

### 6.4 Use AI to justify reworking the landscape, not just patching it

When AI shows up at the edge of an existing policy domain:

- resist the temptation to create an **AI-only annex** that mirrors all your current problems.  
- instead, say:
  - “To govern AI here, we have to simplify and harden the underlying rule ecosystem anyway. Let’s do that work once, in a way that makes AI and non-AI cases easier.”

That is the opposite of the “AI exception bucket” pattern.

### 6.5 Where this fits in my broader work (without selling you a framework)

In my research I fold this into an open **meta-governance kernel** – a reusable way to:

- make the rule ecosystem explicit, and  
- connect it to a rule-change lifecycle (how rules move between draft, active, deprecated, retired).

You don’t need the spec to get most of the benefit.

Most of the impact comes from:

- mapping roles and edges honestly,  
- making sure each edge is somebody’s job,  
- and treating AI as a stress-test that justifies cleaning the landscape, not plastering over it.

---

## 7. What’s next: lifecycles, performance and metabolism

Once you can see your rule ecosystem, the next natural questions are:

- “How do these rules actually **perform** over time?”  
- “How does our **rule administration** perform?”  
- “How do rules move from draft to active to retired without ossifying or exploding in complexity?”

That’s the **rule metabolism / lifecycle** side:

- states (draft, active, deprecated, retired),  
- triggers for change,  
- clear authority,  
- legible trails.

In my next pieces I’ll introduce a lifecycle lens with **domain- and tier-agnostic** rule-administrative steps:

- so you can pinpoint more precisely where bottlenecks and breakdowns come from,  
- and fix them without having to reinvent governance from scratch for every domain.

I’ve already sketched part of this in my article on *the metabolism of rules* – how governance debt forms when rule intake outpaces rule metabolism.

Together, the two lenses – **ecosystem** and **metabolism** – are about one thing:

> Rules that are lived, not just written –  
> and institutions that can adapt them under acceleration without losing legitimacy.

If you’re already mapping this in your organisation – especially around AI, privacy, health, welfare or finance – I’m keen to see what you’ve tried, what’s broken, and what has quietly worked.

That’s where the real pattern library for AI-era rule ecosystems is going to come from.
