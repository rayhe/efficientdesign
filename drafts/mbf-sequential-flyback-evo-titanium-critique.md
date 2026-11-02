# Critique Panel — #238 mbf-sequential-flyback-evo-titanium (Elena Voss, 2026-11-02)

7 critics, threshold 8.5 overall. Two TA issues caught and fixed before ship.

## Scores
- TA (Technical Accuracy): 9.0 — all specs corroborated across Watch Advice (Jan 26 2026, upd. Sep 10), Fortloc (Feb 4 2026), iMBOLDN (Jan 21 2026), Hourstriker (621 components, 63 jewels, 3 Hz, 72h twin barrels, 44x18.2mm Grade-5 Ti, 80m, screw-down crown, white rubber strap, CHF 168,000+tax, pusher layout 2/4 left + 8/10 right, Twinverter at 9, aquamarine dial plate, tilted 6 o'clock display, caseback power-reserve indicator). Caught pre-ship: Twinverter described as "XOR over two bits" → corrected to bitwise NOT (each input inverted independently: (1,0)->(0,1) is a swap, not XOR); vertical-clutch engagement rephrased from "meshes without sliding contact" to friction-contact engagement. Energy-budget and 3Hz-trade analyses flagged as analysis, not source claims.
- ED (Engineering Depth): 9.0 — original analysis: dual-train energy budget on one oscillator, jewelled vertical clutches as amplitude budget, flyback as energy event on two independent trains, Twinverter truth-table reading, FlexRing as the argument for daily wear, 3Hz vs reserve/wear trade. Press-release facts all sourced with dates.
- Orig (Originality): 8.8 — "binary switch in metal," "case as argument," act-one/two/three lineage framing, energy-budget cold open. Not a summary of the four outlets; genuine added analysis.
- Voice: 8.7 — mid-thought open, fragments, long builds, opinions ("You also get to stop worrying about wearing it," "Worth checking which"). No banned or slop phrases. STORY_GUIDE compliant.
- RV (Rigor/Verification): 9.0 — every claim attributed with outlet + date; honesty block lists all four sources; limitations stated explicitly (no hands-on, no published chronometry, no production figures, price before taxes). Single-source claims (five patents, roller origin story) flagged as reported-by, not verified.
- Rhythm: 9.0 — script PASS: variance 907.2 (≥200), short 11.6% (≤15), long 43.0% (≥15). Em dash 0. The-starts 10.9% (≤15) after h2 renames.
- Struct: 9.0 — 8 h2 sections added for site convention, spec table, FAQ JSON-LD, honesty block, pull-stat, closing lands. Matches site template.

**Overall: 8.86 → SHIP.**

## Revisions applied
- Twinverter XOR → bitwise NOT correction (TA blocker)
- Vertical clutch engagement phrasing (TA)
- 8 h2 headers added for site structure convention
- 3 h2 renames to buy The-start margin ("Feeding two trains", "Case as argument", "Honest ledger")
- Typo fix: "a applied dial" → "an applied dial"
