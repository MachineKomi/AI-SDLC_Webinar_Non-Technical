# Speaker Notes: AI-SDLC Webinar

**Setup:**
- Open the presentation in your browser (`index.html`).
- Press **F11** for full screen.
- Use **Arrow Keys** to navigate.
- Keep this script open on your second screen.

---

## Slide 1: Introduction
**"From Demos to Delivery"**

*   **The Hook:** We've all seen the magic. You type a prompt, you get code. It feels like a superpower.
*   **The Problem:** But magic doesn't scale. Magic is unpredictable. If we want to run a business on this, we don't need magic—we need a machine.
*   **The Goal:** Today is about building that machine. How do we ship AI-assisted work **safely**, **consistently**, and at **scale**?
*   **The Three Pillars:**
    1.  **Speed**: We want small batches and fast cycles.
    2.  **Safety**: We need explicit approval gates.
    3.  **Proof**: We need durable artifacts, not just code.

---

## Slide 2: Context
**"The Landscape Has Shifted"**

*   **Capability:** It's not just "autocomplete" anymore. The new models (Claude 3.5, o1) can reason about architecture. They can refactor across files. They act more like junior architects than typing assistants.
*   **Pressure:** The market is moving. AI-First teams are shipping 30-50% faster. Speed isn't a "nice to have" anymore—it's the currency of the new market.
*   **The Trap (Risk):** But there's a trap. We call it "The Slop Trap." Generating code is easy. Verifying it is hard.
*   **The Shift:** The bottleneck in software delivery has moved. It used to be **writing** code. Now, it is **reviewing** code. If we don't change how we work, we'll just drown in unverified code.

---

## Slide 3: Reality
**"Knowledge is Locked in Heads"**

*   **The "Bob" Problem:** Look at the left side. This is most organizations. Knowledge lives in Bob's head. When Bob is busy (or on holiday), delivery stops.
*   **The AI Problem:** If you point an AI agent at this reality, it fails. It hallucinates because it doesn't know what Bob knows.
*   **The Solution (Right Side):** We need **Shared Context**.
*   **The Mechanic:** We have to move knowledge out of heads and into artifacts—docs, specs, rules. When we do that, the AI can read it. And suddenly, the "bus factor" isn't a crisis.

---

## Slide 4: Two Modes
**"Prototype vs. Production"**

*   **Concept:** We need to be honest about what mode we are in.
*   **Prototype Mode (Left):** "Try things. Break things." This is great for learning. It's high risk, high speed. Use this for demos, for exploration.
*   **Production Mode (Right):** "Prove it works." This is for shipping.
*   **The Key:** You cannot "vibe code" your way into production. Production requires a different discipline: Plan first, stage-by-stage, with evidence.
*   **Transition:** Today, we are focusing on the Right side—how to govern Production Mode.

---

## Slide 5: The Method
**"Plan. Approve. Build. Prove."**

*   **The Loop:** This is the core engine of AI-SDLC. It's a loop we run for every unit of work.
*   1. **Plan:** AI proposes a plan. "Vague inputs = bad outputs," so we force clarity here.
*   2. **Gate (Approve):** Human accountability. You approve the plan *before* code is written. Catch drift early.
*   3. **Build:** AI executes.
*   4. **Prove:** This is the most important step. "It runs on my machine" is not enough. We need evidence.

---

## Slide 6: Evidence
**"Proof Over Promises"**

*   **The Question:** What does "Done" look like?
*   **Old Answer:** A thumbs up in a PR.
*   **New Answer:** A **Validation Report**.
*   **The Standard:** A unit is only done when:
    *   Tests pass (Green).
    *   Security scans are clean.
    *   The build succeeds.
    *   **And we have a document proving it.**
*   **Why:** This creates an audit trail. It turns "trust me" into "show me."

---

## Slide 7: Collaborative Operating Model
**"Working Together"**

*   **The Shift:** We're moving from "handoffs" to "collaboration."
*   **Phase 1: Joint Design:**
    *   Product, Tech, and QA sit together (Mob session).
    *   We align on **Intent** before a single line of code is generated.
*   **Phase 2: Joint Review:**
    *   When the AI builds, we review together.
    *   Dev reviews logic. AI generates tests. Rules govern the quality.
*   **Impact:** We compress weeks of "email tag" and Jira comments into a single high-bandwidth session.

---

## Slide 8: Legacy
**"Modernizing Context, Not Just Code"**

*   **The Fear:** "This is great for new apps, but I have a 20-year-old monolith."
*   **The Reality:** AI is actually *better* at legacy than humans are, **if** you give it context.
*   **The Technique:** We call it "Context Injection."
*   **Visual:** Look at the code block. The Agent reads `risk-rules.md`. It spots that the code relies on an old tax table. It flags it.
*   **Takeaway:** You don't have to rewrite the whole system. You just have to document the *understanding* of it. A semantically dense README is the highest-ROI thing you can write today.

---

## Slide 9: Roles
**"Everyone Plays a Part"**

*   **Accountability:** AI does not own the outcome. **Humans own the loss function.**
*   **Product:** Your job is **Intent**. Be clear about what we are building.
*   **QA:** Your job is **Proof**. Define the tests that prove it works.
*   **Ops:** Your job is **Rails**. Set the safety boundaries.
*   **Everyone:** Your job is to **Capture Knowledge**. Stop keeping it in your head. Write it down.

---

## Slide 10: Adoption
**"Start Small. Prove Value. Scale."**

*   **How to Start:** Do not try to change everything overnight.
*   **Step 1: Pick One Thing.** A single feature. A single bug fix. Keep it small.
*   **Step 2: Run with Evidence.** Force the "Proving" step. Do not shortcut the validation report.
*   **Step 3: Share the Win.** Don't just show the demo. Show the *report*. Show the *process*. That is how you build trust.

---

## Slide 11: Discussion
**"Let's Discuss"**

*   *facilitator note: Open the floor for these questions.*
*   "Where does knowledge live today?" (Is it Bob?)
*   "What makes a prototype unsafe?" (Lack of tests? Security?)
*   "One legacy area to document?" (Where is the biggest risk?)

---

## Slide 12: End
**"It's Time to Build."**

*   **The Quote:** Marc Andreessen said it best.
*   **The Mandate:** It's not enough to talk about AI. It's time to build the machine that delivers it.
*   **Call to Action:** Start this week. Pick one item. Run the loop. Share the proof.
*   **Closing:** Thank you. Let's get to work.
