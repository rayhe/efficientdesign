# STORY_GUIDE.md — Efficient Design

## Voice
Engineering appreciation for enthusiasts who care about *how* things work, not just what they cost. Watches and cars — the intersection of mechanical ingenuity and aesthetic discipline. Write for someone who'd spend 20 minutes explaining why a flat-plane crankshaft sounds different.

## Anti-AI Voice Rules
- **Banned phrases:** "Here's the thing," "Here's where it gets interesting," "The kicker:," "Let's be clear," "Make no mistake," "And it's not even close," "The numbers don't lie," "X isn't about Y. It's about Z."
- **Vary sentence lengths** — fragments, one-liners, then longer builds
- **Have actual opinions** — "The Tudor Black Bay is overrated for what you get at $4,200" not "the market continues to evolve"
- **Start mid-thought** — no throat-clearing setup paragraphs

## Scholarly Rigor
- Every claim needs a source. Cite the movement reference, the horological study, the dyno chart.
- Original contribution required — don't just summarize press releases.
- State limitations. If you haven't handled the watch or driven the car, say so.

## Sentence Rhythm Gate (Required — HARD GATE)

**Why this exists:** AIPM community research found that AI-generated articles have a telltale sentence length clustering pattern. Human writing has wildly varied sentence lengths (variance ~287); AI writing clusters around the mean (variance ~84). Human writers use ~9-10% short sentences; AI uses 36%. Human writers build 23% long complex sentences; AI manages only 2%. This gate catches that fingerprint.

This is related to the broader stylometric problem: function word cosine similarity across AI personas is 0.9563 vs 0.9208 for real journalists. LLMs cluster around structural means regardless of persona prompting. Sentence rhythm is a cleaner, more actionable dimension of the same defect.

### Targets
- **Sentence length variance:** ≥ 200 (human ~287, AI ~84)
- **Short sentences (<8 words):** ≤ 15% of total (human ~9-10%, AI ~36%)
- **Long complex sentences (>20 words):** ≥ 15% of total (human ~23%, AI ~2%)

### How to check
Run the sentence rhythm script before publishing:
```bash
python3 ~/workspace/scripts/sentence-rhythm-check.py <article.html|article.md> --histogram
```
For JSON output (pipeline integration): add `--json`
For per-sentence detail: add `--sentences`

Exit code 0 = PASS, 1 = FAIL. The script gives specific rewrite suggestions on failure.

### What failing looks like
An article that reads like a metronome — every sentence is 12-18 words, no punchy fragments, no sprawling complex constructions. The rhythm is flat. A human reader won't consciously notice, but they'll feel it: the writing is boring and they can't say why.

### How to fix it
1. **Add short punches.** "That's insane." / "It worked." / "Nobody noticed." — 3-5 word sentences that land like a slap.
2. **Build long constructions.** Sentences that unfold through subclauses, layered arguments, or lists — the kind where the reader is committed before they realize how far the sentence is going to take them, and by the time they reach the period they've absorbed three ideas without stopping.
3. **Break patterns.** If three paragraphs in a row have the same sentence-length rhythm, rewrite one. Monotony is the enemy.
4. **Read it aloud.** Varied rhythm sounds like someone talking. Uniform rhythm sounds like a textbook.

### For the critic pipeline
Add "Sentence Rhythm" as a dimension in the Voice Coach critic. The Voice Coach should:
- Run `sentence-rhythm-check.py --json` on the draft
- Report the three metrics and pass/fail status
- If FAIL, include the script's rewrite suggestions verbatim
- Weight this as a blocking gate — an article that fails rhythm review should not ship
