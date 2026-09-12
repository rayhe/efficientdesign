# Research: Stellantis predictive hybrid controller patent (article #187, cars)

## News hook
CarBuzz investigative piece, Sep 11 2026: FCA-US LLC (Stellantis North America) patent describing a
hybrid powertrain control unit that "integrates Kalman filtering with horizon prediction techniques
to effectively address time delay compensation." Target: standard + plug-in hybrids with no clutch to
disconnect the engine from the rest of the powertrain (i.e., CVT/powersplit-style hybrids).

## Key patent quotes (via CarBuzz)
- "the presence of time delays, arising from task scheduling and communication latency between
  control units, can significantly hinder the effectiveness of advanced control algorithms.
  Closed loop performance is often limited by the equivalent time delay between the control
  action command, its effect on the system, and the measurement of the reaction.
  Frequently, commands and measurements originate from different sources, requiring precise
  coordination to accurately estimate the driveline response."
- Controller goal: match electric motors to engine pulses -> reduced driveline shock, smoother journey.
- Applies largely to hybrids "with no clutch available to disconnect the engine from the rest of the
  powertrain" -> aimed at CVT hybrids; usable to some degree on geared transmissions.
- Patent != production intent. CarBuzz caveat retained.

## Technical pillars
1. Kalman filter (Rudolf Kalman, 1960): recursive state estimator. Maintains a model-based prediction
   of system state, fuses it with incoming measurements weighted by their covariances. Handles the
   "measurements from different sources arrive with different latencies and noise" problem.
2. Horizon prediction / MPC: predict system evolution N steps ahead using the model, optimize a
   control sequence over the horizon, apply the first command, repeat (receding horizon).
   MERL reference: Di Cairano & Kolmanovsky, "Automotive Applications of Model Predictive Control,"
   draft Nov 2017: hybrid energy management with multiple power sources (engine, motor, generator)
   requires modeling the power balance Pveh = Peng - Pgen + Pmot - losses.
3. Why hybrids shake: engine torque is a train of combustion pulses (firing-frequency vibration
   component). Powersplit hybrids have no disconnect clutch, so engine-start transients go straight
   through the planetary gearset to the wheels (SJTU/EVS30 paper: "shuffles and jerks"; low-order
   modal resonances of the driveline). Active damping: use the motor as the anti-noise speaker -
   Hyundai/Kia patent US9527503B2 extracts the vibration component of the engine explosion stroke
   and commands antiphase torque from the motor.
4. The delay problem: sensors sample on schedules, CAN arbitration, ECU task scheduling. Even with
   signals at light speed, the control loop acts on stale data. Prediction closes the loop on the
   future state, not the measured past.
5. Compute cost: MPC + Kalman on an automotive ECU is expensive; calibration burden (weights,
   covariance entries, horizons, solver tolerances) is the real engineering (Bemporad CCTA 2020
   slides: "MPC calibration problem" - controller depends on a vector x of parameters).
6. Context: Stellantis hybrid lineup is thin; its 4xe systems are P2 (motor between engine and
   transmission), not powersplit. So this patent builds control IP for an architecture Stellantis
   does not currently sell - future product, or a licensing/defensive play. Toyota owns the
   powersplit topology mindshare; FCA filing here is the notable tension.

## Sources
- Chris (?), CarBuzz, "Stellantis Has A Hybrid Engine Solution That Could Make Toyotas Feel Like A Busted Truck," Sep 11 2026. https://carbuzz.com/stellantis-patent-hybrid-engine-control-september-2026/
- Zhang et al., "A control strategy for a smooth engine start in a power-split hybrid electric vehicle," EVS30. https://papers.evs30.org/download.php?f=papers/EVS30-10320657.pdf
- MDPI Energies 18(11):2847, "Torsional Vibration Characterization of Hybrid Power Systems via Disturbance Observer and Partitioned Learning." https://www.mdpi.com/1996-1073/18/11/2847
- US9527503B2, "Active vibration reduction control apparatus and method of hybrid vehicle" (Hyundai). https://patents.google.com/patent/US9527503B2/en
- Di Cairano, Kolmanovsky, "Automotive Applications of Model Predictive Control," MERL TR2018-213 (draft Nov 17 2017). https://merl.com/publications/docs/TR2018-213.pdf
- Bemporad, "Model Predictive Control: A Rising Technology in the Automotive Industry," CCTA 2020 slides. http://cse.lab.imtlucca.it/~bemporad/talks/ccta2020/bemporad-ccta2020.pdf

## Limitations
- Patent text itself was not directly readable (ppubs.uspto.gov link failed); relying on CarBuzz's
  quoted excerpts. No independent verification of patent claims beyond the excerpts.
- No Stellantis vehicle or concept has been announced using this controller.
- No performance figures (latency reduction, NVH dB improvement) in the public reporting.
- Computational feasibility on production ECUs is inference from the MPC literature, not stated.
