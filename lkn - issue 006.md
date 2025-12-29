## DRAFT - Why Today’s AI Governance Still Feels Like Theatre to the People Running the Systems  

From the outside, it looks like we’ve made real progress.

We have:  

- **UNESCO** and **OECD** AI principles  
- the **NIST AI Risk Management Framework**  
- the **EU AI Act**  
- **ISO/IEC 42001**  
- and thick binders of corporate “Responsible AI” playbooks  

On paper, it’s a lot.

But if you talk to the people actually **building and operating AI systems**, you hear something different:

> “We’ve got beautiful principles and terrible plumbing.”

This piece is for them.

I’m not arguing that global frameworks are useless. They raised the floor. They gave us shared language, legitimacy and political cover to say “AI governance matters”.

The problem is architectural:  

We’ve treated governance as **statements around the system**, not **machinery inside the system**.

From an operational point of view, five things keep breaking.

---

## 1. Beautiful principles, terrible plumbing

In most organisations today, governance looks like this:

- ethics principles on a slide,  
- a risk framework in Confluence,  
- a model evaluation checklist,  
- a “human-in-the-loop” line in the design doc.

Then you ship.

When the real system misbehaves in production, none of those artefacts tell you:

- how the workflow was actually wired  
- who could call which function, against which rules  
- where the system should have been stopped  
- or how to replay what happened without a week of forensics

On the policy side, UNESCO/OECD/NIST/ISO/EU all make the same move:

- they define **what good AI should feel like** – fair, transparent, accountable, human-centred  
- they define **obligations** for providers and deployers  
- they define **processes** – risk assessments, monitoring, documentation  

But they mostly stop at the boundary of *“the AI system”* as a black box.

Inside the organisation, that lands as:

- “we’re compliant on paper”  
- “…but our pipelines and workflows still run on vibes”

**What’s missing is very simple to describe and very hard to build:**

> Governance that shows up in the wiring:  
> **who can do what, when, with what logs, and who can stop it.**

Until that exists, most governance will feel like theatre to the people in the engine room.

---

## 2. We don’t have a clean map of who should do what

Every framework says some version of:

- “there must be meaningful human oversight”

In practice, “human oversight” usually means:

- somewhere in the slide deck, there’s a bullet saying “a human is in the loop”  
- nobody can agree which **decisions** are actually human  
- nobody can show, in a crisp trail, **why** a particular task was given to AI rather than a person

If you never draw a **task-level map**, “oversight” collapses into a slogan.

From an operational point of view, we need to start from **tasks**, not job titles.

At minimum:

- break work down into **small decisions**:
  - one input,  
  - one transformation,  
  - one output  
- classify them roughly by **reasoning depth**:
  - *Why* – purpose, ethics, improvisation  
  - *How* – method, process, optimisation  
  - *What* – concrete execution  
- and by **information messiness**:
  - structured, semi-structured, unstructured

Then you can say, with a straight face:

- these **Why-tier, high-ambiguity, high-consequence** tasks: human-only  
- these **structured, What-tier** tasks: safe to automate under guardrails  
- these in the middle: AI-assist, with defined checks and explicit logs

In my own work I call this a **task boundary framework** – a reasoning-first way to decide:

> who should do what, under which conditions, with what trail.

You don’t need my label. But without some shared task map, “human oversight” will keep living as a sentence in a PDF, not a property of the system.

---

## 3. Our AI “team” has no constitution

Most organisations are now edging toward **multi-agent** or multi-tool setups, whether they call them that or not:

- a “copilot” that talks to users  
- a chain that calls internal tools  
- retrieval and summarisation layers  
- some monitoring around the edges

But the default pattern is still:

> one **mega-assistant** doing everything:
> - talks to the user  
> - searches  
> - plans  
> - writes  
> - calls tools  
> - self-checks  

No clear roles. No separation of powers. No governance layer with real veto.

It’s like putting a single very smart person in a sealed room with root access and saying “be responsible”.

If you were designing a critical system anywhere else – aircraft, ships, power plants – you would not accept that.

You’d ask:

- where is the **redundancy**?  
- where is the **voting**?  
- where is the **independent safety function** that can cut power if things go weird?

Aircraft don’t rely on one perfect computer. They fly with **triplex redundancy**:

- three computers running in parallel,  
- comparing outputs,  
- cutting out the outlier when they disagree.

A ship’s engine is judged less by “can it hit this speed once?” and more by:

- can it run near max output for **hours** or **days**,  
- self-monitoring,  
- with humans able to intervene,  
- without killing everyone if something misfires.

We keep evaluating AI like students in an exam: *can it pass this one test?*  

In operations, we should care about AI systems the way we care about engines and operating systems:

- not “can it boot once without errors?”,  
- but “can it run for weeks, self-monitor, and fail safely under load?”

Right now, the **global and national AI governance stack** behaves more like a **patch-heavy consumer OS**:

- every new risk adds another guideline, another national layer, another exception  
- helpful in the moment,  
- but not designed as a coherent, long-running substrate

What we actually need is the **server-grade version of governance**:

- a small set of shared primitives – tasks, roles, rights, logs, escalation paths –  
- that different jurisdictions and sectors can implement and extend,  
- while still inter-operating like parts of one operating system rather than a pile of loosely compatible patches.

For AI, we often do the opposite of what we do in real safety-critical systems:

- we obsess over **one-shot benchmarks** (“did it pass this exam?”)  
- but we don’t design for **long-running, self-correcting, fail-safe operation**

An operations-centric governance architecture would look more like:

- a **team of small agents** with narrow, auditable roles:
  - one for extracting facts,  
  - one for checking policy fit,  
  - one for drafting options,  
  - one for user comms,  
  - one for tool access  
- plus a **governance layer**:
  - agents or services whose *only* job is to:
    - enforce boundaries,  
    - watch for risky patterns,  
    - and control starting/stopping and access – even if they never see the content.

With simple rules like:

- if certain governance agents flag a risk, **the whole workflow pauses**  
- if a key “lead” goes down, **a backup cohort** takes over or the human owner must intervene  
- agents cannot be muted or quietly bypassed; only the human owner can override them

I’ve been prototyping this as a governance-first “white-collar AI team” architecture, but the deeper point is simple:

> If you’re going to let AI behave like a team,  
> you need the equivalent of a **constitution**, not a friendly monarch.

Right now, most AI “teams” don’t have one.

---

## 4. When things go wrong, we keep having the same meetings

Ask anyone who has sat through enough AI or system incidents and they’ll recognise this pattern:

1. Something goes wrong.  
2. There’s a post-mortem.  
3. A list of “lessons learned” and action items is produced.  
4. Six months later, a very similar incident happens.  
5. Repeat.

On paper, every framework tells you to:

- “monitor and review”,  
- “continuously improve”,  
- “update your risk assessment”.

In reality, **rule intake outpaces rule metabolism**:

- new policies, controls and insights accumulate,  
- very few rules get retired or fundamentally reworked,  
- nobody is clearly mandated to say:
  > “this rule, in this scope, is now wrong.”

We don’t have a **rule-change engine**. We have meetings.

Operationally, that shows up as:

- known problems that never quite get fixed in the rules  
- “temporary workarounds” that become permanent  
- controls that pile up without a concept of deprecation or retirement  
- the same failure mode showing up under different ticket numbers

A minimal rule-change engine doesn’t require new philosophy. It needs:

- **triggers** – events that *force* a review:
  - repeated incidents of a certain type,  
  - specific drift in metrics,  
  - new evidence about harm  
- **authority** – clarity on:
  - who can declare “this rule is broken” at team / product / org / cross-org level  
- **states** – rules aren’t just “there”:
  - proposed, active, deprecated, retired  
- **trails** – a way to see:
  - when and why a rule changed,  
  - who approved it,  
  - what evidence they relied on

In my own work I call this a **meta-governance kernel** – a small set of rules about how rules change.

You don’t need the spec to get the point:

> Until you treat rule-change as a **designed process**,  
> “continuous improvement” will stay stuck at the slideware layer.

---

## 5. Even when it “works”, people feel their work and worth dissolving

Most AI governance conversations live on the **rule side**:

- risk categories,  
- rights,  
- controls,  
- audits,  
- penalties.

Much less attention goes to the **value side**:

- which work still “counts”  
- whose contribution is visible in metrics  
- what paths through the system are still open to people

I use a city image for this.

- The **traffic system** – laws, lights, signs, enforcement – is the **rules**.  
- The **routes people actually drive** – where they go, which roads crowd, which areas they avoid – are the **value signals**.

AI is hitting both sides at once.

On the rule side:

- we add principles, controls, obligations.

On the value side:

- AI takes over work that people used to rely on to answer:
  - “what am I good at?”  
  - “what do people need from me?”  
  - “what is a respectable life path here?”  
- some forms of effort vanish from dashboards and KPIs  
- whole neighbourhoods of work become:
  - lower-status,  
  - lower-paid,  
  - or structurally precarious

You can be fully compliant with the EU AI Act and your internal RAIO policies, and still end up with:

- a workforce that feels hollowed out,  
- fewer meaningful paths for humans,  
- more invisible care work and glue work with no recognition.

Ethical **value assertion** (“we respect human dignity and autonomy”) does not, by itself, produce **ethical outcomes**:

- if you don’t change how decisions are structured,  
- if you don’t change how contribution is recognised,  
- if you don’t give people real alternatives when old roles erode.

A serious governance conversation has to see **both**:

- the traffic system (rules, enforcement, audits)  
- the routes (what journeys through work and life remain viable and meaningful)

I’m developing this further as a **governance–economic system** lens – how rules and value signals interact under acceleration – but the immediate point is simple:

> Don’t declare AI governance “done”  
> until you’ve looked at what your systems are doing to people’s **future paths**, not just to today’s risk profile.

---

## 6. From governance as decoration to governance as infrastructure

None of this is an argument against UNESCO, OECD, NIST, the EU AI Act or ISO.

They did important first-generation work:

- made AI governance **speakable**  
- anchored it in human rights language  
- created hooks for enforcement and accountability  
- gave RAIO teams air cover

The problem is that we stopped there.

We treated:

- principles as if they were engines,  
- one-shot benchmarks as if they were safety,  
- model-centric risk documents as if they somehow governed **operations**.

From an implementor’s point of view, the next step is not:

- “better commandments”, or  
- “one more meta-framework”

It’s **operational integrity**:

- AI that is evaluated not just on a frontier exam, but on how it behaves in **continuous, self-correcting operation**  
- workflows where **task boundaries** and responsibilities are explicit and reconstructable  
- AI “teams” with **constitutions, not monarchs**  
- rule systems with a **metabolism** – able to change under pressure without collapsing  
- governance that sees both **rules and routes** – the structure of decisions, and the pattern of human lives under them

That’s the shift I’m working on under *Legitimacy Under Acceleration*.

If you’re in a RAIO team, an architecture group, or a policy role and you recognise this gap between **principles and plumbing**, I’m interested in two things:

- the **incidents and near misses** you’ve seen that current frameworks couldn’t really explain, and  
- the **patterns** you’ve already discovered that make AI systems more fail-safe and more human-coherent in practice.

That’s where the next generation of governance will come from: not another set of slogans, but people quietly rebuilding the wiring so that our systems can fail and recover without losing the people they’re meant to serve.

---

© Kelvin Chau, 2025  
This piece is part of the [Legitimacy Under Acceleration](https://github.com/kfkchau/Legitimacy-Under-Acceleration/) project.  
It may be shared non-commercially with attribution but not modified or republished without permission.  
Licensed under [Creative Commons Attribution–NonCommercial–NoDerivatives 4.0 International (CC BY-NC-ND 4.0)](https://creativecommons.org/licenses/by-nc-nd/4.0/)  
For attribution, citation, or inquiries, please refer to:  
🔗 [https://au.linkedin.com/in/kfkchau](https://au.linkedin.com/in/kfkchau)
