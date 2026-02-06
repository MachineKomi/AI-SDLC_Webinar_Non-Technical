# Speaker Notes: AI-SDLC Webinar (v6)

**Setup:**
- Open the presentation in your browser (`index.html`).
- Press **F11** for full screen.
- Use **Arrow Keys** to navigate.
- Keep this script open on your second screen.

---

## Slide 1: Introduction
**"From Demos to Delivery"**

*   **The Hook:** We've all seen the magic. You type a prompt, you get code. It feels like a superpower.
*   **The Key Message:** But magic doesn't scale. Magic is unpredictable. If we want to run a business on this, we need a machine.
*   **Include Legacy:** Note the subtitle now emphasizes "including on legacy systems" — this is a headline message, not a footnote.
*   **The Three Pillars:**
    1.  **Speed**: Small batches, fast cycles.
    2.  **Safety**: Explicit approval gates.
    3.  **Proof**: Durable, verifiable artifacts.

---

## Slide 2: Context
**"The Landscape Has Shifted"**

*   **Capability:** It's not "autocomplete" anymore. Models reason about architecture, refactor across files, understand intent.
*   **Pressure:** AI-First teams ship 30-50% faster. Speed is the currency of this market.
*   **The Trap (Risk):** "The Slop Trap" — generating code is easy; verifying it is hard. The bottleneck has moved to review.

---

## Slide 3: Reality
**"Knowledge is Locked in Heads"**

*   **The "Bob" Problem:** Most orgs don't have docs. They have "Bob." When Bob is busy, delivery stops.
*   **The AI Unlock:** When knowledge is captured as artifacts, AI becomes a force multiplier — not a replacement.
*   **Interactive Prompt:** "Where does knowledge live today when someone is out?"

---

## Slide 4: Two Modes
**"Prototype vs. Production"**

*   **This is the bridge** from prior "vibe coding" sessions to real delivery.
*   **Prototype Mode (Left):** "Try things. Break things." Great for learning. High risk, high speed. Not safe for production data.
*   **Production Mode (Right):** "Prove it works." Plan-first, step-by-step, small batches, explicit approval. "Done" = evidence, not vibes.
*   **Interactive Prompt:** "What makes a prototype unsafe to ship to production?"

---

## Slide 5: Legacy
**"Yes, It Helps on Older Stacks"**

*   **This is a headline message.** Don't self-disqualify because your tech is old.
*   **Honest Caveat:** Models are weaker on rare/old languages with less public training data.
*   **Practical Mitigation:**
    1.  Put docs, runbooks, comments in-repo.
    2.  Use retrieval-first (AI reads your docs).
    3.  Add tests, iterate with verifiable checks.
*   **The Visual:** The code block shows an AI agent reading context files and flagging a legacy dependency.

---

## Slide 6: Method
**"Plan. Approve. Build. Prove."**

*   **The Core Loop:** This is the engine we run for every unit of work.
    1.  **Plan:** AI proposes. Vague inputs = bad outputs.
    2.  **Approve:** Human accountability. Catch drift before code is written.
    3.  **Build:** AI executes.
    4.  **Prove:** Evidence over vibes. Tests passing, checks green, behaviour validated.

---

## Slide 7: Evidence
**"Proof Over Promises"**

*   **The Question:** What does "Done" look like?
*   **Old Answer:** A thumbs up in a PR.
*   **New Answer:** A Validation Report. Tests passed, security scan clean, build succeeded, artifact documented.
*   **The Evidence Rule:** A unit is done only when acceptance criteria pass, tests are green, and the validation report documents the proof.
*   **Interactive Prompt:** "What evidence would you need to trust an AI-generated change?"

---

## Slide 8: Collaboration
**"Compress Weeks into Hours"**

*   **Phase 1 — Joint Design (Alignment):**
    *   Product defines value and priority.
    *   Tech sets constraints and feasibility.
    *   QA defines success criteria early.
*   **Phase 2 — Joint Review (Evaluation):**
    *   Dev reviews logic and edge cases.
    *   AI generates code and tests.
    *   Ops validates operational readiness.

---

## Slide 9: Roles
**"Everyone Contributes"**

*   **Accountability:** AI does not own the outcome. Humans own the loss function.
*   **Product / PM / BA:** Intent, acceptance criteria, edge cases, trade-off decisions.
*   **QA:** Test intent early, define evidence, add checks from day 1.
*   **Ops / ProServ:** Operational constraints, supportability, runbooks, rollout.
*   **Everyone:** Capture knowledge. Document decisions. Share what you know.

---

## Slide 10: Adoption
**"Start Small. Prove Value. Scale."**

*   **Step 1:** Pick one thing. Small, bounded, clear acceptance criteria.
*   **Step 2:** Run with evidence. Force the "Proving" step. No shortcuts.
*   **Step 3:** Capture knowledge. Use the tools to document what the experts know.
*   **The Goal:** Reduce knowledge bottlenecks, speed onboarding, reduce risk — not replace experienced people.

---

## Slide 11: Discussion
**"Let's Discuss"**

*   Four key questions embedded:
    1.  "Where does knowledge live today?"
    2.  "What makes a prototype unsafe?"
    3.  "What evidence would you need to trust AI output?"
    4.  "One legacy area you wish was documented better?"

---

## Slide 12: Takeaways
**"It's Time to Build."**

*   **Three Anchors:**
    1.  Plan First — No vibe coding to production.
    2.  Small Batches — Reviewable, reversible.
    3.  Proof over Promises — Evidence, not vibes.
*   **The Quote:** "It's time to build." — Marc Andreessen
*   **Call to Action:** Start this week. Pick one small item. Run the loop. Share the proof.
*   **Note:** A deeper technical workshop is available for developers who want the full detail.

---

## Key Links
- AI-SDLC Explainer: https://ai-sdlc-explainer.vercel.app/
- GitHub Repo: https://github.com/MachineKomi/AI-SDLC_Explainer
