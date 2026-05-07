# Motion 2026 Creative Strategy Bootcamp — Corpus

Markdown library extracted from the **Motion 2026 Creative Strategy Bootcamp** (recorded weekly Tuesday classes + Thursday group coaching, ~13K-person Slack community). Designed to drop into Claude, Cursor, Runneth, or any agent that reads markdown — so it can answer questions about the course material.

## Coverage

13 sessions across **weeks 1–7** of the 8-week curriculum:
- 7 Tuesday classes (single-instructor or guest-panel deep dives, slide-driven)
- 6 Thursday group coaching calls (live student work review + tactic walkthroughs)

Not yet captured (sessions either un-recorded at extraction time or future-dated): Week 7 Thursday, Week 8 Tuesday (Sprint #3 capstone), Master's Series Weeks 9–10.

## Shape

```
bootcamp/
├── index.md              ← cheat sheet — load this first
├── week-01/
│   ├── tuesday-evan-what-is-creative-strategy.md       ← lesson (~5–7K tokens)
│   ├── tuesday-evan-what-is-creative-strategy.full.md  ← reference (~25–100K tokens)
│   ├── thursday-coaching-hook-writing.md
│   └── thursday-coaching-hook-writing.full.md
├── week-02/  …  week-07/
```

Every session has two files:

| File | Contains | Open when |
|---|---|---|
| `<session>.md` (lesson) | Frontmatter, summary, chapters, **frameworks** with full taxonomies, claims, tactics, anti-patterns, named entities (people / brands / tools), key quotes, time-bound claims, homework, cross-week refs. Coaching sessions also include student questions answered, ads critiqued live, live worked examples. | **By default.** Answers ~80% of questions about a session. |
| `<session>.full.md` (reference) | Frontmatter (copy) + verbatim ad-facts registry (every ad shown, with brand / format / hook / on-screen text / speaker framing) + verbatim slide-facts registry (every distinct slide with title / layout / body / charts / annotations / reveal states / speaker framing) + full speaker-tagged transcript with inline `[VISUAL: …]` annotations. | When you need a verbatim quote, an exact slide, or to cite a specific moment by timestamp. |

Total corpus: ~330 KB (~80K tokens) for the lesson layer; per-session reference files run 25–100K tokens each.

## How an agent should use this

1. **Always load `index.md` first.** It contains:
   - A 1-paragraph overview per week
   - A card per session (instructor, frameworks introduced, distinctive content, "what to open this file for")
   - A topic index (`hooks → which sessions`, `Andromeda → which sessions`, etc.)
   - A speaker index (every instructor, guest, and recurring coach)
   - A framework index (every named framework → canonical home session)
   - A "If a user asks…" routing table (~35 likely Slack questions → which file to open first)

2. **Open the lesson `.md` for the relevant session.** That handles most questions.

3. **Only open `.full.md` when you need verbatim wording, exact slide content, or to cite a specific moment.** Reference files are large; don't load them speculatively.

4. **Cross-reference** — many sessions reference each other (e.g., Week 7 Tuesday repeatedly cites Dara's Week 3 frameworks). The `## Cross-week references` section in each lesson file lists these explicitly.

## Notable known gaps

- **Week 5 Thursday's structured slide registry is a placeholder.** The transcript captures slide content via 112 inline `[VISUAL: …]` annotations, but the dedicated slide registry pass exhausted retries. Slide *content* is recoverable via the transcript; only the deduplicated structured registry format is missing.
- **Verification notes** appear at the end of each lesson file documenting any corrections made during synthesis (name spellings, transcript loop artifacts, OCR quirks).

## Provenance

- Videos: original Drive recordings, pre-encoded to 720p / 1.5 Mbps for upload.
- Extraction stack: Gemini 2.5 Pro for 4 parallel passes (verbatim transcript / slide registry / ad registry / structured metadata) at `MEDIA_RESOLUTION_LOW` to fit ~2.5h videos under the 1M-token input cap; Claude Opus 4.7 for verification + metadata synthesis using sampled key frames.
