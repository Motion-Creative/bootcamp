---
name: motion-bootcamp
description: Answers questions about the Motion 2026 Creative Strategy Bootcamp — 13 recorded sessions across weeks 1–7 covering hooks, persona research, prioritization and diagnosis, AI-assisted ad production, performance analysis, and live coaching. Use whenever a user asks about bootcamp content, a specific session, an instructor or guest speaker (Evan Lee, Sarah Levinger, Dara Denney, Will Sartorius, Jade Heritage, Daniel Rivera, Sophia Beauvoir, Viti Videtta, Janae LeVander, Jake Abrams, Joanna Wallace, Eric Philippou, Sarah Burnett, Matteo Friend, Darcy Tennant, Blaise Ormond, Naomi Peh Haeger, Alysha Boehm), or any framework taught in the course (T-E-E-P, Three Realities Research System, Customer Reality Cake, Hook Analytics Funnel, 3 Altitudes of a Creative Strategist, Hook's 3 Jobs, Top 5 Hook Formats, 50/25/25 Creative Mix, Battleship Mindset, Grocery List Ideation, Cost Iceberg, Alignment Statement, Valence and Intensity Model). Also trigger on quotes, slides, ad critiques, or moments from the Tuesday classes or Thursday coaching calls, on student work reviewed live, and on bootcamp-adjacent topics like Meta's Andromeda algorithm, hook diversity, Claude/Motion workflows shown in coaching, and "ugly ads" / Barry Hott references.
---

# Motion 2026 Creative Strategy Bootcamp

This skill gives you a structured library of the **Motion 2026 Creative Strategy Bootcamp** — 13 sessions across weeks 1–7 of the 8-week curriculum, with both compressed lesson files and verbatim transcript/slide/ad references.

## Important: all files are bundled inside this skill

Every file referenced below is included in this skill's `references/` folder. **Read them as local files via your file-reading tool. Do not fetch them from GitHub, raw.githubusercontent.com, or any URL. Do not run a web search for them.** If you cannot read a referenced file, say so directly — do not try to substitute a URL fetch.

## File layout

```
motion-bootcamp/
├── SKILL.md                                              ← this file
└── references/
    ├── index.md                                          ← router, load first
    └── week-01/ … week-07/
        ├── <session>.md          ← lesson (~5–7K tokens)    ← open by default
        └── <session>.full.md     ← reference (25–100K tokens) ← open only for verbatim
```

Every session has two files:

- **`<session>.md` (lesson)** — frontmatter, summary, chapters, frameworks with full taxonomies, claims, tactics, anti-patterns, named entities, key quotes, time-bound claims, homework, cross-week refs. Coaching sessions also include student questions answered, ads critiqued live, and live worked examples. Answers ~80% of bootcamp questions.
- **`<session>.full.md` (reference)** — verbatim ads registry, verbatim slides registry, full speaker-tagged transcript with inline `[VISUAL: …]` annotations. Open only when the user wants an exact quote, a specific slide, or to cite a moment by timestamp. (Note: the lessons-only bundle does not include `.full.md` files — if one is missing, fall back to the lesson `.md`.)

## How to use this skill

1. **Always load `references/index.md` first.** It is the router and contains:
   - A 1-paragraph overview per week
   - A card per session (instructor, frameworks, distinctive content, "what to open this file for")
   - A topic index (`hooks → which sessions`, `Andromeda → which sessions`, etc.)
   - A speaker index (every instructor, guest, recurring coach)
   - A framework index (every named framework → canonical home session)
   - A "If a user asks…" routing table mapping ~35 likely questions → which file to open first

2. **Open the lesson `.md`** for the relevant session, e.g. `references/week-02/tuesday-sarah-levinger-research.md`. This handles most questions on its own.

3. **Only open `.full.md` when you need verbatim wording, exact slide content, or a timestamped citation.** Reference files are large (25–100K tokens each) — do not load them speculatively.

4. **Cross-reference across sessions.** Many lessons cite each other (e.g., Week 7 Tuesday repeatedly cites Dara's Week 3 frameworks). The `## Cross-week references` section in each lesson file lists these explicitly — follow them when a single session doesn't fully answer the question.

## Known gaps to be aware of

- **Week 5 Thursday's structured slide registry is a placeholder.** Slide content is still recoverable via the 112 inline `[VISUAL: …]` annotations in the transcript; only the deduplicated structured registry is missing.
- **Week 7 Thursday, Week 8 Tuesday, and Master's Series Weeks 9–10 are not captured** — sessions were un-recorded at extraction time or future-dated.
- **Verification notes** at the end of each lesson file document corrections made during synthesis (name spellings, transcript loop artifacts, OCR quirks). Defer to those notes when a name or claim looks off.

## What to do when uncertain

- If the user's question is bootcamp-adjacent but you can't tell which session it belongs to, read `references/index.md` and use its topic index and "If a user asks…" routing table.
- If a framework is mentioned by name (e.g., "T-E-E-P", "Three Realities"), the framework index in `references/index.md` names the canonical home session.
- If a speaker is mentioned, the speaker index in `references/index.md` lists every session they appeared in.
- If the user wants a verbatim quote and the lesson file doesn't have it, open the matching `.full.md` (if present in this bundle) and search the transcript.
