# Motion Creative Strategy Bootcamp — as a Claude skill

> 13K marketers just finished our 7-week creative strategy bootcamp.
> Now your agent can take it too.

The complete bootcamp — every Tuesday class, every Thursday coaching call — extracted into structured markdown and packaged as a Claude skill. Once installed, ask Claude anything about the course and it will pull the right session for you automatically.

**Scope:** 13 sessions × 2 files each (structured lesson + verbatim reference). ~80K tokens of lessons + 25–100K tokens per reference file. Every framework, claim, tactic, anti-pattern, key quote, ad shown, and slide — extracted, indexed, and cross-referenced.

## Install

### claude.ai (web / desktop app)

1. Go to the [latest release](https://github.com/Motion-Creative/bootcamp/releases/latest) and download **`motion-bootcamp.skill`** (lessons only, ~80K tokens, recommended) or **`motion-bootcamp-full.skill`** (lessons + full verbatim transcripts, much larger).
2. In claude.ai, go to **Settings → Capabilities → Skills** and upload the `.skill` file.

Done. Ask Claude anything bootcamp-related and the skill activates automatically.

### Claude Code (terminal)

**Paste this into Claude Code:**

> Install this as a skill: `https://github.com/Motion-Creative/bootcamp`

Or do it directly:

```bash
git clone https://github.com/Motion-Creative/bootcamp.git ~/.claude/skills/motion-bootcamp
```

### Other agents (Cursor, Runneth, anything markdown-aware)

Clone anywhere and point your agent at the folder. `references/index.md` is the router.

```bash
git clone https://github.com/Motion-Creative/bootcamp.git
```

## How to use

No special commands. Once installed, just ask:

> "What did Sarah Levinger say about micro-moments?"
> "Explain T-E-E-P with an example."
> "What's the hook analytics funnel?"
> "Walk me through Eric's Flowell turnaround."
> "Give me a verbatim quote from Week 3 Tuesday about Andromeda."

The skill activates automatically when your question matches bootcamp content. Claude reads `index.md` first to find the right session, then opens that session's lesson file, and only cracks the full transcript when you ask for an exact quote.

## What's inside

```
bootcamp/
├── SKILL.md                  ← skill manifest (read by Claude)
├── README.md
└── references/
    ├── index.md              ← cheat sheet — Claude loads this first
    ├── week-01/
    │   ├── tuesday-evan-what-is-creative-strategy.md       ← lesson (~5–7K tokens)
    │   ├── tuesday-evan-what-is-creative-strategy.full.md  ← reference (~25–100K tokens)
    │   ├── thursday-coaching-hook-writing.md
    │   └── thursday-coaching-hook-writing.full.md
    └── week-02/  …  week-07/
```

Every session has two files:

| File | Contains | When Claude opens it |
|---|---|---|
| `<session>.md` (lesson) | Frontmatter, summary, chapters, **frameworks** with full taxonomies, claims, tactics, anti-patterns, named entities (people / brands / tools), key quotes, time-bound claims, homework, cross-week refs. Coaching sessions also include student questions answered, ads critiqued live, live worked examples. | **By default.** Answers ~80% of questions about a session. |
| `<session>.full.md` (reference) | Frontmatter (copy) + verbatim ad-facts registry (every ad shown, with brand / format / hook / on-screen text / speaker framing) + verbatim slide-facts registry (every distinct slide with title / layout / body / charts / annotations / reveal states / speaker framing) + full speaker-tagged transcript with inline `[VISUAL: …]` annotations. | When you need a verbatim quote, an exact slide, or to cite a specific moment by timestamp. |

Total corpus: ~330 KB (~80K tokens) for the lesson layer; per-session reference files run 25–100K tokens each.

## Speakers

Sarah Levinger (Tether Insights), Dara Denney (Point Guard Media), Will Sartorius (SelfMade), Jade Heritage (Calm), Daniel Rivera (Harry's), Sophia Beauvoir (Ready Set), Viti Videtta (Happy Mammoth), Janae LeVander (Caraway), Jake Abrams (Odyssey), Joanna Wallace (Creativly), Eric Philippou (Laughing Heart Media), Sarah Burnett, Matteo Friend, Darcy Tennant (Heights), Blaise Ormond (MTRX Media), Naomi Peh Haeger (Spacegoods), and the Motion team.

## Coverage

13 sessions across **weeks 1–7** of the 8-week curriculum:
- 7 Tuesday classes (single-instructor or guest-panel deep dives, slide-driven)
- 6 Thursday group coaching calls (live student work review + tactic walkthroughs)

Not yet captured (sessions either un-recorded at extraction time or future-dated): Week 7 Thursday, Week 8 Tuesday (Sprint #3 capstone), Master's Series Weeks 9–10.

## Notable known gaps

- **Week 5 Thursday's structured slide registry is a placeholder.** The transcript captures slide content via 112 inline `[VISUAL: …]` annotations, but the dedicated slide registry pass exhausted retries. Slide *content* is recoverable via the transcript; only the deduplicated structured registry format is missing.
- **Verification notes** appear at the end of each lesson file documenting any corrections made during synthesis (name spellings, transcript loop artifacts, OCR quirks).

## Provenance

- Videos: original Drive recordings, pre-encoded to 720p / 1.5 Mbps for upload.
- Extraction stack: Gemini 2.5 Pro for 4 parallel passes (verbatim transcript / slide registry / ad registry / structured metadata) at `MEDIA_RESOLUTION_LOW` to fit ~2.5h videos under the 1M-token input cap; Claude Opus 4.7 for verification + metadata synthesis using sampled key frames.

## License

No formal license. Bootcamp recordings, slides, and frameworks belong to their respective speakers (Motion team + guest instructors). Transcripts and structured extraction are published here for fair-use reading and personal/agent consumption — drop them into your tools, learn from them, share what you've learned. For redistribution or commercial use of speaker content, please reach out.
