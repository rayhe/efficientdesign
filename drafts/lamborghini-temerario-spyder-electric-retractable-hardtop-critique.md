# Critique — lamborghini-temerario-spyder-electric-retractable-hardtop (article #261)

Date: 2026-11-25. Author: Marcus Thorne (cars). Topic: Lamborghini Temerario Spyder, unveiled November 19, 2026 — first retractable hard top on a Lamborghini Spyder, fully electric, patented vertical stow, ten actuators, 920 CV HPEV V8.

## Gate results (hard)
- Em dash regex count: 0 (limit 3). PASS.
- Sentence rhythm script (~/workspace/scripts/sentence-rhythm-check.py): PASS first draft. Variance 798.8 (target >=200), short 9.6% (<=15%), long 61.6% (>=15%). 73 sentences.
- "The" sentence starts: 5.5% (4 of 73, incl. title/subtitle/heading fragments). PASS (<=15%).
- Slop phrases ("Here's the thing", "paradigm shift", "game-changer", "deep dive", "unpack") + STORY_GUIDE banned set ("Let's be clear", "Make no mistake", "The kicker:", "X isn't about Y. It's about Z."): none. PASS.
- Hero: media.generate_image -> JPEG 1920x1280 (579,464 bytes, `file` + PIL confirmed), renamed to stories/images/hero-lamborghini-temerario-spyder-electric-retractable-hardtop.jpg. Visual check: orange Spyder rear three-quarter, roof panels stowed vertically behind seats, hexagonal cowls framing exposed twin-turbo V8, warm amber workshop light. Matches alt text. Minor: script badge reads "Lomerario" (generation artifact); acceptable for an editorial illustration, not a product photo. PASS.
- Word count: ~2,116 total incl. spec table and sources; ~1,850 body.

## Critic scores (7 critics, threshold 8.5)
- Technical Accuracy (TA): 9.0 — every spec corroborated against the Lamborghini newsroom release of Nov 19, 2026 (920 CV / 677 kW / 800 Nm; V8 800 CV, 10,000 rpm, 10,250 rpm Launch Control; flat-plane crank, 2.5 bar hot-V turbos, titanium rods, A357+Cu heads, DLC followers; 10 actuators, patented vertical stow, CG -3 mm, weight distribution unaltered; +6%/+9%/+6% spaceframe; 50% fewer components, 80% fewer welds; 13 modes; Citta 190 CV electric; 2.8 s / 7.3 s / 343 km/h) plus Bridgestone release, Hypebeast, Gearculture, Vulkan, ArabWheels, Batmangarage for roof cycle (~17 s, up to 50 km/h), dry weight (~1,805 kg, ~100 kg over coupe), cabin gains (+46/+22 mm), neck warmer, 112 L frunk, Akrapovic (11.40 kg, 12% lighter), Alleggerita (up to 22 kg). Secondary-sourced figures are flagged as such in the Limitations block and hedged in the body ("about", "per secondary reports"). No price used; reported $390,900 figure deliberately excluded as unofficial.
- Engineering Depth (ED): 8.9 — roof-as-packaging thesis (vertical stow inverts the convertible compromise), per-actuator position control vs single-pump hydraulics, failure-mode comparison (stalled actuator vs burst line), heat-affected-zone argument for the 80% weld reduction, flat-plane crank / titanium rods / DLC followers as the three answers to the high-rev turbo problem, CG-direction-over-magnitude framing. Actuator failure modes and service-life unknowns stated as open questions, not glossed over.
- Originality (Orig): 8.8 — "the roof stands up" framing, CG direction as the receipt, "spend money on materials, not on apologies" for the weight options, stiffness-is-the-headline-simplicity-is-the-mechanism, roof-and-engine-in-the-same-conversation close. Not a press-release summary; the release leads with horsepower, this article leads with the roof.
- Voice: 8.7 — opens mid-thought on the November 19 dual unveiling, punchy opinions throughout ("Three millimetres is a small number. Its direction is the point."), Marcus Thorne tone consistent with site's car coverage. No throat-clearing.
- Scholarly Rigor (RV): 8.9 — primary source read directly (lamborghini.com newsroom, crawled Nov 25), 8 corroborating outlets, limitations block states plainly what is not known (no price, no delivery date, no official weight, no durability data), secondary figures quarantined with provenance, reported price excluded. One soft spot: cabin dimension gains are secondary-reported and noted as such only in Limitations, not inline; acceptable, flagged there.
- Sentence Rhythm: 9.0 — script PASS with wide margin (variance 798.8, short 9.6%, long 61.6%); long builds carry layered arguments (roof-compromise paragraph, valve-train paragraph) and short punches land where they matter ("Three millimetres is a small number.", "That matters for a car whose engine note is part of the purchase.").
- Structure (Struct): 8.8 — lede (Nov 19, fifty years of fabric) -> roof mechanism -> frame -> engine -> cabin -> honest weight -> unanswered questions -> close (roof and engine in the same conversation) -> spec table -> limitations -> sources.

**Average: 8.86 — SHIP.**

## Revisions applied
- Limitations paragraph extended to name cabin dimension gains as secondary-reported (not just weight/roof cycle/delivery timing).
- No rhythm or "The"-start revisions needed; first draft passed all gates.

## Topic selection note
- Rivian R2 rejected: already covered three times on this site (rivian-r2-engineering, rivian-r2-material-circularity-1200-pounds-second-life, rivian-r2-second-shift-normal-production-ramp), including the second-shift story this article would have retold.
- Ferrari 849 Testarossa rejected: already covered Nov 11 (ferrari-849-testarossa-five-digital-twin).
- Corvette ZR1X/Zora rejected: already covered Oct 18 (corvette-zr1x-wards-10-best-engines-lt7).
- Temerario Spyder won on recency (unveiled Nov 19, six days before publication) and on a mechanism the site has never covered: an electric, vertically stowed hard top.
