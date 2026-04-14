# HailShapes Document Index

**Purpose:** Quick-reference summary of all research documents on hail shape, impact, and damage patterns.  
**Use Case:** Counter insurer claims that hail damage to windows is always round without scratches.  
**Total Documents:** 24 research documents across 5 folders + 4 project documents + 2 insurer documents  
**Last Updated:** April 11, 2026  

**Relevance Legend:** CRITICAL = Directly counters insurer claims | HIGH = Strong supporting evidence | MEDIUM = Supplementary support

---

## Key Formulas and Theorems Reference

This section collects the most important equations from the academic papers. See individual document entries below for full context.

### Terminal Velocity of Hailstones

**General form** (A-4, A-8, S-9):
```
vt = √(4·g·ρh·D / (3·Cd·ρa))
```
Where: vt = terminal velocity (m/s), g = 9.81 m/s², ρh = hailstone density (917 kg/m³), D = diameter (m), Cd = drag coefficient, ρa = air density (1.225 kg/m³).

**Why it matters:** Drag coefficient Cd varies with hailstone shape — irregular shapes have higher Cd (0.45–0.80) than smooth spheres (~0.47), meaning non-spherical hail falls slower and is MORE deflected by wind, producing MORE angled impacts.

**Empirical terminal velocity models** (A-4):
```
v = 9.9 × D^0.38   (hailstones up to 8 cm)
v = 7.6 × D^0.89   (diameters < 1.5 cm)
v = 8.4 × D^0.67   (diameters ≥ 1.5 cm)
v = 14.04 × D^0.5  (ASTM E822 standard)
```

### Resultant Impact Velocity with Wind

**Resultant velocity** (A-4):
```
vr = √(vw² + (vt + vd)²)
```
Where: vr = resultant velocity, vw = horizontal wind speed, vt = terminal velocity, vd = downdraft speed.

**Why it matters:** The impact angle θ = arctan(vw / (vt + vd)). Any horizontal wind component means hail strikes at an angle, NOT perpendicular. This directly produces elongated, non-circular damage marks.

### Peak Impact Force with Wind (Regression Model)

**From A-1** (Applied Sciences, 2025):
```
Fp = 2.321·Vw + 6375.502·d + 9.487·Vhail − 262.402
```
Where: Fp = peak impact force (N), Vw = wind speed (m/s), d = hailstone diameter (m), Vhail = hail velocity (m/s). R² significant at p ≤ 0.001.

**Standardized coefficients (Beta):** Hail velocity (0.564) > Hail diameter (0.506) > Wind speed (0.344) — all three factors are statistically significant.

### Peak Impact Force with Turbulence

**From A-10** (Scientific Reports / Nature, 2024):
```
F = −0.624·Iu + 5116.25·D + 7.85·Vhail − 259.709
```
Where: F = peak impact force (N), Iu = turbulence intensity (%), D = hail diameter (m), Vhail = hail velocity (m/s). R² = 0.984.

**Why it matters:** Turbulence REDUCES peak force (negative coefficient) but makes impact behavior MORE irregular and unpredictable — further contradicting uniform round damage.

### Kinetic Energy of Hail Impact

**Basic kinetic energy** (A-1, A-8):
```
E = ½·m·v²
```
Where: m = ρice·(4/3)·π·r³, with ρice = 917 kg/m³ (A-5) or 875 kg/m³ (A-8).

**HIR Classification kinetic energies** (A-8, JCHE):

| Diameter | Mass | Terminal Velocity | Kinetic Energy |
|----------|------|-------------------|----------------|
| 10 mm | 0.5 g | 13.8 m/s | 0.04 J |
| 20 mm | 3.6 g | 19.5 m/s | 0.7 J |
| 30 mm | 12.3 g | 23.9 m/s | 3.5 J |
| 40 mm | 29.2 g | 27.5 m/s | 11.1 J |
| 50 mm | 56.9 g | 30.8 m/s | 27.0 J |

### Dent Depth Formula

**From A-9** (Scientific Reports / Nature, 2022):
```
D = √(α × (m·V²)/(2·t·σf) − β × (σf·π·φ⁴·l³)/(32·E·t³·h³))
```
Where: D = dent depth, m = hailstone mass, V = impact velocity, t = sheet thickness, σf = yield stress (320 MPa for steel), E = Young's modulus (200 GPa), φ = hailstone diameter, l = support spacing, α = rebound energy coefficient = (1 − COR)², β = pressure area coefficient.

**Why it matters:** Dent depth depends on velocity, mass, material thickness, yield stress, AND support spacing. The same hailstone produces different dent depths on different materials, explaining why damage varies across window components.

### Dent Diameter Formula

**From A-3** (Shock and Vibration, 2019 — RETRACTED):
```
Ds = √((Cs·m·v²)/(2π·σy·t) − (Dd·σy)/(8E))
```
Where: Ds = dent diameter, Cs = energy conversion coefficient, Dd = dent depth.

### Energy Conservation at Impact

**From A-9** (Scientific Reports / Nature, 2022):
```
E_impact = E_vibration + E_plastic + E_rebound
```
Where: E_plastic = π·D²·σf·t (plastic deformation energy), E_vibration = F²/(2k) with k = E·h³/l³ (flexural stiffness).

**Why it matters:** Impact energy partitions into vibration, plastic deformation, and rebound. The ratio depends on material properties, meaning different window materials (vinyl, aluminum, steel, glass) absorb energy differently and show different damage patterns.

### Hailstone Shape Parameters

**From S-9** (Lin et al. 2024):
```
Dmax = 1.3978·Deq^0.5 − 0.1486       (max dimension vs. equivalent diameter)
Rmi = Dmi/Dmax                          (major axis ratio)
Rmn = Dmn/Dmax                          (minor-to-major axis ratio)
```

**Terminal velocity for nonspherical hailstones:**
```
vt = (4·ρi·Deq / (3·ρa·Cd))^(1/5)
```

**Nusselt number (heat transfer):**
```
Nu = 2.0 + 0.6·Pr^(1/3)·Re^(1/2)
```

**Why it matters:** Non-spherical shapes have different axis ratios, drag coefficients, and heat transfer rates. These directly affect how hailstones fall, tumble, and impact surfaces.

### Glass Failure Prediction

**From A-CIB** (Fragility curves for toughened glass):
```
ηp(Vf) = Kd/Kc − 1 ≥ 0
```
Where: Kd = dynamic stress intensity factor, Kc = quasi-static fracture toughness (0.75 ± 0.05 MPa·m^0.5 for toughened glass).

**Crack distribution (log-normal):**
```
f(cd) = (1/(√(2π)·σc)) × exp[−(1/2)·((ln(cd) − μc)/σc)²]
```
Where: cd = half-length of dominant crack, μc and σc = statistical parameters of flaw distribution.

**Why it matters:** Glass failure depends on pre-existing microflaws and crack distributions — NOT just on hailstone shape. The same hailstone impact produces different fracture patterns on different glass panes because of varied background flaw distributions. This explains why window damage appears irregular.

### Wind Velocity Decomposition

**From A-7/Thunderstorm** (Calotescu et al. 2024):
```
v(t) = V̄(t) + v'(t)
Iu(t) = σv(t) / V̄(t)
```
Where: V̄(t) = mean wind speed, v'(t) = turbulent fluctuation, Iu = turbulence intensity.

**Hailstone kinetic energy scaling:**
```
Ek = a·D^b
Vt = c·D^d
```
Where: a, b, c, d = empirical constants fitted to storm data.

---

## Shapes Folder

### S-1: Lumpy, Bumpy Hail: Realistic Hail Shapes May Improve Modeling of Severe Weather
- **File:** `Shapes/1. Lumpy, bumpy hail_ Realistic hail shapes may improve modeling of severe weather _ Penn State University.pdf`
- **Source:** Penn State University / Journal of the Atmospheric Sciences (Oct 2024)
- **Type:** University Research / Peer-Reviewed
- **Relevance:** CRITICAL
- **Summary:** Demonstrates that hailstones are NOT spheres but rather lumpy with spikes. Research supported by Insurance Institute for Business and Home Safety (IBHS). Models using realistic non-spherical shapes produce different size/trajectory predictions.
- **Key Findings:** Hailstones are lumpy with spikes, not spheres. Shape affects trajectory, heat transfer, and growth. Small trajectory changes create large shape variations (butterfly effect). Even the insurance industry's own research body acknowledges non-spherical hail.

### S-2: Zombie Hail: What Causes Odd Hail Shapes
- **File:** `Shapes/2. Zombie Hail_ What causes odd hail shapes _ wqad.com.pdf`
- **Source:** WQAD (Andrew Stutzke, Oct 2019)
- **Type:** Professional Meteorology / News
- **Relevance:** HIGH
- **Summary:** Documents hailstones resembling angels and starfish with jagged edges. Explains wet growth process where sticky liquid layer causes stones to collide and adhere, creating jagged multi-stone aggregations.
- **Key Findings:** Hail observed as angel/starfish shapes with jagged edges. Wet growth creates sticky surfaces causing aggregation. Updraft speeds 30-90 mph create variable tumbling.

### S-3: Come Hail and High Water (The Australian)
- **File:** `Shapes/3. Subscribe to The Australian _ Newspaper home delivery, website, iPad, iPhone & Android apps.pdf`
- **Source:** The Australian Newspaper
- **Type:** News Report
- **Relevance:** MEDIUM
- **Summary:** Reports monster hailstones shaped like cauliflowers, poached eggs, and jellyfish during NSW coast storm. Bureau of Meteorology forecaster confirms shape determined by path through storm.
- **Key Findings:** Hailstones observed as cauliflower, poached egg, and jellyfish shapes. Shape determined by path through storm, time in updraft, and time at negative temperatures.

### S-4: Hail Formation, Explained
- **File:** `Shapes/4. Hail formation, explained _ CNN.pdf`
- **Source:** CNN (Jennifer Gray & Madison Richardson, Apr 2023)
- **Type:** Major Media / Educational
- **Relevance:** MEDIUM
- **Summary:** Explains wet vs. dry growth processes that create different hail shapes. Wet growth produces interesting shapes as pieces combine. Documents speeds over 100 mph for large hailstones.
- **Key Findings:** Wet growth gives hail interesting shapes depending on how pieces combine. Dry growth creates cloudy appearance. 4-inch hail falls at over 100 mph.

### S-5: Patterns in Nature: Hailstones and Their Aftermath
- **File:** `Shapes/5. Patterns in nature_ Hailstones and their aftermath – letting nature back in.pdf`
- **Source:** naturbackin.com (Blog / Storm Documentation)
- **Type:** Firsthand Documentation
- **Relevance:** HIGH
- **Summary:** Photographic documentation of actual hailstorm showing various shapes and sizes. Documents window penetration damage — dining room window had holes beaten through glass panes.
- **Key Findings:** Mixed sizes and shapes in single storm. Hailstones punched through window panes. Window damage patterns consistent with irregular high-velocity projectiles.

### S-6: Severe Weather 101: Hail Types
- **File:** `Shapes/6. Severe Weather 101_ Hail Types NOAA.pdf`
- **Source:** NOAA National Severe Storms Laboratory
- **Type:** U.S. Government Authority
- **Relevance:** CRITICAL
- **Summary:** Official NOAA statement that hailstones can have a variety of shapes including lumps, bumps, and small spikes. Distinguishes hail from other precipitation types.
- **Key Findings:** Hailstones have variety of shapes with lumps, bumps, and spikes. Growth through collection of water freezing onto surface creates varied morphology.

### S-7: Why Do Hail Shapes Vary?
- **File:** `Shapes/7. Why do hail shapes vary_ _ wqad.com.pdf`
- **Source:** WQAD
- **Type:** Professional Meteorology / News
- **Relevance:** MEDIUM
- **Summary:** Explains the atmospheric conditions and formation processes that lead to varied hail shapes. Details how wet and dry growth modes produce different surface characteristics.
- **Key Findings:** Multiple growth modes create varied shapes. Environmental conditions at different altitudes affect shape. Wind shear influences growth trajectory.

### S-8: Shape of Hail and Its Thermodynamic Characteristics Related to Records in Catalonia
- **File:** `Shapes/1-s2.0-S0169809522000849-am.pdf`
- **Source:** Farnell, Rigo & Heymsfield — Atmospheric Research (Elsevier, Feb 2022)
- **Type:** Peer-Reviewed Scientific Study
- **Relevance:** HIGH
- **Summary:** Study of 151 hailstorms categorizing hail into spherical, irregular, and embryo types. Irregular hail has no smooth parts, with contours formed by tiny lobes. Shape depends on dynamic and thermodynamic conditions.
- **Key Findings:** Three recognized shape categories: spherical, irregular, embryo. Irregular hail lacks smooth surfaces. Sizes range 1-6 cm. Wind shear prolongs updraft residence time affecting shape.
- **Key Quantitative Data:** Wmax (max vertical updraft velocity): 30-40 m/s general, up to 80 m/s for summer irregular cases. Wind shear: 5-10 m/s (spring), 10-15 m/s (summer/autumn), >18 m/s (supercells). Precipitable water: ~35 mm (summer), 20-25 mm (spring). Hail sizes: Spring 1-3 cm median, Summer 1-6 cm (Q2 ~3 cm), Autumn 1.5 cm median. Irregular hailstone max diameter: ~5 cm (median ~4 cm).

### S-9: Modeling Nonspherical Hailstones
- **File:** `Shapes/atsc-JAS-D-23-0231.1.pdf`
- **Source:** Lin, Kumjian, Soderholm & Giammanco — Journal of the Atmospheric Sciences (Nov 2024)
- **Type:** Peer-Reviewed Scientific Study
- **Relevance:** CRITICAL
- **Summary:** Explicitly models non-spherical hailstones. States hailstones in nature are lumpy with spikes, categorized as spheroids, ellipsoids, or conical with possible lobes. Shape affects terminal velocity, growth rate, and melting.
- **Key Findings:** Natural hailstones classified as spheroids, ellipsoids, or conical with lobes. Shape affects fall behavior and damage potential. Spherical assumption in models is unrealistic.
- **Key Formulas:** Dmax = 1.3978·Deq^0.5 − 0.1486 (max dimension relationship); vt = (4·ρi·Deq/(3·ρa·Cd))^(1/5) (terminal velocity for nonspherical hail); Nu = 2.0 + 0.6·Pr^(1/3)·Re^(1/2) (heat transfer); 28 numbered equations total covering rime density, shape parameters, drag coefficients, and shedding mechanics.

---

## AcademicPapers_Claude Folder

### A-1: Experimental Study on the Effect of Wind Speed on Hail Impacts
- **File:** `AcademicPapers_Claude/1. Eprrimental Study on the Effect of Wind Spped on Hail impacts-applsci-15-05120.pdf`
- **Source:** Applied Sciences (Peer-Reviewed Journal, 2025)
- **Type:** Peer-Reviewed Academic Paper
- **Relevance:** CRITICAL
- **Summary:** Tests hail impacts at various wind speeds. At 13 m/s wind speed, peak impact force increases 18.9%. Wind-hail coupling creates non-perpendicular impacts producing elongated damage. Turbulence intensity affects impact behavior.
- **Key Findings:** Wind speed amplifies peak forces by 18.9%. Turbulence creates irregular impact behavior. Impact angle varies with wind, producing non-circular damage patterns. Turbulence variation (2.5% to 25.5%) produces ~21.84% decrease in peak impact force. Influence order: hail velocity > hail diameter > turbulence intensity.
- **Key Formulas:**
  - Mass: `m = ρi·(4/3)·π·r³` (ρi = 0.9 × 10³ kg/m³)
  - Terminal velocity: `v = (4·ρi·g·d / (3·ρa·Ca))^(1/2)` where Ca = 0.41·D^(−0.185) for 0.5 cm ≤ D ≤ 5 cm
  - Kinetic energy: `E = ½·m·v²`
  - **Peak impact force regression: `Fp = 2.321·Vw + 6375.502·d + 9.487·Vhail − 262.402`** (all coefficients p ≤ 0.001)
  - Standardized Beta: Vhail (0.564) > d (0.506) > Vw (0.344)
  - Peak forces for 3.2 cm hailstone: 110.9 N (no wind) → 159.2 N (13 m/s wind)

### A-3: Examining Dent Formation Caused by Hailstone Impact
- **File:** `AcademicPapers_Claude/3. Shock and Vibration - 2019 - Uz - Retracted  Examining Dent Formation Caused by Hailstone Impact.pdf`
- **Source:** Shock and Vibration (2019)
- **Type:** Academic Paper (RETRACTED — use cautiously)
- **Relevance:** MEDIUM
- **Summary:** Finite Element Model of hail dent formation. Shows dent profiles are NOT purely circular — deformation varies across impact zone. Dent depths vary 2.78-2.95mm for same-sized hailstones.
- **Key Findings:** Dent profiles are not purely circular. Steel sheet thickness (0.30-0.70mm) affects dent resistance. Variable dent depths from same-sized hail due to material and momentum variations.
- **Key Formulas:**
  - Denting force: `Fd = Ks·σy^n·t^(p−5)` (Ks = 17.78)
  - Energy for visible dent: `W0 = Kw·σy^0.915·t^0.322` (Kw = 0.005)
  - Dent diameter: `Ds = √((Cs·m·v²)/(2π·σy·t) − (Dd·σy)/(8E))`
  - Dent depth: `Dd = √(α·(m·V²)/(2·t·σf) − β·(σf·π·φ⁴·l³)/(32·E·t³·h³))`
  - COR = Rebound Velocity / Impact Velocity; α = (1 − COR)²
  - Material: σy = 320 MPa, E = 200 GPa, hail E = 9.38 GPa

### A-4: Geosciences Paper on Hail Damage
- **File:** `AcademicPapers_Claude/4. geosciences-10-00500.pdf`
- **Source:** Geosciences, Vol. 10, No. 500
- **Type:** Peer-Reviewed Academic Paper
- **Relevance:** HIGH
- **Summary:** Covers hailstone impact mechanics including impact angle effects and damage variability based on material properties and environmental conditions.
- **Key Findings:** Impact angle, material properties, and environmental conditions all affect damage morphology. Damage patterns vary with hailstone size, speed, and angle.
- **Key Formulas:**
  - Terminal velocity: `vt = √(2·m·g / (A·Cd·ρa))`
  - Resultant velocity with wind: `vr = √(vw² + (vt + vd)²)` — proves angled impact
  - Multiple empirical velocity models: v = 9.9·D^0.38 (up to 8 cm); v = 14.04·D^0.5 (ASTM E822)
  - Air density: 1.341 kg/m³ at 0°C, 1.089 kg/m³ at 46.85°C — temperature affects fall speed

### A-5: Recent Study on Hail Impact on Building Envelopes
- **File:** `AcademicPapers_Claude/5. 1-s2.0-S2352710225004863-main.pdf`
- **Source:** Journal of Building Engineering (Elsevier, 2025)
- **Type:** Peer-Reviewed Academic Paper
- **Relevance:** HIGH
- **Summary:** Studies hail impact on building materials. Documents variable damage patterns including elongated marks from angled impacts and varied penetration depths.
- **Key Findings:** Hail damage to building materials varies with impact angle, speed, and material. Non-perpendicular impacts produce elongated damage marks.
- **Key Formulas:**
  - Kinetic Energy: `E = 0.5·m·v²`
  - Material properties: G300 steel yield stress = 320 MPa, elastic modulus = 200 GPa
  - Hailstone density: 917 kg/m³, Cd = 0.60

### A-7: ScienceDirect Articles Collection (Wind Engineering)
- **File:** `AcademicPapers_Claude/7. ScienceDirect_articles_22Mar2026_03-32-24.223/` (subfolder with multiple papers)
- **Source:** Journal of Wind Engineering & Industrial Aerodynamics (2024)
- **Type:** Peer-Reviewed Collection
- **Relevance:** CRITICAL (for Thunderstorm impact paper); MEDIUM (for others)
- **Key papers in this subfolder:**
  - **Thunderstorm-impact-on-the-built-environment** (Calotescu, Li, Mengistu & Repetto, 2024): Full-scale field survey of actual thunderstorm damage. 90% of hail damage on windward facade vs. <5% on leeward. Windward facades showed mostly circular indentations while OTHER orientations showed ELONGATED patterns. Damage intensity increased with height. Indentations 0.5-3.0 cm diameter. Key formulas: Wind velocity decomposition `v(t) = V̄(t) + v'(t)`; Turbulence intensity `Iu(t) = σv(t)/V̄(t)`; Hailstone kinetic energy scaling `Ek = a·D^b`; Terminal velocity `Vt = c·D^d`.
  - **Non-Gaussian-peak-factor-model-for-windward-walls** (Acosta, Wang & Kopp, 2024): Peak pressures on windward walls follow non-Gaussian distributions. Variation with height and turbulence intensity. Peak factor ratios 1.0-1.7x depending on building geometry. Key formulas: Peak factor `gp = (Cp − C̄p)/σC`; Non-Gaussian peak factors up to 1.7× Gaussian values; 77 wind tunnel model configurations; Generalized Pareto distribution for tail fitting.
  - **Parametric-effects-of-turbulence-on-flutter-stability** (Barni & Mannini, 2024): Large-scale atmospheric turbulence significantly affects aerodynamic behavior. Turbulent wind velocity fluctuations create non-uniform loading patterns.
  - **Editorial-Board**: Not relevant (journal editorial board listing).

### A-8: JCHE Paper — Hail Impact Resistance of Building Materials Testing, Evaluation and Classification
- **File:** `AcademicPapers_Claude/8. JCHE_03.01_05.pdf`
- **Source:** Journal of Civil and Hydraulic Engineering, Vol. 3, Issue 1
- **Type:** Peer-Reviewed Academic Paper
- **Relevance:** MEDIUM
- **Summary:** Laboratory testing of hail impact on construction materials. Documents impact energy transfer and damage mechanics at various angles and velocities. Establishes HIR (Hail Impact Resistance) classification system.
- **Key Findings:** Impact energy varies with angle and velocity. Damage morphology depends on impact conditions. Non-normal impacts produce directional damage.
- **Key Formulas:**
  - Terminal velocity: `vtH = √(4·dh·g·ρice / (3·cw·ρair))` (ρice = 875 kg/m³, cw = 0.5)
  - HIR Classification: Class 1 (10mm, 0.04J) through Class 5 (50mm, 27.0J)
  - Kinetic energy: `Ekin = m·v²/2`

### A-9: Nature Scientific Reports — Hail Impact Analysis (2022)
- **File:** `AcademicPapers_Claude/9. s41598-022-24375-3.pdf`
- **Source:** Scientific Reports / Nature (2022)
- **Type:** Peer-Reviewed Academic Paper
- **Relevance:** HIGH
- **Summary:** Analyzes hail impact mechanics and damage patterns with focus on variability based on hailstone properties and environmental conditions.
- **Key Findings:** Hailstone properties (shape, size, density) and environmental conditions (wind, angle) combine to produce variable damage patterns.
- **Key Formulas:**
  - Energy conservation: `E_impact = E_vibration + E_plastic + E_rebound`
  - Plastic energy: `E_plastic = π·D²·σf·t`
  - Dent depth: `D = √(α·(m·V²)/(2·t·σf) − β·(σf·π·φ⁴·l³)/(32·E·t³·h³))`
  - Flexural stiffness: `k = E·h³/l³`
  - Vibration energy: `E_vibration = F²/(2k)`
  - Ellipsoid surface area (Knud Thomsen): `Af = 4π·((ab)^p + (ac)^p + (bc)^p)/3)^(1/p)` where p = 1.6075
  - χ coefficient: `χ = 1.3923·(R/r)^0.6304` — shape-dependent material response

### A-10: Nature Scientific Reports — Hail Impact Analysis (2024)
- **File:** `AcademicPapers_Claude/10. 41598_2024_Article_69234.pdf`
- **Source:** Scientific Reports / Nature (2024)
- **Type:** Peer-Reviewed Academic Paper
- **Relevance:** HIGH
- **Summary:** Analyzes hail impact mechanics and damage patterns. Documents variability in damage based on hailstone properties and environmental conditions.
- **Key Findings:** Hailstone properties (shape, size, density) and environmental conditions (wind, angle) combine to produce variable damage patterns.
- **Key Formulas:**
  - **Turbulence impact force regression: `F = −0.624·Iu + 5116.25·D + 7.85·Vhail − 259.709`** (R² = 0.984)
  - ANOVA: Velocity F = 3917.064 (p < 0.0001), Diameter F = 3188.102 (p < 0.0001), Turbulence F = 382.569 (p < 0.0001)
  - Influence order: velocity > diameter > turbulence intensity
  - Turbulence intensity range tested: 2.5% to 25.5%

### A-CIB: Hail Impact Study (CIB13244)
- **File:** `AcademicPapers_Claude/Hail Impact - CIB13244.pdf`
- **Source:** CIB Publication
- **Type:** Academic/Industry Research
- **Relevance:** MEDIUM
- **Summary:** Study on hail impact testing and damage assessment methodology. Documents testing protocols and damage variability findings.
- **Key Findings:** Standardized testing shows variable damage outcomes. Impact conditions strongly influence damage morphology.
- **Key Formulas:**
  - Glass failure prediction: `ηp(Vf) = Kd/Kc − 1 ≥ 0` (Kd = dynamic stress intensity factor, Kc = fracture toughness = 0.75 ± 0.05 MPa·m^0.5)
  - Crack distribution (log-normal): `f(cd) = (1/(√(2π)·σc))·exp[−(1/2)·((ln(cd) − μc)/σc)²]`
  - Terminal velocity: `Vf = √(4·ρice·Ds / (3·ρair·CD))` (ρice = 870 kg/m³, CD = 0.6)
  - Glass properties: density 2500 kg/m³, E = 69 GPa, Poisson's = 0.22, pre-stress = 85 ± 5 MPa

---

## Speed Folder

### SP-1: Severe Weather 101: Hail Basics
- **File:** `Speed/1. Severe Weather 101_ Hail Basics.pdf`
- **Source:** NOAA National Severe Storms Laboratory
- **Type:** U.S. Government Authority
- **Relevance:** CRITICAL
- **Summary:** Official NOAA guide on hail. Horizontal winds cause hail to fall at angles or nearly sideways. Wind-driven hail breaks windows and tears siding. 3D-printed casts show natural hail falls slower than solid spheres due to irregular shape.
- **Key Findings:**
  - Hail falls at angles or nearly sideways due to wind
  - Fall speeds: Small (<1 in) 9-25 mph, Typical severe (1-1.75 in) 25-40 mph, Large (2-4 in) 44-72 mph, Very large (>4 in) 100+ mph
  - Real hailstones fall slower than spheres due to irregular shape (proven by 3D-printed cast experiments)
  - Wet growth creates bumpy/spiky appearances
  - Hailstones have "various sizes and shapes"

---

## HailData Folder

### HD-1: MRCC — Hail
- **File:** `HailData/MRCC - Hail.pdf`
- **Source:** Midwest Regional Climate Center / Purdue University / NOAA
- **Type:** Government / Academic Partnership
- **Relevance:** HIGH
- **Summary:** Comprehensive hail data resource. Wet growth creates bumpy/spiky hailstones. Windblown hail breaks windows and shreds siding. Baseball-sized hail reaches ~70 mph; larger reaches 100+ mph.
- **Key Findings:** Wet growth creates bumpy/spiky surfaces. Aggregated hailstones maintain individual shapes. Hail causes millions in window damage annually. Property damage exceeds $50 billion since 1949.

---

## HailDamageWindow Folder

### W-1: How Hail Damage to Windows Impacts Your Home's Energy Efficiency
- **File:** `HailDamageWindow/1. How Hail Damage to Windows Impacts Your Home's Energy Efficiency.pdf`
- **Source:** Industry / Educational
- **Type:** Industry Guide
- **Relevance:** MEDIUM
- **Summary:** Covers how hail damage to windows affects home energy performance. Documents various types of window damage from hail impact.
- **Key Findings:** Hail damage to windows includes cracks, chips, and frame damage. Damage varies by window type and impact conditions.

### W-2: Mastering Roof Inspections: Hail Damage, Part 10
- **File:** `HailDamageWindow/2. Mastering Roof Inspections_ Hail Damage, Part 10 - InterNACHI®.pdf`
- **Source:** InterNACHI (International Association of Certified Home Inspectors)
- **Type:** Professional Inspection Guide
- **Relevance:** CRITICAL
- **Summary:** Professional inspection guide documenting hail damage patterns to windows. Window screens show streaking. Aluminum-clad windows show indentations AND spatter marks. Damage includes cracks, indentations, spatter marks, and broken glass. States hail fall is random and won't leave identical marks.
- **Key Findings:**
  - Spatter marks (irregular, NOT circles) are legitimate hail damage
  - Different frame materials show different damage patterns
  - "Hail fall is random. It's not likely to leave marks of identical size, equal distances apart"
  - Vinyl frames crack; steel shows indentations and spatter
  - Window screens show streaking damage (elongated, not round) from even small hail
  - All windows can have broken glass in various patterns

---

## Insurer Documents (FarmersDocs Folder)

### INS-1: Farmers Insurance Denial Letter
- **File:** `FarmersDocs/FarmersDenyLetter-11-4.pdf`
- **Source:** Nicholas Brau, Claims Spec Rep Prop, Fire Insurance Exchange
- **Date:** November 4, 2024
- **Type:** Insurance Denial Letter
- **Summary:** Denies Claim #7007986837-1-1 (Policy #0980554965, Loss Date July 13, 2024) for property at 17756 George Moran Dr, Eden Prairie, MN 55347. Cites wear/tear based on attached Prieve Engineering report. References "Next Generation Homeowners Policy Minnesota, 2nd Ed." Policy provisions cited: Marring (definition 16), wear and tear (A.7, B.8), inherent vice (A.4, B.6), corrosion/deterioration (A.9, B.9), neglect (B.4), faulty construction (B.5).

### INS-2: Prieve Engineering Report (Appendix A)
- **File:** `FarmersDocs/FarmersDenyLetter-11-4-AppendixA.pdf`
- **Source:** Prieve Engineering LLC — Nathan E. Prieve, PE (License #46203)
- **Type:** Engineering Assessment (110 pages of photos)
- **Summary:** Four opinions forming basis of denial: (1) No recent hail damage since Aug 9, 2020; (2) Dents/scrape marks "not consistent with hail"; (3) Water leakage from condensation/aging; (4) East-side siding penetration unrelated to hail. All four opinions are rebutted by assembled scientific evidence — see RebuttalToFarmersDenial.md.

---

## Project Documents

### PROJ-1: Key Decision Document
- **File:** `KeyDecisionDocument.md`
- **Purpose:** Five counter-arguments to insurer's claim that hail damage is always round without scratches, with scientific formulas and complete formula reference appendix.

### PROJ-2: Rebuttal to Farmers Denial
- **File:** `RebuttalToFarmersDenial.md`
- **Purpose:** Point-by-point rebuttal to each of Prieve Engineering's four opinions, mapping specific research evidence to each claim.

### PROJ-3: Case Law Reference
- **File:** `../LegalReferences/CaseLawReference.md` *(moved from HailShapes/ to LegalReferences/ on 4/12/2026)*
- **Purpose:** Seven relevant court cases (CL-1 through CL-7) with analysis of relevance to our claim. Includes Burgess v. Farmers ($130M verdict), State Farm Hail Focus Initiative litigation, Dagley v. Haag Engineering, Cedar Bluff v. American Family (matching), Noonan v. American Family (matching endorsement), and others.

### PROJ-4: Legal Strategy
- **File:** `../LegalReferences/LegalStrategy.md` *(moved from HailShapes/ to LegalReferences/ on 4/12/2026)*
- **Purpose:** Litigation roadmap including legal claims (breach of contract, bad faith, unfair practices, matching/full replacement), evidence framework, timeline, and Minnesota-specific legal considerations.

---

## Quick Reference: Most Important Documents for Counter-Arguments

| Counter-Argument | Best Documents |
|---|---|
| Hailstones are NOT always round | S-6 (NOAA), S-9 (Lin et al. 2024), S-8 (Farnell et al. 2022), S-1 (Penn State/IBHS) |
| Wind causes angled, non-round damage | A-1 (Wind Speed Study), A-7/Thunderstorm (Calotescu 2024), SP-1 (NOAA Basics) |
| Scratches and non-circular marks are legitimate | A-7 (Glass Fragility), W-2 (InterNACHI) |
| Material properties create varied damage | W-2 (InterNACHI), A-3, A-4, A-5 |
| Field evidence of non-uniform damage | A-7/Thunderstorm (Calotescu 2024), S-5 (Storm Documentation) |

---

## Quick Reference: Litigation Document Map

| If You Need... | Go To |
|---|---|
| Summary of all 24 research papers | This file (DocumentIndex.md) |
| Scientific counter-arguments with formulas | KeyDecisionDocument.md (PROJ-1) |
| Point-by-point rebuttal of Prieve's 4 opinions | RebuttalToFarmersDenial.md (PROJ-2) |
| Court cases supporting our position | ../LegalReferences/CaseLawReference.md (PROJ-3) |
| Litigation roadmap and legal claims | ../LegalReferences/LegalStrategy.md (PROJ-4) |
| Original Farmers denial letter | FarmersDocs/FarmersDenyLetter-11-4.pdf (INS-1) |
| Prieve Engineering report + photos | FarmersDocs/FarmersDenyLetter-11-4-AppendixA.pdf (INS-2) |
