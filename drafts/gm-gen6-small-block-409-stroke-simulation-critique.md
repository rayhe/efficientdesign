# Critique Notes — Article #201: Two Millimeters: How Simulation Gave GM's Small Block 409 Cubic Inches

Slug: gm-gen6-small-block-409-stroke-simulation
Author: Elena Voss | Date: 2026-09-26
Gates (all on final draft): em dash count 0 (<=3 PASS) | "The"-starts 4.5% (<=15% PASS) | rhythm script PASS (variance 701.6, short 13.6%, long 50.0%)

## 1. Technical Accuracy — 9.0/10
Every claim traced to coverage of the September 16-17, 2026 reveal:
- Flint Engine Operations media day, Sept 16, 118th anniversary of GM's 1908 founding in Flint, Reuss quote ("The small block V-8 has been a great story for GM for seven decades...") — USA Today.
- L76 5.7L/350ci: 402 hp, 428 lb-ft; L78 6.6L/400ci: 481 hp, 501 lb-ft — EngineLabs. "Most powerful naturally aspirated V8 available in the truck class" attributed to GM, not stated as fact.
- Outgoing 5.3L 355 hp / 6.2L 420 hp — EngineLabs. +6mm truck stroke — EngineLabs.
- LS6 6.7L/409ci: 535 hp @ 6,100, 520 lb-ft @ 4,600, 13.0:1, 6,600 redline, 95mm throttle body, tunnel-ram intake, forged pistons/rods, aluminum block with cast-in iron liners, A356-T6 heads, direct+port injection + AFM — GM Authority wiki, EngineLabs converge. "Most powerful base engine ever offered in a Corvette" and "highest-torque naturally aspirated V8 currently in production" attributed to GM.
- Originally planned as 6.6L; ~2mm additional stroke discovered via simulation; stroke 92→100mm vs LT2 — GM Authority. Bore 103.25mm, 4.4in bore spacing — GM Authority, EngineLabs.
- Five-year development; Mike Kociba (Asst Chief Engineer), Casey Morrison (LS6 Design System Manager) — LSX Magazine. Both Kociba quotes sourced to LSX Magazine, with attribution reworded to avoid implying the full quote context is the final 2mm tweak.
- "400" stamped on L78 block — EngineLabs.
- Continuously variable oil pump, engine-mounted oil cooler, revised oil-feed locations — EngineLabs. The Gen-5 recall framing is explicitly presented as the author's reading ("reads as a response"), not a GM claim.
- 409 echoing 1962 — LSX Magazine. 100M+ small-blocks over seven decades — LSX Magazine. Grand Sport X 721 hp combined — EngineLabs.
- Spec table marks truck bore/stroke, compression, redline as "not disclosed" rather than guessing.
- FIXED in pass: the +33 cubic inches figure was conflated with the +2mm finding in draft 1 (33ci is LT2 6.2L→LS6 6.7L; the planned 6.6→shipped 6.7 step is ~6ci). Paragraph now separates the two. AFM claim scoped: confirmed on LS6 per GM Authority wiki; truck AFM not sourced.
- Caveat stated: hardware not handled, figures are GM's as reported.

## 2. Engineering Rigor — 9.0/10
Original contribution present: (a) the 4.4-inch bore-spacing constraint as the reason stroke was the only displacement lever, with the deck-space argument spelled out; (b) the displacement-economics framing, what stroke costs (taller deck, piston speed, redline) vs what bore costs, and why the simulation result inverts the usual cost structure; (c) the dual-injection division of labor (charge cooling for knock, port wash for valve carbon) rather than treating it as a marketing bullet; (d) the oiling-system rethink read as a response to Gen-5 recall history, framed as inference. Each analysis point is labeled as analysis. Limitation stated in refs.

## 3. Voice / Human-likeness — 9.0/10
Opens mid-thought ("the headline number was not the horsepower"), fragments ("None of those figures required a turbocharger. All of them came from geometry, compression, and airflow. That is the whole point."), real opinions ("This is the unglamorous half of engineering appreciation, and it is the half that matters most."), dry close ("The obituaries were premature. They usually are."). Elena's register consistent with #200's Rolex piece: mechanism-first, romance-second.

## 4. Sentence Rhythm — 9.5/10
Script PASS: variance 701.6 (target >=200), short 13.6% (<=15), long 50.0% (>=15). Punchy opens ("That is the whole point.", "The number is not an accident.") against 30+ word builds. No metronome stretches.

## 5. Anti-Slop — 10/10
Zero banned phrases (checked against STORY_GUIDE.md list + the five extras: "Here's the thing", "paradigm shift", "game-changer", "deep dive", "unpack"). Zero em dashes, literal and entity. No market-speak filler.

## 6. Structure — 9.0/10
Announcement → the two-millimeter discovery → the bore-spacing constraint → 13:1 compression → oiling system → 409 heritage → spec table → refs with caveat. Logical escalation from news to mechanism to meaning. Spec table complete (14 rows, unknowns marked).

## 7. Title / Subtitle — 9.0/10
"Two Millimeters: How Simulation Gave GM's Small Block 409 Cubic Inches" is specific and falsifiable; subtitle front-loads the mechanism (simulation-found stroke) rather than the horsepower. Risk: readers unfamiliar with small-block lore may not know why 409 matters, but the 409 section answers it in the text.

## Composite: 9.2/10 (>= 8.5 SHIP)
