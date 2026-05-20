# *Principles of Marketing with LLMs*

*Per-book CLAUDE.md for the `principles-marketing-with-llms` project. Loaded by every chapter generator before drafting.*

*Initial version: 2026-05-09. Locked voice anchor: Chapter 2.*

---

## Title

**Principles of Marketing with LLMs.**

## What this book is

A 23-chapter introductory marketing textbook (Chapters 0–22) built on OpenStax *Principles of Marketing* source material, rewritten in the **Feynman × MKBHD hybrid** voice (see `style/VOICE.md`) and enriched with end-of-chapter LLM exercises that teach the student to use Claude (and other large language models) as a thinking partner for marketing problems. The book teaches marketing first; LLMs are an instrument, not the topic.

## Audience

**Primary:** undergraduate students taking their first marketing course. No prior marketing knowledge assumed. Comfortable with elementary algebra (a fraction is the most technical thing the student will see). Likely to be exposed to LLMs already through ChatGPT or Claude consumer products but not trained to use them as a research or analytical tool.

**Secondary:** career-changers and early-career professionals who want a working understanding of marketing mechanisms — pricing, positioning, distribution, promotion — that they can apply in operating roles. Same prerequisites as the primary audience.

*[TBD with Bear: should this also explicitly address MBA students or stay strictly intro-undergrad? Current default is intro-undergrad; chapter scaffolding is calibrated for that level. MBA-level uplift would be doable through the Challenge tier exercises and bookmap deferred-material expansion, not through chapter prose density.]*

## Scope

**Inside scope:** the standard introductory marketing curriculum as represented in OpenStax — value, marketing mix, marketing environment, consumer/business buying behavior, segmentation/targeting/positioning, marketing research, global and diverse marketplace considerations, the four Ps in detail (product, price, place, promotion in all its forms), customer relationship management, sustainable marketing.

**Outside scope:** advanced quantitative marketing methods (regression-based attribution modeling, bid optimization, lift testing); deep platform-specific tactical detail (the latest Meta ad-format playbook, current Google Ads bidding modes); industry-specific marketing (healthcare marketing, B2B SaaS marketing as their own domains).

**The LLM layer.** The book treats Claude as the primary tool, with adaptation guidance for ChatGPT and Gemini. LLMs appear in two places: inline **Dig Deeper** prompts that invite students to extend a concept and a chapter-end **LLM Exercise** that advances a running project across all 23 chapters. The book's posture toward LLMs is *skeptical-curious*: useful for thinking, often wrong on facts, never authoritative without verification. The book teaches the student to use them well, not to trust them blindly.

*[TBD with Bear: is the LLM posture exactly "skeptical-curious," or is there a different specific stance for marketing? E.g., should the book be openly critical of LLM-generated marketing copy as a category? Default is "skeptical-curious"; revise if a sharper stance fits.]*

## Voice

See `style/VOICE.md`. In one sentence: Feynman's first-principles explanation and intellectual honesty about model limits, paired with MKBHD's design-philosophy lens — every product, campaign, and framework is evaluated for what was optimized for and what was sacrificed.

**Inviolable across all chapters:**

- Front matter: H1 + epigraph + Learning Objectives + Prerequisites + Why This Chapter Matters
- Three concept sections, each with: motivating puzzle / mechanism / trade-off / worked example / common misconceptions
- Tagged graduated exercises (10 total: 3 warm-up, 3 application, 2 synthesis, 2 challenge)
- Summary with four named beats (What you can do / The one idea / The common mistake / The Feynman test)
- Connections Forward
- 6–10 inline image placeholders mixed across IMAGE / INFOGRAPHIC / TABLE / DIAGRAM / CHART
- Voice anchor footer + source attribution
- No first-person "I" in body text
- Every statistic cited; no fabrication

The voice anchor file `style/VOICE.md` overrides the workshop's root `style/VOICE.md` per CLAUDE.md §10 — specifically on cold-open-at-chapter-level (replaced with structured front matter), author first-person (removed in body), and the front/back-matter conventions (LOs + Prerequisites + Why This Matters at front; four-beat summary + Feynman test + Connections Forward at back; no "What would change my mind" / "Still puzzling" / tags).

## Prerequisites

The book assumes:

- Comfort with simple fractions and percentages (the most quantitative thing in the book is $V = B/P$ and basic loyalty-program math).
- Awareness that LLMs exist and basic experience using one as a chat tool.
- No marketing background.

## Chapter architecture

23 chapters total:

- **Chapter 0** — Claude Basics (LLM onboarding; written last during enrichment)
- **Chapters 1–4** — foundations (definitions, value, marketing mix, environment scan)
- **Chapters 5–8** — buyers and information (consumer + business buying behavior, segmentation/targeting/positioning, research)
- **Chapters 9–11** — context and bridge (global, diverse marketplace, mix introduction)
- **Chapters 12–14** — Product P (consumer offerings, new offerings, services)
- **Chapter 15** — Price P
- **Chapters 16–19** — Promotion P (IMC, advertising/PR, personal selling, direct/digital/social/mobile)
- **Chapters 20–21** — Place P (distribution, retailing/wholesaling)
- **Chapter 22** — Sustainable marketing as the new paradigm

## Thin-chapter convention

Three of the OpenStax source chapters are framing modules with very little source content:

- Chapter 1 (Setting the Stage) — 129 source words
- Chapter 4 (Understanding the Marketplace) — 86 source words
- Chapter 11 (Product, Promotion, Price, Place) — 44 source words

**Default treatment:** these are written as **short framing chapters** of 1,000–1,500 words rather than full 5,000–8,000 word chapters. Honest to source per CLAUDE.md State B rule "do not pad." Structurally clean act breaks for the running project that begins in the LLM enrichment pass. The framing chapters keep the front matter (LOs / Prerequisites / Why This Chapter Matters / Connections Forward) but use a single concept arc instead of three concept sections, with abbreviated exercises (4–5 instead of 10).

*[Reversible if Bear prefers: fold thin chapters into the chapter that follows, or expand from primary marketing literature beyond OpenStax. Current default is the short-framing approach.]*

## Citation discipline

All facts, statistics, brand names, quotations, and historical claims trace to the OpenStax source modules in `chapters/[NN]-[slug]/`. Where a chapter compresses or re-orders source material, the bookmap records the trace. No fabrication; CLAUDE.md hard rule #1 governs.

When external corroboration is needed beyond OpenStax (e.g., updated market-share numbers if the OpenStax source is from 2022 and the chapter ships in 2026), the chapter explicitly notes the date of the source and either uses the dated number or marks `[verify with current source]` for Bear's review.

## What's still open (decisions pending Bear)

1. **Audience uplift for MBA / executive audiences** — primary audience defaults to intro undergrad; uplift would change exercise difficulty calibration but not chapter prose.
2. **LLM posture sharpness** — default is skeptical-curious; revise if a sharper stance is wanted.
3. **Career-development sidebar template** — OpenStax has rich career sidebars in many chapters; deferred from Chapter 2; needs a per-chapter template if used.
4. **Source subfolder cleanup** — defer to end-of-run.
5. **Plugin naming** — per-book voice override or new plugin? Defer.

## Cross-references

- `style/VOICE.md` — voice anchor and 14-point combined test
- `outline.md` — *not yet created; chapter-by-chapter purpose statements TBD*
- `pantry/[chapter-slug].md` — reusable ingredients per chapter
- `images/[chapter-slug].md` — image manifest per chapter
- `bookmaps/[chapter-slug].md` — source-to-chapter mapping per chapter

---

*Workshop CLAUDE.md hard rules apply without modification. This file adds book-specific context; it never overrides workshop rules. Voice rules in `style/VOICE.md` override the workshop's root voice spec per CLAUDE.md §10.*
