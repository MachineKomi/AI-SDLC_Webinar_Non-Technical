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
**"Where We Sit: AI-SDLC"**

*   **The Spectrum (NEW):** Before we dive into prototype vs production, let's position where AI-SDLC sits on the AI adoption spectrum:
    *   **AI-Assisted (Left):** Humans do the core work. AI helps with narrow tasks like autocomplete. This is too conservative — you're underutilizing what's possible.
    *   **AI-Managed (Right):** AI builds autonomously with minimal human involvement. This is too risky — you lose accountability and control.
    *   **AI-SDLC (Center):** AI orchestrates planning and execution. Humans validate and make decisions. **This is us.** This is the sweet spot.

*   **The Key Quote:** "AI-SDLC keeps humans as decision makers. Vibe coding offloads decisions to AI." — Use this to distinguish from prior demo sessions.

*   **Prototype vs Production Cards:**
    *   **Prototype Mode (Left):** "Try things. Break things." Great for learning. High risk, high speed. **Not safe for production data.**
    *   **Production Mode (Right):** "Prove it works." Plan-first, step-by-step, small batches, explicit approval. **"Done" = evidence, not vibes.**

*   **[TRANSITION]:** "So how do we actually DO this on systems that aren't brand new? Let's talk about legacy..."

*   **Interactive Prompt:** "What makes a prototype unsafe to ship to production?"
    *   **[PAUSE FOR DISCUSSION: 60 seconds]** — Ask for 2-3 quick answers from the audience.

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

*   **Improvement Targets (NEW visual):** Point to the metrics bar at the bottom:
    *   **Cycle Time:** From weeks to hours or days. That's the difference between "we'll get to it next sprint" and "let's do it now."
    *   **Iterations:** From sprints (weeks) to bolts (hours/days). Smaller, faster feedback loops.
    *   **Quality:** From variable to consistent. When you have evidence at every step, quality becomes predictable.
    *   **Decisions:** From manual deliberation to AI-informed choices. You still decide, but with better data faster.

---

### 📘 FOR TECHNICAL DEPTH (9-Step AI-DLC Workflow)

*Use this expanded detail for developer-heavy audiences or follow-up workshops. This is the full AWS AI-DLC methodology.*

**Phase 1: INCEPTION (Plan)**
1.  **Build context on existing code** — AI analyzes codebase, reads docs, understands constraints
2.  **Elaborate intent with user stories** — AI proposes stories, humans refine and approve
3.  **Plan with units of work ("Bolts")** — Break into small, verifiable chunks

**Phase 2: CONSTRUCTION (Build)**
4.  **Domain model** — AI creates component/domain models, humans validate
5.  **Generate code and tests** — AI writes, humans review critical paths
6.  **Add architectural components** — AI suggests patterns, architects approve
7.  **Deploy with IaC and tests** — Automated deployment with validation gates

**Phase 3: OPERATION (Prove & Maintain)**
8.  **Deploy in production with IaC** — Infrastructure as code, monitored rollout
9.  **Manage incidents** — AI analyzes telemetry, suggests fixes, humans approve

**Key principle:** Each step builds richer context for the next. Context flows forward, decisions are validated backward.

---

*   **[TRANSITION]:** "So what does 'done' actually look like? How do we know we're not just generating garbage? Let's talk about evidence..."

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
**"Your Role Transforms — Not Disappears"**

*   **Key Message:** This is NOT about replacing anyone. It's about shifting from manual production work to strategic oversight and validation.

*   **Walk Through Each Card (Left to Right):**
    *   **Product / PM:** Before = writing detailed specs manually. AI-SDLC = validate AI-generated stories, approve units, refine intent. Benefit: **Faster elaboration**, less miscommunication.
    *   **QA:** Before = manual test creation, reactive bug tracking. AI-SDLC = validate AI test scenarios, guide optimization. Benefit: **Proactive quality** not reactive.
    *   **Ops / DevOps:** Before = manual pipelines, reactive monitoring. AI-SDLC = approve AI infra recommendations, predictive resolution. Benefit: **Predictive ops**.
    *   **Developer:** Before = code from scratch, manual debugging. AI-SDLC = validate AI domain models, approve architecture. Benefit: **Higher quality** code, faster cycles.
    *   **Architect:** Before = design alone, write detailed specs. AI-SDLC = validate AI logical designs, approve patterns. Benefit: **Faster decisions**, consistent patterns.

*   **The Shift:** Emphasize the footer: "From manual production work → AI-informed validation & strategic decisions."

*   **Non-Developer Inclusion Script:** "Notice this isn't just about developers. Product, QA, Ops, Architects — everyone's role transforms. The expertise you have today becomes MORE valuable because you're validating and guiding AI, not being replaced by it."

*   **[TRANSITION]:** "So how do we actually start this? Let me show you a practical adoption approach..."

---

## Slide 10: Adoption
**"Start Small. Prove Value. Scale."**

*   **The Model:** We recommend a 4-step loop to get this going without boiling the ocean.
    1.  **Align:** Find a use case and a champion. Don't try to change the whole company at once.
    2.  **Experience:** Practice on real work. Not a toy project. Real code, real production path.
    3.  **Adapt:** Tune the method. Your culture is different. Adjust the "bolts" to fit your size.
    4.  **Scale:** Once you have a win, build a community. Let the skeptics see the success.

*   **Win Over Skeptics:** "The best way to win over a skeptic is to clear a blocker for them. Co-create a small win. Use the tools to capture *their* knowledge so they feel heard, not replaced."

*   **The Goal:** Reduce knowledge bottlenecks, speed onboarding, reduce risk — keep the experts, lose the toil.

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
