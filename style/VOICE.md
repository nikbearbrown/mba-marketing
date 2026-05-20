# Voice anchor — *Principles of Marketing with LLMs*

*Per-book voice spec. Read by every chapter generator before drafting. Overrides root `style/VOICE.md` on conflict per CLAUDE.md §10.*

*Locked: 2026-05-09. Calibration anchor: `chapters/02-marketing-and-customer-value.md`.*

---

## What this voice is

A **Feynman × MKBHD hybrid**. Two intellectual postures in one register.

**From Feynman:** explanation from first principles; intellectual honesty about what the model hides; willingness to say "the framework breaks down here"; the test that the student should be able to explain the idea to a friend in two minutes; jargon translated, never deferred.

**From MKBHD:** the design-philosophy lens. Every product, every campaign, every framework is *evaluated*: what was it optimized for, and what was sacrificed? Ecosystem thinking — no single P, no single decision, evaluated alone. The interest is in the system of choices, not in the single feature.

The combination is well-suited to marketing as a subject. Marketing is exactly the discipline where you have to evaluate trade-offs in product, price, place, and promotion as a system, and where the temptation to memorize names instead of understanding mechanisms is highest.

---

## Structural commitments — non-negotiable across every chapter in this book

1. **Front matter, in this order, no exceptions:**
   - H1 chapter title
   - One-line italicized chapter epigraph
   - **Learning Objectives** — numbered list of 6–10 specific, testable competencies. Each begins with a verb (Define, Compute, Identify, Distinguish, Decompose, Apply, Trace, Evaluate). The objectives are the contract; the exercises must each test a named objective.
   - **Prerequisites** — name what the student must already know. If there is a technical prerequisite, point them at how to get it (e.g., "ask an LLM to explain what a ratio is").
   - **Why This Chapter Matters** — 3–4 paragraphs. Why this material in particular, why now in the book, what downstream chapters depend on it. Honest. Not "this is important because it's important."

2. **Three concept sections.** Each follows the same internal structure:
   - **The motivating puzzle** — a real example. Not invented. A specific firm, a specific decision, a specific outcome. Source-verified.
   - **The mechanism** — the model unfolded. Equation if there is one. Definitions in plain English on first use.
   - **The trade-off** — what the model optimizes for, what it sacrifices. *This is the MKBHD move and it is non-negotiable.*
   - **Worked example** — run the model on a specific case. Show the math. Walk the case end-to-end.
   - **Common misconceptions** — at least one wrong reading of the framework that students reliably arrive at. Name it, correct it.

3. **Integration section** — the chapter's three concepts assembled into one picture. May include the connecting process (e.g., the 5-step marketing process), the historical evolution (where did this thinking come from?), and the boundary (where does the math stop being allowed to operate?).

4. **Exercises — graduated and tagged.** Four difficulty tiers:
   - **Warm-up** (3 exercises, Difficulty: Low or Low-medium) — recognition and direct application
   - **Application** (3 exercises, Difficulty: Medium) — multi-step problems
   - **Synthesis** (2 exercises, Difficulty: Medium-high) — integration across concepts
   - **Challenge** (2 exercises, Difficulty: High) — open-ended; honest answers may be debatable

   Every exercise carries:
   - A bolded title (numbered 1–10)
   - The full prompt
   - An italicized footer: *Tests: Objective N (or Objectives N, M). Difficulty: [tier].* Followed by one sentence of pedagogical justification.

5. **Chapter Summary — three named beats.** "What you can do now that you could not do before this chapter" / "The one idea that matters most from this chapter" / "The common mistake to watch for." Then a fourth beat: **The Feynman test** — a specific question the student should be able to answer in two minutes if they have internalized the chapter.

6. **Connections Forward** — name the next chapter, what other chapters in the book unpack which Ps or which frames, and the through-line of the book. The student should leave knowing where the chapter sits in the larger architecture.

7. **End-matter footer** — italicized voice anchor reminder + source attribution (one-liner naming the OpenStax modules used). No "What would change my mind," no "Still puzzling," no tags. Those are essay conventions, not textbook conventions.

---

## What this voice is *not*

- **Not** the workshop's `feynman` plugin baseline. That voice opens with a puzzle and ends by handing judgment to the reader; this voice opens with structure (LOs, prerequisites) and closes with a self-test. Different audience contract.
- **Not** the workshop's `fry` plugin (Attenborough × Feynman). No cold-open-mid-scene at the chapter level. No "moral weight at the end, not the start." No author first-person ("I had to think about this for three weeks") in body text.
- **Not** the OpenStax baseline. OpenStax is institutional, definition-forward, and avoids evaluation. This voice evaluates.
- **Not** lecture notes. No source-faithful summary register. Drafts that read like polished OpenStax prose are wrong for this voice; the chapter is supposed to *interpret* OpenStax, not paraphrase it.

---

## Voice and stance

- **Authority earned through evaluation.** The voice has a view. It is willing to say "this is a $B$ lead, not a product lead," "the model breaks down here," "the firms that win sustainably almost always do $B$ work, not $P$ work." Never asserted by credential; always earned by walking through why.
- **Direct address: "you," not "the student."** "You can take any market…" "You will need the concept throughout the book." The reader is treated as the colleague who is going to use this, not the apprentice who is being lectured.
- **"We" sparingly, for genuine collaborative reasoning.** "We will test each framework against real examples." Not for false-modesty exposition.
- **No first-person "I."** This is a deliberate departure from the root `style/VOICE.md` Author Direct Address rule. For this textbook, the voice is institutional with a viewpoint, not personal narration. The Nik byline lives on the cover; the chapter speaks in editorial third-and-second person.

---

## Rhythm rules

- **Vary sentence length on purpose.** Short sentences land judgments: *"Confusion is death."* Longer sentences carry argument and accumulation.
- **Single-sentence paragraphs at pivots.** *"That something has four layers."* Used to mark the transition from setup to mechanism, or from mechanism to consequence.
- **Bolded terms on first technical use.** **product**, **price**, **place**, **promotion** — bolded when introduced. The student is being given vocabulary; mark the moment vocabulary is being given.
- **Parenthetical clarifications work hard.** "(Difficulty: Medium-high)" "(born 1946–1964)" — give exactly the disambiguation the student needs without breaking sentence flow.
- **Equations in display mode.** $V = B/P$ rendered as `$$V = \frac{B}{P}$$` when the equation is the point of the paragraph. Inline `$V = B/P$` when it is a callback.
- **Code-block voice for math.** When the chapter is computing on the page (worked examples), the math is *visible*. Not "the model gives us…" but "$V_2 = \frac{B}{70} \approx 1.14$." Numbers with cadence.

---

## Image conventions

- **Inline HTML comment placeholders, not separate `[FIGURE: NN]` syntax.** Format:

  `<!-- → IMAGE: [brief]. [Pedagogical purpose.] -->`

  `<!-- → INFOGRAPHIC: [brief]. -->`

  `<!-- → TABLE: [columns]. [Why these columns.] -->`

  `<!-- → DIAGRAM: [structure]. [What the student should see before reading]. -->`

  `<!-- → CHART: [type]. [What the student should see]. -->`

- **Five image categories.** IMAGE (photographic / scene), INFOGRAPHIC (concept stack, hierarchy), TABLE (multi-column comparison), DIAGRAM (structural relationship, e.g., concentric rings, four levers), CHART (data over time, ratio, distribution).

- **Each placement is an editorial choice.** The brief includes *why* the image goes where it goes — usually because the student needs the structure before the prose unpacks it, or the comparison before the explanation justifies it.

- **Target ~6–10 image placeholders per chapter.** Chapter 2 has 10. This is the upper bound for a long, dense chapter; thinner chapters land at 6–8.

- **The separate `images/[chapter-slug].md` companion file becomes a manifest, not a brief spec.** It indexes the inline placements and tracks any cross-chapter image conventions. Briefs themselves live in the chapter file.

---

## Forbidden phrases (cut on sight)

- "It could be argued that…" — make the argument or cut.
- "Some experts believe…" — name them.
- "Obviously" / "clearly" — if it were obvious, the sentence would be unnecessary.
- "In many ways…" — which ways?
- "The data suggests…" — *shows*, *demonstrates*, *complicates*, *fails to distinguish* — choose.
- "Stakeholders" when you mean *people*.
- "Robust" / "scalable" / "best-in-class" without explaining what you mean.
- "Cutting-edge" / "innovative" / "revolutionary" — describe what specifically changed.
- Technical terms used before being defined.
- Any sentence that could appear unchanged in a corporate marketing brochure.
- *"Fascinating"* / *"remarkable"* without showing why.

## Replacements

- "Here is what is actually happening…" / "Watch what happens when…"
- "The model forces vague intuitions into specific questions."
- "What was optimized for? What was sacrificed?" *(the MKBHD move)*
- "$X$ is doing most of the work in that sentence." *(the Feynman move)*
- "The interesting trade-off is…"
- "This is humbling. It is also…" *(the move that lets a difficult truth land without defensiveness)*

---

## Numbers and citations

- **Every contested factual claim carries a primary-source link.** Per CLAUDE.md §7 hard rule #3.
- **Every statistic is named to its source on first use.** "Mintel research found that 56 percent of U.S. consumers stop buying from companies they believe are unethical." Not "research shows."
- **No invented numbers.** No back-of-envelope estimates passed off as findings. If certainty isn't available, write `[verify]` inline and flag for review.

---

## How this voice handles trade-offs (the MKBHD move)

Every concept section includes a sub-section called **The trade-off**. The structure:

> If you do X, you get [benefit]. The cost is [specific sacrifice]. Firms that do X well almost always also [downstream choice]. The mistake is [misreading the trade-off as one-sided].

Examples from Chapter 2:

- $V = B/P$: *"Cutting $P$ is fast, visible, and immediately reversible — but it costs you margin on every sale and is trivially easy for competitors to copy. Raising $B$ is slow, expensive, and hard to copy."*
- 4Ps: *"All four have to lean the same direction for the customer to read them as a coherent offer. A premium-priced product on Amazon next to a $9 knockoff is doing two of its Ps in opposite directions."*
- Three environments: *"Spend most of your decision-making energy on what you control, but most of your attention on what you cannot."*

A chapter that doesn't name the trade-off in each concept section has not yet earned the voice. Send it back.

---

## How this voice handles ethics and limits

- **Ethics is the *boundary*, not the topic.** Ethics gets a section in chapters where it applies, not a sticker. The frame: *the math gives you the leverage; ethics defines the domain over which the math is allowed to operate*.
- **Model limits get named.** When a framework breaks down at edges, the chapter says so. Chapter 2: *"The relationship between $P$ and $B$ is not independent."* This is honesty, not hedging.
- **No false confidence.** "The evidence does not yet distinguish X from Y" is stronger than "X is proven."

---

## The combined test — every chapter passes before delivery

1. **Front matter complete?** Title, epigraph, LOs, Prerequisites, Why This Chapter Matters — all present and in order.
2. **Three concept sections, each with the five-part internal structure?** (puzzle / mechanism / trade-off / worked example / misconceptions)
3. **Trade-off named in every concept section?** What was optimized for, what was sacrificed.
4. **Worked example shows the math?** Or the case end-to-end if no math.
5. **Misconceptions section names a real student error?** Not a strawman.
6. **Integration section connects the three concepts to the larger frame?**
7. **Exercises tagged with objectives and difficulty?** Mix of warm-up / application / synthesis / challenge.
8. **Summary uses the four named beats?** "What you can do" / "The one idea" / "The common mistake" / "The Feynman test."
9. **Connections Forward names specific subsequent chapters?**
10. **Voice anchor footer + source attribution present?**
11. **Image placeholders are inline HTML comments, mixed across the five categories?** Roughly 6–10 per chapter.
12. **Every statistic cited?** Every brand named is in source?
13. **No forbidden phrases?**
14. **No first-person "I" in body text?** Author voice is editorial.

If all 14 pass, the chapter is in voice. If any fail, the chapter is not yet ready.

---

## Relationship to root `style/VOICE.md`

The root `style/VOICE.md` defines the `fry` voice (Attenborough × Feynman) for the workshop's longread/essay form. This per-book voice is *different*. Per CLAUDE.md §10, this file overrides the root on conflict. Specifically:

- **Cold open at chapter level:** root says yes, this book says no (chapter opens with structure; cold-open-in-scene is reserved for the concept section's "motivating puzzle").
- **Author first-person:** root says light hand but allowed; this book says no in body text.
- **Moral weight delayed to end:** root rule; this book replaces with explicit ethics-as-boundary section.
- **No 3 suggested titles, no TL;DR, no "What would change my mind," no "Still puzzling," no tags.** Replaced by Learning Objectives + Prerequisites + Why This Chapter Matters at front, and Summary + Feynman test + Connections Forward at back.

The root voice's standards on numbers, citations, no fabrication, primary sources, and forbidden phrases all carry over without modification.

---

## What's still open

- **Plugin naming.** This voice doesn't match `feynman`, `fry`, or `emma` from CLAUDE.md §6. Two paths: (a) treat it as a per-book override of `feynman` and document the override, or (b) introduce a new plugin name (candidates: `mkbhd`, `evaluator`, `posture`). Decision pending; for now, the slash command remains `/chapter` and reads this file for voice.
- **Does this voice extend to `/essay` and `/nart` and `/bookmap` for this book?** Probably not — the structural commitments above are textbook-specific. Essays and narratives in this book may need their own voice register. Decision deferred until those forms are needed.
- **Image vendor or generation plan.** The chapter has 10 placeholders; someone has to make 10 figures. TBD.
- **Companion-file convention.** With image briefs inline, the `images/[slug].md` companion file is now a manifest. The pantry and bookmap conventions are unchanged. Confirm with first batch of chapters.

---

*Initial version: 2026-05-09. Revisions logged here on subsequent drafts.*
