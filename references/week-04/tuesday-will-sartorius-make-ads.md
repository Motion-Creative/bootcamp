---
slug: week-04-tuesday-will-sartorius-make-ads
bootcamp: motion-2026-creative-strategy-bootcamp
week: 4
date: 2026-04-07
day: Tuesday
session_type: class
title: "Make Some Ads!"
instructor: "Will Sartorius"
guests: []
learning_focus: "AI-assisted ad production without sacrificing quality. Prompt iteration loops for generative control. Creating static product ads, animated GIFs, and production-ready B-roll. Balancing AI efficiency with human creative control."
homework_channel: #homework-week-4
duration_sec: 7291
primary_topics: [ai-tooling, creative-production, prompt-engineering, ad-cloning, scalable-ad-systems]
speakers:
  - name: Evan Lee
    role: Head of Partnerships
    org: Motion
  - name: Will Sartorius
    role: CEO
    org: SelfMade
processed_by: gemini-2.5-pro + claude-opus-4-7
processed_at: 2026-05-05T02:29:40.044Z
---

## Summary

Will Sartorius, CEO of SelfMade, presents a comprehensive tutorial on building an AI-assisted creative process for performance ads. He outlines two primary methods: a "quick win" approach for rapidly cloning competitor ads and animating static images, and a more advanced "scalable method" for building an iterative ad creation system using Claude Code, Fal.ai, Nano Banana 2, and Veo 3.1. The session emphasizes structured prompting, four-layer setup (brand extraction, reference cards, format templates, copywriting agents), and leveraging long, context-rich prompts to generate high-volume, on-brand ad creatives while keeping a human creative strategist in the loop.

## Chapters
- 00:00–10:34 — Pre-show waiting screen
- 10:34–13:21 — Evan Lee intro, tech difficulties recap, agenda
- 13:21–22:23 — Will Sartorius intro and overview of AI creative process
- 22:23–23:23 — Quick Win 1: Lazy Man's Approach to Cloning Ads
- 23:23–24:21 — Quick Win 2: (Not So) Lazy Man's Approach to Animating Statics
- 24:21–26:44 — The Scalable Method intro: Claude Code for iterative systems
- 26:44–27:18 — The System: Build Once, Run Every Time
- 27:18–28:41 — Layer 1: Brand Extraction
- 28:41–29:32 — Layer 2: Brand Reference Cards
- 29:32–29:55 — Layer 3: Format Templates
- 29:55–31:42 — Layer 4: Optional Copy Scoring Agents
- 31:42–33:36 — System in action: Generating on-brand statics (Hexclad)
- 33:36–37:37 — System in action: Multiplying ads across formats (Jones Road)
- 37:37–47:08 — Q&A with Will and Evan
- 47:08–51:28 — Homework brief and $5,000 contest details
- 51:28–end — Extended live Q&A

## Frameworks / models / taxonomies presented

- **Name**: Two-Method AI Creative Process
- **Definition**: A dual approach balancing immediate output with long-term scalability.
- **Structure**: Quick Win Method (clone competitor ads, animate statics) | Scalable Method (build a repeatable, on-brand system)
- **Introduced at**: ~22:12
- **Mode**: both
- **Attribution**: presenter's own

- **Name**: The System: Start to Finish
- **Definition**: Workflow split between one-time setup and repeatable execution.
- **Structure**: BUILD ONCE: (1) Brand Extraction (2) Brand Reference Cards (3) Format Templates (4) Optional Scoring Assistants. RUN EVERY TIME: (1) Pick a Format (2) Claude Writes Brief (3) Assistants Score (4) Assemble NB2 Prompt
- **Introduced at**: ~26:44
- **Mode**: visual
- **Attribution**: presenter's own

- **Name**: The Four Layers
- **Definition**: Foundational components of the scalable AI ad system.
- **Structure**: L1 Brand Extraction Prompt | L2 Brand Reference Cards (spec card + visual style card) | L3 Format Templates (recipe cards per ad type) | L4 Optional Copywriting Agents (5–7 scoring agents at 90+ threshold)
- **Introduced at**: ~27:18
- **Mode**: both
- **Attribution**: presenter's own

- **Name**: Three Tiers of Claude (Charmander → Charmeleon → Charizard)
- **Definition**: Progression of Claude tools by capability.
- **Structure**: Cowork (desktop watching, recurring tasks, native connectors) | Chat (browser/desktop interface, projects, strategy & briefs) | Code (folder-based, agentic, batch ops, production scale)
- **Introduced at**: ~29:42
- **Mode**: both
- **Attribution**: presenter's own (Pokémon analogy)

- **Name**: Two Frames Animation Concept
- **Definition**: Animate statics by generating start + end frames and letting Veo connect them, rather than asking AI to "animate this ad."
- **Introduced at**: ~23:32
- **Mode**: both
- **Attribution**: presenter's own

## Claims

- **Claim**: "Prompts, markdown files, agents, and skills are all just text files" — Will Sartorius — observation — ~26:50
- **Claim**: "The last time I read a full prompt was probably two years ago" — Will Sartorius — observation — ~27:00
- **Claim**: "Nano Banana 2 doesn't guess well — if you don't specify it, it won't do it" — Will Sartorius — observation — ~33:24
- **Claim**: "Ideal Nano Banana 2 prompt length is 1,000–1,500 words; ceiling around 2,000" — Will Sartorius — observation — ~33:24
- **Claim**: "Veo 3.1 is the only major model that requires structured JSON for precise control" — Will Sartorius — observation — ~43:17
- **Claim**: "Claude is bad at extracting proper fonts and colors from web research" — Will Sartorius — observation — ~28:41
- **Claim**: "For statics, AI is there. For videos and GIFs, we're getting there" — Will Sartorius — opinion — ~42:13
- **Claim**: "GIF CPMs are generally lower than statics, so converting winning statics to GIFs adds leverage" — Will Sartorius — observation — ~23:23
- **Claim**: "Quick-win brand reference method gets ~60–70% hit rate; scalable method with reference cards gets ~90–95%" — Will Sartorius — observation — ~52:09
- **Claim**: "Veo 4 comes out in May, which will make this presentation partially obsolete" — Will Sartorius — time-bound — ~29:30
- **Claim**: "Meta requires volume in 2026; AI is how you supplement that volume" — Will Sartorius — observation — ~54:04
- **Claim**: "You still need human-oriented content (2–4 minute ads) for top of funnel" — Will Sartorius — opinion — ~54:17
- **Claim**: "Slop is slop, whether AI or human-made" — Evan Lee (citing community member Jen) — opinion — ~51:11
- **Claim**: "Negative AI ad commenters often haven't purchased and won't — cross-reference Shopify before reacting" — Will Sartorius — observation — Q&A
- **Claim**: "AI video ads work particularly well for older demographics" — Will Sartorius — opinion — Q&A
- **Claim**: "This entire system assumes you know baseline creative strategy — persona, angle, emotion, product fit" — Will Sartorius — observation — Q&A

## Tactics recommended (do this)

- Upload competitor ad to Claude (Opus model) with a deconstruction prompt that extracts ad format, copy, product, layout, background, typography, visual devices, color palette, and spacing — then rework for your brand.
- For animation, decide whether your existing static is the start frame or end frame, then use Nano Banana 2 to generate the missing frame.
- Generate Veo 3.1 video prompts as JSON in Claude, explicitly labeling start frame vs. end frame, then run in Google Labs Flow with 9x16 aspect.
- Iterate on bad video outputs by uploading the GIF/MP4 back to Claude, describing exactly what's wrong, and asking for a corrected JSON prompt that preserves what worked.
- Use Claude Code over Claude Chat for production scale — files in your folder are read automatically without re-uploading.
- Build a "cookbook" of format templates as markdown files: headline, testimonial, before/after, statistics, features-and-callouts, UGC-style, etc.
- Collect 5–6+ examples per ad format from Facebook ad library (use ImageI Chrome plugin), upload to Claude, classify and synthesize into a markdown template.
- Spin up 5–7 copywriting agents (persona fit, angle fit, emotional fit, brand fit, conversion, format, grammar) and require each to score 90+/100 before image generation.
- Use long prompts (1,000–1,500 words) loaded with brand context, hex codes (with reference card image), font references (with reference card image), safe zones, and explicit visual rules.
- Save EVERY output (extraction, spec cards, format templates, agents) into your project folder/Claude project — repeated reminder.
- For brand fonts/colors when no brand bible exists: inspect the brand's webpage in browser, search "font" and "color," paste raw CSS into Claude, ask it to update the spec cards.
- Convert PDFs/PowerPoints to markdown before uploading to Claude — PDFs get screenshotted page by page, wasting tokens.
- Use Fal.ai over native Gemini to generate four images at once and access every model.
- Whitelist AI ads from a side Facebook page (e.g., "Irish Beer Club") rather than the main brand page to insulate the brand from negative comments.
- Take winning brief, ask Claude to "rewrite this brief for each format template in my folder" to multiply one ad into many on-brand variants.

## Anti-patterns (don't do this)

- Don't just upload reference images and hope the AI captures the aesthetic — give it structured spec + visual style cards.
- Don't try to read or hand-engineer long prompts — they're for the machine. Iterate by feeding outputs back to Claude instead.
- Don't ask AI to "animate this static ad" directly — it doesn't work. Generate frames first.
- Don't use short prompts with Nano Banana 2 — it won't fill gaps gracefully (use Nano Banana Pro if you want assumption-filling).
- Don't upload PDFs directly to Claude — convert to markdown first.
- Don't upload more than 2–3 brand reference ads — contradictions hurt output.
- Don't use Higgsfield (speaker considers it shady) — use Fal.ai instead.
- Don't use AI UGC with fake doctors / fake people (morally and reputationally problematic).
- Don't try to volume-produce slop just for volume's sake — prioritize quality even within scaled workflows.
- Don't skip the human creative strategy work — the system assumes persona/angle/emotion are already decided.
- Don't forget to save extraction outputs, cards, templates, and agents — multiple "Stop. Save it." reminders throughout.

## Data / stats cited

- "$14 billion in media spend analyzed every year by Motion's customers" — Evan Lee, ~14:39, slide
- "~8 cents per generation in Fal.ai" — Will Sartorius, ~30:56, verbal
- "Past ~2,000 words the model loses focus" — Will Sartorius, ~33:24, slide/verbal
- "I have like 20 copywriting agents now" — Will Sartorius, ~41:00, verbal
- "Quick-win method ~60–70% on-brand hit rate; scalable method ~90–95%" — Will Sartorius, ~52:09 in scalable section, verbal
- "$5,000 grand prize + $500 random draw for Week 4 homework" — Evan Lee, ~38:16
- Last week's swag winners: Wasan (Wes) Al Roubaie, Taylor Durkin, Payton Brooks — Evan Lee
- Question upvote count visible: Ashley Humphreys' question got 39 upvotes

## Named entities

### People mentioned (excluding speakers)
- **Sarah Levinger** — Foundations instructor (Week 2) — referenced for research/persona work
- **Dara Denney** — Foundations instructor (Week 3) — referenced for prioritization/angle work
- **Bill Rom** — Masters instructor — slide reference
- **Oren John** — Masters instructor — slide reference
- **Alysha Bains, John Abrams, Sarah Bunnell, Joanna Wallace, Naomi-Pei Ganger** — Group coaching coaches
- **Naomi (Space Goods)** — referenced for Miro creative retro presentation in prior coaching call
- **Harry Demage / Delmage** — referenced re: Foxwell presentation in Lisbon, human-centric ads
- **Jen** — community member, "slop is slop" comment
- **Jerry, Lance, Ashley Humphreys, Bria Mirante, Derek Daniels, Georgie, Murad, Sam Khan, Annie, Kim, Maya, Emma, Ali, Jay, Ellen, Alex, Candace, Silas, Christina, Patrick, Raphael, Brad, Cynthia, Makaya, Jess, Melissa, Marley, Alia, Vishnu, Kyle, Jason** — community attendees mentioned/cited in chat
- **Mr. Abbott** — Will's sixth-grade physics teacher (anecdote: "when in doubt, overcommunicate")

### Brands / companies referenced
- SelfMade, Skipper (getskipper.ai), Jones Road, HexClad, Ridge, True Classic, Vuori, Ilia, Wpromote, ClickUp, BYLT, AG1, PrettyLitter, Earth Breeze, Grüns, Obvi, MuteSix, Liquid Death, Lucky Charms (analogy), Medby (cautionary), Foxwell (event), Space Goods

### Tools / products referenced (excluding Motion)
- Claude (Cowork, Chat, Code) — Anthropic
- Claude Opus model (specifically Opus 4.6 mentioned as best)
- Codex (OpenAI) — briefly mentioned as comparable
- Fal.ai — multi-model platform
- Higgsfield — flagged as shady, not recommended
- Nano Banana 2 (and Nano Banana Pro predecessor) — Google image gen
- Veo 3.1 (Veo 4 forthcoming) — Google video gen
- Gemini chat — alternative interface
- Google Labs / Flow — Veo interface
- Kling — video model (text prompts)
- Seedance — new model on Fal.ai (early access)
- Canva — alternate execution path
- Image Downloader (Chrome plugin) — for Facebook ad library scraping
- Facebook Ad Library
- Shopify — for cross-referencing commenters
- Asana, Slack, Gmail — Claude Cowork connectors

### External frameworks / concepts cited
- JSON prompts
- Markdown (.md) files
- VBA macros (analogy for Cowork)
- HTML inspect / CSS scraping for fonts and colors
- "Skills" (Anthropic terminology)
- Andromeda (Meta's ad system, referenced re: volume requirements)

## Motion product shown

- **Feature**: Motion content library + product UI overview
  - **What was shown**: Creative Benchmarks 2026, Becoming a Creative Strategist guide, Creative Strategy Summit 2025 branding, dashboard analytics
  - **Timestamp**: ~14:01
- **Feature**: Customer logos / spend stat
  - **What was shown**: $14B media spend stat with brand logos
  - **Timestamp**: ~14:39
- **Feature**: Slack community screenshots
  - **What was shown**: Active conversations and creative sharing in bootcamp Slack
  - **Timestamp**: ~14:50
- **Feature**: Motion Creative Gallery
  - **What was shown**: Grid of ad creatives during homework walkthrough
  - **Timestamp**: ~48:14
- **Feature**: 60-day trial offer
  - **What was shown**: Trial claim slide
  - **Timestamp**: ~16:00
- **Feature**: Brand Intel (referenced)
  - **What was shown**: Brand-level breakdown during homework walkthrough
  - **Timestamp**: ~48:26

## Key quotes

- "I'm not a designer. I'm innately lazy. So I have tried to come up with a system that requires the least amount of work for the most amount of output." — Will Sartorius
- "People love to overcomplicate this to make themselves seem smarter than they are. Prompts, markdown files, agents, skills — these are all just text files." — Will Sartorius
- "The last time I read a full prompt was probably two years ago." — Will Sartorius
- "Stop reading prompts. Stop trying to over-engineer your prompts. It will drive you crazy and it doesn't work." — Will Sartorius
- "When in doubt, over-communicate. Something my sixth-grade physics teacher used to say." — Will Sartorius
- "You're not asking AI to animate your ad. You're creating two frames and letting AI connect them." — Will Sartorius
- "The spec card tells Nano Banana what your brand looks like. The style card tells it how your brand feels." — Will Sartorius
- "You are in control of what this model is doing. It is just helping you get from point A to point Z." — Will Sartorius
- "If I showed you any of the statics I created, would you know they were AI-generated? Probably not." — Will Sartorius
- "These people were never going to purchase in the first place. They are just there to troll, and that ad — it's printing." — Will Sartorius
- "You need volume. You also really need to have human elements, human ads. No ad account is going to take off with just statics and GIFs." — Will Sartorius
- "This entire presentation assumes that you know baseline creative strategy. I just gave you the system after you've done all of your creative strategy and how to execute." — Will Sartorius
- "Slop is slop, whether AI-made or human-made." — Evan Lee (citing Jen)
- "This is the difference between a wannabe and a doer." — Evan Lee (citing Lance)
- "We fly high, no lie, you know this. Ballin'." — Evan Lee
- "Welcome, welcome, one of us, one of us." — Evan Lee
- "Motion has a lot of tech issues for a tech company… I will own it when you are in Motion. But when it's this, I will not own it." — Evan Lee
- "Charmander, Charmeleon, Charizard." — Will Sartorius (Claude tier analogy)

## Time-bound claims

- "Veo 4 comes out in May. This presentation will be obsolete at that point." — Will Sartorius, ~29:30 / restated near video section
- "As of now, Claude is by far the frontier model." — Will Sartorius, ~26:01
- "Opus 4.6 is going to give you the best results." — Will Sartorius, Q&A re: cheap stack
- "Claude's been down today, so I'm not going to risk a live demo." — Will Sartorius, end of presentation
- Homework deadline: April 17 — Evan Lee
- Bootcamp date context: Week 4 of 2026 cohort (Foundations stage)

## Homework / assignments mentioned

- **Assignment**: Make an AI-generated ad using one of three workflows from the class:
  1. Easy — Clone a competitor ad
  2. Harder — Animate a static into a GIF (start/end frames + Veo)
  3. Hardest — Multiply one ad concept across multiple formats using the scalable system
  - Use one of the partner brands (Jones Road, HexClad, Ridge), a brand from prior weeks' homework, a brand explored in Motion, or your own brand.
- **Channel / where to post**: #homework-week-4 in Slack
- **Additional requirement for contest**: Create a social media post about the ad and tag Motion
- **Deadline**: April 17 (submit-by deadline; speed not rewarded — quality is)
- **Prizes**:
  - Grand prize: $5,000 USD for the best ad (judged by panel using Will's criteria)
  - Random draw: $500 USD for one homework submitter
  - Ongoing weekly swag for social posts tagging Motion
- **Submission encouraged**: Both the creative output AND the workflow/process behind it
- **Timestamp**: ~47:08–48:30

## Cross-week references

- **Reference**: Persona, angle, emotion as prerequisites for the AI system
  - **Pointing to**: Sarah Levinger (Week 2) and Dara Denney (Week 3)
  - **Timestamp**: ~31:30, ~59:08
- **Reference**: "Be real about your volume" — capacity over aspiration
  - **Pointing to**: Dara and Sarah's prior sessions
  - **Timestamp**: Q&A on creative team division
- **Reference**: Naomi (Space Goods) Miro board on creative retros
  - **Pointing to**: Prior Thursday group coaching call
  - **Timestamp**: ~16:00
- **Reference**: Foundations → Sprints → Masters arc; "You are here" in Foundations Week 4
  - **Pointing to**: Curriculum overview slides
  - **Timestamp**: ~14:50–15:30
- **Reference**: Last week's swag winners (Wasan, Taylor, Payton)
  - **Pointing to**: Week 3 social tagging
  - **Timestamp**: ~16:30

## Verification notes

- Date corrected from structured (no date provided) to canonical 2026-04-07 (Week 4 Tuesday).
- Title corrected from structured implicit ("Building Your AI Creative Process") to canonical syllabus title "Make Some Ads!" — the in-deck title slide reads "Building Your AI Creative Process" but the bootcamp curriculum title is "Make Some Ads!"; preserved canonical.
- Speakers list verified: Will Sartorius (instructor) + Evan Lee (host/Head of Partnerships, Motion). No additional guests despite Q&A format. Marked guests: [].
- Duration 7291 sec (~2h 1m 31s) consistent with 5–7 PM UTC scheduled window.
- Slide #5 in extraction had a corrupted/repeated logo list (MuteSix loop) — disregarded the spam, used the clean logo list from the visible slide.
- The transcript field in the extraction is heavily duplicated/looped in the post-Q&A section (Evan's extended Q&A repeats verbatim many times) and ends with garbled Lightshot filename strings — flagged as transcription artifact, not session content. The actual session ended cleanly after Will's farewell and Evan's homework walkthrough; ignored the looped/garbled tail when extracting metadata.
- Brand name "Medby" / "Med-B" referenced as cautionary example (fake-doctor ads) — kept as-is, low confidence on exact spelling.
- "Harry Demage" likely "Harry Dry" or another spelling — Will explicitly said "probably butchering his last name." Left as transcribed.
- "Andromeda" referenced once (Meta's system requiring volume) — consistent with curriculum context.
- Hex code / font extraction tactic via browser Inspect verified across slide and verbal.
- Three-tier Claude framework (Cowork/Chat/Code) verified via slide and verbal explanation.
- Quote attribution for "slop is slop" corrected: spoken by Evan Lee citing community member Jen in Slack, not Evan's original.
- Otherwise all four extraction sources (transcript, slides, ads, structured) are consistent on the substantive content. Corrections applied: title, date, deduplication of looped transcript content, cleanup of spam logo list.

---

📂 **Full transcript, slides registry, and ads registry** — see `tuesday-will-sartorius-make-ads.full.md`
