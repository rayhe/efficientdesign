# Critique: 3D-Printed Metallic Glass for EV Motor Cores

## Article Under Review
**Title:** No Crystal Lattice, No Problem: 3D-Printed Metallic Glass for EV Motor Cores
**Writer:** Elena Voss
**Word Count:** ~3,400
**Category:** Cars × Materials Engineering

---

## Critic 1: Technical Accuracy (Dr. Miriam Ostfeld, Materials Science)
**Score: 8.5/10**

The core physics of domain reorientation, hysteresis loss, and eddy current loss is explained accurately and at the right level of detail for a general technical audience. The distinction between crystalline and amorphous structures is well drawn, and the explanation of why rapid cooling preserves the amorphous state is correct.

Verified claims:
- ✅ Metglas 2605SA1 saturation flux density 1.56T: confirmed against Metglas official documentation and Proterial datasheets.
- ✅ AM2SoftMag project: €3.5M, 2022–Feb 2026, Horizon Europe Pathfinder Open, grant GA 101046870. Confirmed via brightsurf.com, chargedevs.com, IMDEA Materials, and metal-am.com.
- ✅ Ralf Busch, Matthias Nienhaus, Saarland University: confirmed.
- ✅ Heraeus AMLOY Technologies (Karlstein am Main): confirmed as industrial 3D-printing partner.
- ✅ Partners in Spain (IMDEA), Italy (INRIM), Poland (AMAZEMET): confirmed.
- ✅ Three alloys identified, five-dimensional compositional space: confirmed. Busch quotes reproduced verbatim from Saarland University press materials.
- ✅ LPBF layer thickness ~50 μm: confirmed across multiple sources (chargedevs.com, interestingengineering.com, voxelmatters.com).
- ✅ Iron content 70–80%: confirmed (chargedevs.com, archynewsy.com).
- ✅ Core losses in amorphous alloys ~1/10th of silicon steel: confirmed by FeSiB motor simulation study (MDPI, 2025, showing 1/10 to 1/14 ratio) and the M19 vs amorphous FEM study.
- ✅ UNIST research, iron loss ~25% of total motor loss: confirmed from TechXplore coverage of UNIST publication in Journal of Materials Science & Technology. Note: other studies cite ~30%; article correctly attributes the 25% figure to UNIST specifically.
- ✅ Melt spinning, ribbon ~25 μm: confirmed from Metglas datasheets (23–25 μm).

Issues found:
- ⚠️ "Hitachi Metals commercialized this process as Metglas in the 1970s": Incorrect attribution. Allied Chemical Corporation (later AlliedSignal, then Honeywell) developed and commercialized Metglas in the 1970s. Hitachi Metals acquired the Metglas business from Honeywell in 2003. The material was commercially available in the 1970s, but the company was not Hitachi Metals at that time.
- ⚠️ Transformer core loss reduction "70 to 80 percent": Metglas's own brochure states losses are "about one-third" of conventional silicon steel (M3 grade), which is a ~65–67% reduction. The 70–80% figure may apply against lower-grade conventional steels but overstates the case against the comparison Metglas itself makes.
- ⚠️ M19 saturation "2.2 tesla": On the high end. M19 non-oriented silicon steel typically saturates around 1.95–2.05T at standard test conditions. 2.2T is more representative of low-silicon or pure iron compositions. The article's stated contrast (1.56T vs 2.2T) slightly exaggerates the gap.
- ⚠️ Simizu et al. 2018, 3W vs 90W: Could not independently locate this specific paper or data point. The 30:1 ratio is extreme compared to the 1/10 to 1/14 ratios documented in the 2025 FeSiB motor study and the 4–5x ratios at lower frequencies (800 Hz) in the MDPI high-speed PMSM study. At very high speeds/frequencies the ratio does increase dramatically, so 30:1 is not impossible, but the specific citation could not be verified.
- ⚠️ ANSYS Motor-CAD simulation (62% core loss reduction, 85.46% vs 80.71%, 17°C): Could not locate this exact study or application note. The numbers are internally consistent and align with the range documented in peer-reviewed literature (61–72% reduction, 3–5% efficiency gain), but the source is unverified.

Deduction: 0.5 for the Hitachi Metals/Allied Chemical misattribution (factual error on a named company), 0.5 for the transformer loss reduction overstatement, 0.5 for M19 saturation figure being high-end generous.

## Critic 2: Narrative Structure (Prof. Akira Taniguchi, Technical Narrative)
**Score: 9.0/10**

Excellent structural logic. The article follows a clean arc: problem (iron loss in motors) → fundamental physics (why it happens) → the material that solves it (amorphous metals) → the manufacturing barrier (can't shape them) → the breakthrough (LPBF) → what it means for EVs → the trade-off (saturation) → what still has to happen (scale). Each section depends on the one before it, and no section is superfluous.

The transition from "What Metallic Glass Actually Is" to "The Saarland Breakthrough" is particularly well handled, closing with "for four decades nobody could solve one without sacrificing the other" and then immediately delivering the solution. The reader is never in doubt about where the argument is going or why.

The "What This Changes for EV Motors" section correctly translates the materials science into driver-relevant terms (additional miles, thermal derating headroom) without losing technical credibility. The closing section on production readiness is honest and avoids the breathless tone that typically infects "breakthrough" articles.

Minor structural issue: the Simizu et al. and ANSYS Motor-CAD data points appear in the "What Metallic Glass Actually Is" section, which is about the material itself, not about motor simulations. They would sit more naturally in "What This Changes for EV Motors" or a dedicated evidence section.

Deduction: 0.5 for the simulation data placement, 0.5 for the "What Still Has to Happen" section running slightly long relative to its content density (three constraints could be tighter).

## Critic 3: Writing Quality (Sandra Kwan, Editorial)
**Score: 9.0/10**

Strong, confident prose throughout. The voice is authoritative without being academic, and the article earns its length by explaining physics in terms a motivated reader can follow without dumbing it down. "Billions of microscopic compass needles, snapping to point the other way, over and over" is effective sensory writing for an abstract concept.

The article avoids every banned AI slop phrase. No "Here's the thing," no "paradigm shift," no "game-changer," no "deep dive," no "unpack." Zero em dashes in the body text (1 &mdash; in the HTML title element, which is standard). "The"-initial sentences at 12.3%, comfortably under the 15% ceiling.

Sentence rhythm has genuine variation: punchy short constructions ("The physics is elegant. The manufacturing problem was brutal.") alongside complex multi-clause sentences that earn their length. The closing paragraph is strong, converting a technical paper into a single forward-looking statement without overselling.

Minor issues: "You can optimize the lattice indefinitely without eliminating its resistance. Or you can eliminate the lattice itself." is the article's strongest rhetorical turn but it arrives mid-section rather than as a section closer, slightly undercutting its impact. A few sentences in the LPBF explanation section stack subordinate clauses in similar patterns. The parenthetical "(properly called Weiss domains)" reads slightly like a textbook aside in an otherwise conversational piece.

Deduction: 0.5 for minor rhythm clustering in the LPBF section, 0.5 for the "(properly called Weiss domains)" textbook insertion.

## Critic 4: Depth & Rigor (Prof. Henrik Sorensen, Peer Review)
**Score: 8.5/10**

The article does real work explaining the physics rather than summarizing press releases, and it does not shy away from the saturation trade-off, the manufacturing cost problem, or the qualification timeline. The section on saturation flux density is particularly honest, acknowledging that amorphous alloys are not strictly better in all operating regimes and that low-speed, high-torque applications may not benefit.

Sources are mostly well-attributed: UNIST for the 25% iron loss figure, Metglas for core loss data, Busch for direct quotes, AM2SoftMag for project details. The Simizu et al. 2018 and ANSYS Motor-CAD simulation are cited by name/tool but without DOIs or publication venues, which weakens verifiability.

The article correctly identifies the three simultaneous constraints for the LPBF alloy (vitrification, magnetic properties, process compatibility) and explains why the search space is large. It mentions NASA, DLR, and ISS experiments to establish Busch's credentials without overplaying them.

Limitations properly addressed: LPBF build speed, powder cost, qualification timeline. Strongest counterargument (saturation trade-off) gets its own section. The article does not mention one relevant limitation: potential for crystallization during motor operation at elevated temperatures, which could degrade the amorphous structure over time. This is a known concern in amorphous alloy applications and relevant to the 15-year warranty discussion.

Deduction: 0.5 for unverifiable Simizu and ANSYS Motor-CAD citations, 0.5 for omitting thermal stability/recrystallization risk during long-term motor operation, 0.5 for not mentioning that Metglas is now Proterial (formerly Hitachi Metals) when referencing current-day published data.

## Critic 5: Reader Value (David Park, Audience)
**Score: 9.0/10**

A reader finishing this article will understand: why electric motors waste energy in their cores, why amorphous metals are fundamentally better for this application, why nobody could use them before, what changed, and what still stands in the way. That is a complete story arc with genuine explanatory power.

The range translation (2–5% efficiency → 9–24 additional miles on a 300-mile EV) is the kind of concrete output a non-specialist reader can hold onto. The thermal derating discussion adds a second practical dimension that goes beyond the efficiency number.

The saturation trade-off section is valuable precisely because it does not pretend the material is universally better. A reader who is an EV enthusiast or a motor engineer will find the high-speed vs. low-speed distinction useful and honest.

The article is not actionable in the consumer sense (nobody can buy an amorphous motor), but it is genuinely educational about a technology that may reach production in the 2030s, and it explains the physics well enough that the reader can evaluate future claims about amorphous motor cores independently.

Deduction: 0.5 for not providing a timeline estimate for when this technology might appear in production vehicles (even a rough one would help), 0.5 for the mid-article simulation data being harder to absorb than it needs to be.

## Critic 6: Originality (James Holbrook, Technical Journalism)
**Score: 8.5/10**

Most coverage of the AM2SoftMag results (chargedevs.com, interestingengineering.com, newatlas.com, voxelmatters.com) is press-release-derived: it summarizes the "what" and includes Busch quotes. This article goes substantially further by:

1. Building up from first-principles physics (domain reorientation, hysteresis, eddy currents) before introducing the solution.
2. Explaining WHY melt-spun ribbon doesn't work for motors (not just "it's hard to shape" but the specific failure modes: tool dulling, local crystallization at cut surfaces, poor slot geometry from stacking).
3. Connecting LPBF layer thickness to cooling rate requirements, explaining why the process works thermodynamically rather than just stating that it does.
4. Framing the saturation trade-off as a motor-design problem (high-speed vs. low-speed applications) rather than a materials-only issue.

What prevents a higher score: the transformer loss comparison, the Metglas history, and the Simizu/ANSYS data all appear in multiple other technical articles about amorphous metals. The EV-specific framing (range, thermal derating) is the most original contribution, but the supporting evidence sections draw on well-known data points.

Deduction: 1.0 for the supporting evidence being familiar ground in amorphous-materials literature, 0.5 for not engaging with competing approaches (nanocrystalline soft magnetics, thin-gauge silicon steel advances) that are also targeting the same core loss problem.

## Critic 7: Editorial Fit (Elena Voss, efficientdesign.net)
**Score: 9.5/10**

This article is squarely within efficientdesign.net's mandate: engineering-driven, materials-focused, with direct relevance to automotive efficiency. The Cars × Materials Engineering kicker is accurate. The article treats the reader as technically literate without requiring a PhD, which is the site's target register.

The article connects a university research project to real-world EV performance in a way that respects both the science and the reader's time. It does not hype the breakthrough or dismiss its limitations. The closing section is appropriately cautious without being dismissive.

Elena Voss is the right byline: the article has her characteristic attention to materials properties and manufacturing constraints, with a preference for explaining physics over quoting executives.

Minor note: the article could benefit from a brief mention of how this connects to efficientdesign.net's previous coverage of motor efficiency or electrical steel if any exists, but this is a minor editorial preference, not a deficiency.

Deduction: 0.5 for not cross-referencing any previous ED coverage of related topics.

---

## Aggregate Score

| Critic | Score |
|--------|-------|
| Technical Accuracy | 8.5 |
| Narrative Structure | 9.0 |
| Writing Quality | 9.0 |
| Depth & Rigor | 8.5 |
| Reader Value | 9.0 |
| Originality | 8.5 |
| Editorial Fit | 9.5 |
| **Average** | **8.86** |

**VERDICT: PASS (8.86 ≥ 8.5 threshold)**

## Pre-Ship Checks

- **Em dash count (body):** 0 literal `—`, 0 `&mdash;` in body text. 1 `&mdash;` in `<title>` element (standard HTML practice). ✅ PASS
- **"The"-initial sentences:** 13/106 = 12.3%. ✅ PASS (under 15% ceiling)
- **AI slop phrases:** None detected. ✅ PASS

## Recommended Fixes Before Ship

1. **Hitachi Metals attribution (factual error):** Change "Hitachi Metals commercialized this process as Metglas in the 1970s" to "Allied Chemical commercialized this process as Metglas in the 1970s" (or "Allied Chemical, whose successor eventually became part of Hitachi Metals"). Hitachi Metals acquired Metglas from Honeywell in 2003.
2. **Transformer loss reduction:** Consider softening "70 to 80 percent" to "roughly two-thirds" or "65 to 75 percent" to align with Metglas's own published data (losses reduced to "about one-third" of conventional steel).
3. **M19 saturation value:** Consider "approximately 2.0 tesla" instead of "2.2 tesla" for M19 specifically. 2.2T is defensible for generic silicon steels but high for M19.
4. **Simizu et al. citation:** If a DOI or publication venue can be added, it would strengthen this data point. The 30:1 ratio is extreme vs. the more commonly documented 10–14:1 range.
