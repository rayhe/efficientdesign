# Critique — mercedes-amg-gt-suv-continuous-power-engineering (article #225)

Date: 2026-10-20. Author: Marcus Thorne (cars). Topic: Mercedes-AMG GT SUV debut (unveiled Oct 17, 2026), first fully in-house AMG SUV on the AMG.EA architecture, with the continuous-power (530 kW) thesis.

## Gate results (hard)
- Em dash regex count: 0 (limit 3). PASS.
- Sentence rhythm script (~/workspace/scripts/sentence-rhythm-check.py): PASS. Variance 2235.2 (target >=200), short 1.4% (<=15%), long 51.4% (>=15%). 9 merges to fix initial FAIL (16.7% short).
- "The" sentence starts: 3.9% (down from 17.4%, 10 surgical rewrites + 9 rhythm merges). PASS (<=15%).
- Slop phrases ("Here's the thing", "paradigm shift", "game-changer", "deep dive", "unpack"): none. PASS.
- Hero: media.generate_image -> JPEG 1920x1280, `file` confirmed, renamed to stories/images/hero-mercedes-amg-gt-suv-continuous-power-engineering.jpg. PASS.
- Word count: ~2,090.

## Critic scores (7 critics, threshold 8.5)
- Technical Accuracy (TA): 9.0 — every spec corroborated across 8 outlets (GTspirit, Review Central ME, ArenaEV, FreshMotors, GSMDome, The EV Report, eMobility Online, NamasteCar): 860 kW peak / 530 kW continuous, 2,000 Nm, 106/128 kWh packs, dielectric oil immersion, 4.1x1.0 in cells, NCMA + silicon anode, >298 Wh/kg, 710 kW charging, 700 km WLTP, 21.2 kWh/100 km, ACTIVE RIDE CONTROL+, 6-degree rear steering, one-foot-rollout basis for 2.5 s, Sindelfingen build, order/availability timeline. 530/860 = 61.6% -> "62 percent" verified. One consistency fix applied (2.7-tonne -> more-than-2.6-tonne to match "over 2.6 tonnes" spec line).
- Engineering Depth (ED): 8.9 — continuous power framed as a cooling-system spec: immersion cooling (no cold plate, no TIM), oil-cooled pancake motors + planetary gearboxes (continuous torque -> continuous heat), SiC inverters as load off the cooling system, pancake thermal path working both directions, two-speed vs single-ratio as car-by-car decision, front-motor disconnect as mechanical-AWD-era habit translated to EV.
- Originality (Orig): 8.7 — the "530 kW not a motor spec; it is a cooling spec" thesis; continuous rating as un-fudgeable segment convention; charging presented as vehicle-side capability with honest infrastructure caveat; AMGFORCE sound criticism (simulated V8 on a car whose philosophy is seamless torque). Not a press-release summary.
- Voice: 8.7 — opens with peak-hp obituary ("a party trick measured in seconds", "what happens on the fourth lap"), punchy opinions (most expensive possible answers; the sound critique; "the first AMG that tells you the whole truth about power"). Marcus Thorne tone consistent with site.
- Scholarly Rigor (RV): 8.6 — limitations stated (not driven; all per published sources), one-foot-rollout convention called out with ~0.2s magnitude, charging figures flagged as infrastructure-dependent/preliminary, continuous-vs-peak ratio computed rather than repeated, sources block with dates and outlet names. Weakest dimension: no conflicting press figures found to surface (specs were unusually consistent).
- Sentence Rhythm: 9.0 — script PASS with margin; variance 2235, short punches retained where they matter ("None of this is free:").
- Structure (Struct): 8.8 — lede (peak vs continuous) -> battery -> motors -> inverters -> disconnects/two-speed -> charging honesty -> mass/chassis -> rollout asterisk -> sound critique -> close -> spec table -> sources.

**Average: 8.81 — SHIP.**

## Revisions applied
- 10 "The"-start rewrites + 9 sentence merges (rhythm FAIL 16.7% short -> 1.4%).
- 2.7-tonne -> more-than-2.6-tonne consistency fix.
- Em dash 0 throughout; no slop phrases.
