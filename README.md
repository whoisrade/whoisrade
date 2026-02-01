# Rade Joksimović

I design AI SaaS systems where early decisions determine whether the product stays understandable—or becomes something no one can fully explain.

---

## The question I start with

**"What happens when this works?"**

Everyone asks what happens if it fails. I ask what happens when it succeeds:

- When 10x more users hit this endpoint
- When the team doubles and no one remembers why it was built this way
- When AI costs scale with usage but revenue doesn't
- When a feature works so well that users depend on it in ways you didn't design for

Most architectural debt comes from success, not failure. I design for that.

---

## What I've learned the hard way

**On data modeling:**
The database choice isn't about features—it's about how you'll be charged. Per-operation pricing punishes dense, sustained workloads. Storage-based pricing punishes sparse workloads with high provisioned capacity. I've picked wrong before. A 3-month migration from document to relational storage taught me to model the cost curve before modeling the data.

**On infrastructure:**
Managed platforms are for iteration speed. Owned infrastructure is for control, isolation, and margin. The mistake is treating managed as the destination instead of a phase. When your constraints shift from "ship fast" to "tenant isolation" or "predictable unit economics," you've already waited too long to migrate.

**On AI costs:**
The biggest waste isn't the model. It's the recomputation you don't see—retry loops, regeneration cascades, context that should've been cached but wasn't. In one system, I traced 40% of token spend to interactions that never needed to hit the model twice. The fix wasn't prompt engineering. It was UX and state design.

**On UX:**
Every "undo" is a recomputation. Every "regenerate" is a confession that the system guessed wrong. I redesign the interaction before I optimize the pipeline. The cheapest token is the one you never send.

---

## What most engineers don't do (but I learned to)

**Sit in session recordings.**
I've spent hours watching real users struggle with interfaces I designed. Clarity, FullStory, LogRocket—not for heatmaps, but to see the hesitation before the click. That's where the recompute starts.

**Model incentives before systems.**
I ran a regulated fund where fee structures could create misaligned behavior between us and investors. That experience trained me to see where system design creates perverse incentives—in pricing, in UX, in how teams interact with the product.

**Treat infrastructure as product economics.**
I've moved systems from Vercel to self-managed Kubernetes on Hetzner—not for ideology, but because tenant isolation and margin math demanded it. I understand when managed is right and when it becomes a ceiling.

**Design for the audit you haven't been asked for yet.**
Enterprise buyers increasingly want to trace what the AI knew, when, and why. I build provenance into systems before compliance requires it.

---

## How I work

I don't start with best practices. I start with:

1. What does real usage actually look like?
2. Where will failures compound instead of staying local?
3. What's still reversible and what isn't?

Then I change the architecture.

---

## What I won't do

- Take a role where I'm far from the system
- Optimize for titles or org chart position
- Pretend every problem is a technology problem

I do my best work close to the code, accountable for outcomes, partnering with CTOs who need someone to own the hard parts.

---

## Background

- Products scaled to **1.5M+ MAU**
- Teams of **~30** as founder/CEO under board and investor pressure
- **20 years** shipping in production
- Structured a **regulated fund** from zero (governance, fee alignment, multi-venue execution)
- **Google Launchpad mentor**, advised 100+ startups on product and growth
- Design background → still care about **typography, UX, and conversion**
- Now: Principal IC, fully remote

---

> I figure out what should exist—and build it so it stays right.

---

[LinkedIn](https://linkedin.com/in/radejoksimovic) ・ [unit01.dev](https://unit01.dev)
