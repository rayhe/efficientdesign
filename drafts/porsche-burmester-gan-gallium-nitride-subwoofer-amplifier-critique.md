# Critique — Article #181: "Wide Bandgap, Deep Bass: Porsche's Gallium Nitride Subwoofer Amplifier"
Slug: porsche-burmester-gan-gallium-nitride-subwoofer-amplifier.html · Author: Elena Voss · Cars
Date: 2026-09-06 · Overall: **8.93/10** (threshold 8.5, PASS)

## Hard gates (scripts are truth)
- Em dashes: 0 (grep count, limit 3) — PASS
- "The" sentence starters: 8/69 = 11.6% (limit 15%) — PASS
- Banned phrases: none found — PASS
- Sentence rhythm (sentence-rhythm-check.py --json): variance 325.9 (>=200), short 4.3% (<=15%), long 62.3% (>=15%) — PASS

## 1. Voice Coach — 9.0/10
Opens mid-thought on the August 21 announcement, no throat-clearing. Sentence lengths genuinely varied (4-word punches to 30+ word builds, histogram spread across all bins). Real opinions present: "Nobody is going to buy a Porsche because of the transistors in its stereo, and that is precisely why this is worth writing about." No banned phrases. Minor: one "corporate-speak" aside is slightly glib but on-voice.

## 2. Technical Accuracy — 9.0/10
All Porsche claims verified against the primary source (Porsche Newsroom 21/08/2026): world-first production-ready claim, 400W subwoofer amplifier voltage conversion, ~20% lighter aluminum heat sink, smaller passives, 2027 production, University of Stuttgart Institute for Robust Power Semiconductor Systems, mid-2023 idea / spring-2024 team, "Driven by GaN", unnamed chip manufacturer + audio partner, patent applications, Heuken and Burosch quotes, blue-LED 1990s lineage. Background facts (GaN 3.4 eV vs Si 1.1 eV; Nobel 2014 for blue-LED GaN work; GaN-vs-SiC roles in power electronics) are standard, non-controversial power-electronics knowledge. Burmester system figures (21 speakers/channels, ~1,455W) corroborated by audioxpress. EMC tradeoff of fast GaN switching framed as an open question, not asserted. No claim invented.

## 3. Original Contribution — 8.75/10
Goes well beyond the press release: (a) engineering triage argument that bass is the heaviest load so it gets the best silicon, (b) audio as a low-risk proving ground for traction-inverter GaN, (c) GaN-vs-SiC strategic framing against the blog's earlier SiC inverter piece, (d) the EMC question and the listening-vs-weight question. The "materials colonize a car from the edges inward" closer is an original synthesis. Not a summary.

## 4. Structure — 9.0/10
Matches the #177 reference format: H1, subtitle, byline, hero figure, six H2 sections in a logical arc (announcement → material physics → why-this-subsystem → development history → strategic play → unknowns), spec table, sources paragraph. Spec table is factual and sourced. No section bloat.

## 5. Reader Value — 8.75/10
An enthusiast learns real physics (bandgap → switching losses → heat sink mass), a genuine industry strategy (audio as GaN beachhead toward high-voltage systems), and what remains unknown. Practical value: knowing what to watch for when the 2027 models land. Could be stronger with a named model, but Porsche hasn't named one, so this is a source limitation, not a writing one.

## 6. Scholarly Rigor — 9.0/10
Final paragraph explicitly separates sourced facts (Porsche newsroom, The Drive, audioxpress, StereoNET) from background knowledge (bandgap figures, GaN history) from original analysis (proving-ground thesis, marked as "my own analysis, not Porsche's claim"). Limitations stated: no listening session possible, no vehicle named, no gram figure published, author hasn't heard it. Every checkable number is attributed.

## 7. Line Editor — 9.0/10
Clean copy. Varied cadence reads aloud naturally. No filler transitions, no repeated constructions. Two long sentences could be trimmed but they carry multiple ideas by design. Punctuation and hyphenation consistent ("subwoofer", "wide-bandgap", "high-voltage" as compounds).

## Verdict
**SHIP.** 8.93/10, all critics above 8.5, all hard gates pass. No revision round required.
