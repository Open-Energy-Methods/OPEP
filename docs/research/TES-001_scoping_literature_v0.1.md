# TES-001 — Small-scale sensible-heat TES: research scope and preliminary literature review

**Status:** Draft technical scoping note (not a released test procedure)  
**Revision:** 0.1 — 22 November 2026  
**Project:** Independent personal engineering investigation within Open Energy Methods  
**No institutional sponsorship, assured facility access, experimental results or safety approval is claimed.**  
**Literature status:** Targeted exploratory scan of accessible article records, publisher pages, public institutional documents, and selected full HTML articles. Not a systematic review, exhaustive novelty assessment or full-text critical appraisal of all papers.

## 1. Project decision

Investigate a **small-scale, electrically charged solid sensible-heat thermal energy storage module**, with interchangeable metallic storage bodies, controlled thermal interfaces, measured electricity input, and independent thermal measurements. The central aim is **uncertainty-aware prediction and validation of charge, standby, and eventually controlled discharge**, including loss mechanisms and assembly variation.

This is a self-directed, thesis-level *standard of investigation*, not an enrolled or supervised thesis. The apparatus may use reclaimed materials with documented provenance and appropriate independent characterization. No fixed schedule or deadline.

**Working question:** *How accurately can the charging, standby, and discharging response of a low-cost solid TES module be predicted when thermal contact resistance, fixture heat losses, manufacturing/assembly variation and measurement uncertainty are represented explicitly?*

This proposed question is not a demonstrated novel research gap. Existing work already addresses heat losses, reduced-order model calibration, packing/geometry and experimental TES performance. In particular, Rao et al. (2018) and Niksiar et al. (2024) report complete measured solid sensible-heat charge/discharge experiments, albeit at considerably greater facility complexity. Distinct contribution, if any, must be established through more targeted literature review and acquired physical evidence.

## 2. Scope boundary and definitions

### Included, first investigation
- Mechanical design, CAD, safe fixture manufacture, metrology and provenance for a small solid storage module.
- Protected low-voltage resistive heating **only at a separately approved operating location and configuration**.
- Voltage/current/temperature/time acquisition with documented calibration/reference checks and uncertainty.
- Quantification of storage-body response, heating power, interface influence, remount variability and standby loss.
- Analytical thermal network, transient conduction FEA/finite volume where physically justified, numerical verification, parameter identifiability and independent experimental validation.
- Open engineering files, documented negative results, processed and raw data with metadata, suitably licensed after ownership review.

### Included only after independent discharge metrology is feasible
- Deliberate heat recovery into an independently characterized sink, e.g. a guarded water calorimeter (electrically isolated during discharge, if approved) or an instrumented air stream with calibrated mass flow and inlet/outlet temperature.
- Useful recovered heat, discharge power, charge/discharge efficiency and system-level energy balance with defensible definitions and uncertainty.

### Explicitly deferred
- PCM, thermochemical or pumped-fluid systems; pressurized equipment; industrial-scale packed bed; turbine, combustion or high-temperature tests; grid integration; commercial manufacturing studies.
- The existing 2000 W mains space heater is **not an approved heat source for this rig**. Do not extract its heater or obstruct its vents. No 230 V custom construction in the workshop.

**Scientific naming rule:** The initial apparatus is an *electrothermal characterization platform*. It becomes a defensible *TES performance rig* only when charge, standby, and useful discharge can be quantified with stated boundary conditions and uncertainty. Passive cooling alone is not measured useful heat delivery.

## 3. Literature evidence map (selected primary sources)

| Source | Observed contribution | Consequence for this study | Access / caution |
|---|---|---|---|
| Angrisani et al., 2014, *Applied Thermal Engineering*, [doi:10.1016/j.applthermaleng.2014.03.012](https://doi.org/10.1016/j.applthermaleng.2014.03.012) | Experimentally calibrated a TES model; observed losses about four times a theoretical estimate, notably from thermal bridges and insulation deficits | Model mounting, wires and supports explicitly; do not infer loss from nominal insulation alone | Publisher abstract and accessible excerpts; different, much larger water system |
| MacLeod et al., 2018, *System identification calorimetry*, [arXiv:1808.04518](https://arxiv.org/abs/1808.04518) | Multi-sensor, lumped nonlinear model and system identification used for calorimetry | Compare simpler vs multi-node models; assess whether parameters are identifiable | Preprint abstract inspected; not a TES-specific performance test |
| Firman et al., 2023, *HardwareX* 16, e00496, [doi:10.1016/j.ohx.2023.e00496](https://doi.org/10.1016/j.ohx.2023.e00496) | Low-cost PCM capacity apparatus, validation against DSC/prior evidence | Example of accessible apparatus with validation; relevant to a future PCM module | Open full HTML available; **different physical storage mechanism** |
| Couvreur et al., 2023, *Applied Thermal Engineering* 219, 119526, [doi:10.1016/j.applthermaleng.2022.119526](https://doi.org/10.1016/j.applthermaleng.2022.119526) | Added heat-loss representation to a reduced-order latent TES characterization method and compared against validation cases | Standby and ambient losses can undermine compact predictive models | Publisher abstract; latent storage, not direct validation of our design |
| Schwarzmayr et al., 2023, *Standby efficiency and thermocline degradation...*, [arXiv:2301.01071](https://arxiv.org/abs/2301.01071) | Lab packed-bed standby and thermocline behaviour depends on preceding charge direction | Treat standby as a controlled phase with thermal history | Preprint abstract; packed bed, not solid block |
| Verma et al., 2024, *Designing for effective heat transfer in a solid thermal energy storage system*, [arXiv:2402.07764](https://arxiv.org/abs/2402.07764) | Geometry and heat-transfer access govern solid TES charge/discharge power | Include geometry/heat-transfer path in later module comparison | Modelling of high-temperature graphite/tin; **do not transfer scale or performance** |
| Spietz et al., 2026, *Energies* 19, 3196, [doi:10.3390/en19133196](https://doi.org/10.3390/en19133196) | Measured sensible/latent air-based packed-bed heat storage, recovery, repeatability and uncertainty | Distinguish stored energy from recovered energy, flow and temperature distributions | Publisher full HTML; 25-L high-temperature system and substantially higher heating power |
| Rao, Niyas & Muthukumar, 2018, *Applied Thermal Engineering* 129, 953–967, [publisher](https://www.sciencedirect.com/science/article/abs/pii/S1359431117353991) | Tested 15-MJ cast steel/concrete solid TES prototypes with charge/discharge measurements, fluid circulation and heat-transfer augmentation | Closest conceptual evidence that a solid storage body must be paired with measured heat extraction; prototype size and equipment are not transferable | Publisher abstract and excerpts; industrial-scale laboratory infrastructure |
| Niksiar et al., 2024, *Energies* 17, 5402, [doi:10.3390/en17215402](https://doi.org/10.3390/en17215402) | Compared sand grade and fin configurations in a measured shell-and-tube TES, using hot/cold water loops, flow measurements and spatial thermometry | Geometry and material comparison demands matched fluid boundary conditions; practical example of a complete TES test section | Open full HTML reviewed; more complex pumped system than baseline |
| IHI, *Development of Evaluation Technology for Packed Bed TES*, [technical report](https://www.ihi.co.jp/en/technology/techinfo/contents_no/1200325_13586.html) | Steel ball vs stone test, multiple axial/radial thermocouples, airflow measurements and thermal network model | A concrete example of industrially relevant instrumentation density and model comparison | Industry technical report; not independent benchmarking of our micro-rig |
| IEA SHC Task 67 / ES Task 40, [measurement procedures](https://task67.iea-shc.org/publications) | Round-robin material measurement procedures, reproducibility, uncertainty, material state assessment | Develop traceable measurement and reporting practice | Primarily PCM/TCM, not a normative solid TES rig protocol |
| BIPM/JCGM 100:2008, [GUM](https://www.bipm.org/en/doi/10.59161/jcgm100-2008e) | General measurement uncertainty framework | Standard-uncertainty budgets and covariance for derived energy quantities | Guidance; not evidence of calibrated instruments |
| NIST/SEMATECH, [Engineering Statistics Handbook](https://www.nist.gov/programs-projects/nistsematech-engineering-statistics-handbook) | Experimental design, repeatability, blocking and statistical analysis | Predefine experimental units, factor changes and repeats | General methodology |
| ASME V&V 20-2009 (R2021), [standard overview](https://www.asme.org/codes-standards/find-codes-standards/standard-for-verification-and-validation-in-computational-fluid-dynamics-and-heat-transfer) | Credible comparison of computational and experimental quantities, with uncertainty | Define validation quantities and points; separate numerical verification from experimental validation | **Not claiming compliance with full purchased standard** |
| IEC TS 62862-2-1:2021, [official overview](https://webstore.iec.ch/en/publication/31588) | Charge/discharge, uncertainty and loss reporting procedures for active sensible storage in solar thermal plants with **liquid** media | Illustrative system-level reporting concepts, not directly applicable requirements to a metal-block rig | Scope mismatch; **do not claim IEC compliance** |

### Research gap hypothesis, to be challenged
A low-resource, interchangeable **metallic** TES module with published assembly/remount datasets, explicit measurement-chain uncertainty, energy balance, model identifiability checks, and **held-out** charging/standby/discharge validation *may* provide a useful reproducible methodological case study. Similar low-cost calibration and TES studies already exist. Publication novelty is **unproven** until a reproducible database search and detailed competing-method comparison are complete.

Next search work: Scopus/Web of Science/OpenAlex or equivalent with a dated search log, controlled synonyms (solid sensible TES, thermal battery, metal block, test bench, thermal network, calorimetry, inverse identification, thermal contact, remount, uncertainty, open hardware), forward/backward citations, pre-registered inclusion rules and close review of directly competing methods.

## 4. Architecture selection

| Candidate | Advantages | Limitation / decision |
|---|---|---|
| A. Removable aluminium/steel solid block + controllable heater + guarded interfaces | Small, robust, easy to machine, amenable to heat-capacity estimates, simpler uncertainty analysis | **Choose for baseline** |
| B. Air-fed sand/rock/steel-ball packed bed | Strong industrial TES relevance, breakthrough physics, reclaimed storage medium | Requires safe hot-air stream, **measured air flow** and pressure loss; large boundary-condition uncertainties at small scale. **Defer** |
| C. PCM capsule | Latent storage and state-of-charge research | Composition, hysteresis, leakage, heat capacity and reference characterization; more complex safety/provenance. **Defer** |
| D. Water vessel | High heat capacity and potential stratification study | Water containment, heating safety, stratification, fluid flow and access issues. **Not initial storage architecture** |

**Provisional starting envelope**, purely for designing measurement feasibility: ~0.5–1.5 kg metal storage body; temperature rise of tens of kelvin; guarded low-voltage resistive input of the order of tens of watts. No heater setpoint, temperature limit, protection design or mechanical drawing is authorized by this note. Chosen parameters depend on actual material, fixtures, instrumentation and local approval.

Illustrative magnitude only: 1 kg aluminium with an assumed representative 900 J/(kg K) heat capacity and 40 K rise holds ~36 kJ (~10 Wh) in the metal; this ignores fixtures, heater, cp variation and all losses. For 30 W **net stored power** the ideal charge time would be ~20 minutes, not a predicted test duration. Electrical input and net stored power are **not equal** in general.

## 5. Measurement boundaries and equations

Define charge/discharge boundaries, reference temperature, initial states, ambient and useful sink. Distinguish **electrical input**, **increase in internal energy**, **ambient losses**, **useful delivered heat** and **final residual energy**.

Approximate metal-only stored energy, for a well-characterized near-uniform body:

U_s(T)-U_s(T_ref) = m_s * integral[T_ref..T] cp_s(theta) dtheta.

Temperature gradients require spatial modelling/integration. Unknown scrap alloy cp and conductivity require independent property evidence, realistic intervals or restrictions on claims.

Electrical energy delivered to the heater terminals (measured synchronously for transient power):

E_elec = integral[V_h(t)*I_h(t) dt].

A conceptual integrated control-volume balance:

E_elec = Delta(U_metal + U_fixture + U_heater + other components) + Q_ambient + Q_useful + E_other + residual.

No component is zero by assumption. Resistive heating terminals, cables, electronics and supports may lie inside or outside the chosen control-volume boundary.

Measured useful output options:
- **Later guarded water calorimeter**: heat collected by a known water mass and characterized vessel, corrected for independent background losses and retained heat, after electrical disconnection where required.
- **Later air discharge**: integral of measured air mass flow times enthalpy rise between inlet and outlet; must validate flow and transient sensor response, bypass and wall losses.

A temperature decay curve alone cannot establish a system round-trip efficiency.

Model hierarchy:
- M0: analytical constant-property, spatially lumped thermal RC model; check Biot-number implications before treating as one node.
- M1: 2–3-node network separating heater, metal storage, fixture and ambient; avoid fitting more unknowns than measurements can distinguish.
- M2: transient conduction finite-element/finite-volume model with measured geometry, verified mesh and time step, and physically justified loss boundaries.
- M3: coupled airflow/CFD only when measured airflow and thermal boundary information are adequate.

**Identifiability check:** Confounded coefficients (e.g. heat capacity vs ambient conductance, or heater contact vs fixture bypass) cannot be uniquely inferred merely because an optimizer fits temperature traces. Evaluate sensitivity, parameter correlation and predictive robustness; obtain an independent input/configuration where needed.

## 6. Hypotheses and minimum experiment sequence

- H1: Interface configuration/remounting contributes distinguishable variation to transient temperature response after measurement uncertainty and ambient drift are accounted for.
- H2: An explicitly measured fixture/ambient loss model improves **held-out** prediction relative to an idealized adiabatic or single-loss baseline.
- H3: A model calibrated on a subset of charge/standby conditions predicts **independent** input and assembly conditions within a quantified discrepancy distribution, rather than only the fitted traces.
- H4 (conditional): Useful discharged energy into a separately measured sink can be reconciled against initial stored energy, final residual energy and ambient losses within a pre-agreed uncertainty budget.

Planned stages and **gates**:
1. **G0: Access/instrument/safety gate** — written agreement on fabrication, powered testing site, supply, guarding and independently acting thermal protection. Check multi-channel temperature references/DAQ, mass/dimension measurement. If unavailable, no powered test at EECS.
2. **G1: Metrology/material baseline** — material source, cleaning/inspection, mass/dimensions, sensor cross-comparison and calibration evidence, thermal property provenance and preliminary uncertainty budget. Choose one reference module; no many-material comparison yet.
3. **G2: Component/fixture engineering** — CAD, tolerance and manufacturing records, part identification, mounting load method, sensor location and thermal interface, independent physical/safety review. No machined drawing until actual dimensions and safety are approved.
4. **G3: Pilot system identification** — authorized low-power charging and passive standby; acquire heat input, ambient, 3–5 spatial temperature measurements, replicate after independent remounts. Check data integrity, lag, energy consistency and model identifiability.
5. **G4: Locked validation campaign** — freeze model and analysis code, test an uncalibrated power profile or fresh assembly/configuration; report predictive residuals versus combined uncertainty and baseline performance.
6. **G5: Useful discharge calorimetry** — only if an independent heat sink can be characterized. Test charge/standby/deliberate discharge and measure useful recovery; then define and report carefully bounded TES efficiency.
7. **G6: Research report** — measurement uncertainty tables, verified code, raw and processed data, negative results, sensitivity/limits, comparison to competing literature and reasoned novelty assessment.

### Prospective experiment matrix (illustrative, **not approved**)
Pilot: two thermal interface configurations with independent remounts; at least one low and one higher input level **subject to safety limits**, plus passive standby. A plausible initial structure is 2 interfaces x 2 safe power conditions x 3 independent assemblies = 12 charge/standby records, but change factors and sample count after pilot variance and identifiability analysis. Reserve an additional different input profile and fresh remounts exclusively for validation. Repeated time samples on one run are not replicate assemblies. Randomize or block run order where feasible.

Record room conditions and changes in mounting geometry; torque settings are not necessarily known contact forces. Measure sensor positions and verify they have not shifted after remounting.

### Reportable outputs
- Charge input energy/time series, spatial temperature response, estimated stored sensible energy with property/temperature uncertainty, and standby decay.
- Ensemble repeatability by independent assemblies and sample material provenance.
- Model prediction error, residual structure, numerical error estimates, parameter sensitivity/identifiability and interpolation/extrapolation boundaries.
- **Only with G5:** delivered heat, power curve, energy-recovery fraction and any defined TES efficiency, with measurement uncertainty and complete heat-accounting boundary.

## 7. Instruments and construction

**Borrow/verify before buying:** bench DC power supply, multimeters, 3–5 suitably characterized temperature channels and time-synchronized logging, weighing scale, calipers/micrometer, mounting-force/torque method, suitable cooling or calorimetry apparatus.

**Likely needed even when scavenging:** known-rated heating element, new appropriate thermal cutout/protective parts, suitable insulated wire, rated connectors, guarded enclosure, known temperature probes/attachment media, fastening hardware, verified insulation materials, storage specimen/stock if no usable offcuts.

**Not established at KTH:** calibrated thermometry, multi-channel DAQ, physical approval for powered heating, workshop stock for this experiment, use of machining outside supervised access, or permission for independent calorimetry.

A reclaimed CPU cooler and 12-V fan may serve as later discharge interface components, but their heat-removal performance cannot be presumed from fan labels. Scrap metal is acceptable for exploratory prototypes; unknown alloy properties limit quantitative material comparisons until adequately characterized.

## 8. Safety and facility restrictions

The KTH EECS Student Workshop publicly lists electronics workstations, supplies, multimeters, assembly and supervised metal-machining facilities. Its written rules prohibit working alone and work on live circuits; supervisory booking is required for milling, turning, CNC and other listed machines. [KTH workshop](https://www.kth.se/emp/student-workshop/studentverkstan-1.683473), [safety](https://www.kth.se/emp/student-workshop/regler-och-sakerhet/regler-och-sakerhet-1.683474), [electronics](https://www.kth.se/emp/student-workshop/verkstan/elektronik-1.686912), [manufacturing](https://www.kth.se/emp/student-workshop/verkstan/mekanik-1.686913).

An available bench power supply does **not** establish permission for a continuously energized, heat-producing test article. Obtain explicit site approval of the circuit, overtemperature response, flammable-material clearance, emergency shutoff, operating supervision and storage. If prohibited, use the workshop for authorized cold fabrication/assembly only and a different approved test space for heating. Do not modify or repurpose the discarded 2000 W mains space heater.

Never use reclaimed high-voltage parts, unknown high-temperature insulation, damaged power connectors or unverified safety devices. No pressure vessel, combustor, exposed high-speed rotating assembly or high-temperature molten material.

## 9. Data and scientific release

- Raw data immutable; include timestamps, units, timebase, calibration, sensor placement, ambient conditions, power state and equipment IDs.
- Assembly/run IDs distinct; preserve unprocessed physical data and identify all simulated/synthetic data as such.
- Freeze independent validation runs before parameter fitting; record exclusions and failures.
- Analysis scripts reproduce equations, uncertainty budgets, model verification, plots and versioned research reports.
- Use an uncertainty-aware energy-balance closure criterion determined **before** full testing, after an instrument capability analysis; do not invent a universal target or interpret unclosed energy as zero loss.
- Documents/working hardware are **not** laboratory-certified, a KTH thesis, or evidence of standard conformity.

## 10. Decision points and next research work

**Preferred first build:** small, removable, known-metal solid storage cartridge on an independently characterized mount, plus measured low-voltage heating **if expressly approved**, 3–5 temperature measurements and initial standby characterization.

**Immediate tasks before procurement:**
1. Obtain workshop approval answer and actual inventory of usable temperature/voltage/current metrology.
2. Inspect available reclaimed specimens and characterize mass/geometry/material confidence.
3. Bound thermal storage capacity and sensor resolution/uncertainty for candidate masses and temperature rises; establish whether the expected treatment effect is measurable.
4. Perform a targeted full-text novelty audit, especially around low-cost metal-block thermal characterization, calorimetry, model identifiability and repeatable mount/thermal resistance.
5. Choose useful discharge measurement route before claiming TES cycle efficiency.
6. Update the **public proposal** only after this decision note has been reviewed; do not silently replace the separate EBT research programme.

### Status note

This is **literature-informed scoping only**. No equipment has been qualified, no test location approved, no component purchased for the proposed TES campaign, no verified measured dataset acquired and no publishable novelty established.