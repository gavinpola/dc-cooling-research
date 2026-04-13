# Bear Case: Space-Based Passive Radiative Cooling Is Impractical

**Thesis:** Passive radiative cooling to space is fundamentally unsuited for data center applications due to insurmountable scale, geographic, and economic constraints.

**Date:** April 13, 2026

---

## Executive Summary

The bear case against radiative cooling for data centers is simple: **the math doesn't work.**

1. **500-5,000x scale mismatch** - 100 W/m² vs 100+ kW/rack
2. **Geographic constraints eliminate most markets** - Fails in humid, cloudy regions
3. **No path to required performance** - Physics limits cooling power
4. **Competing with superior alternatives** - Liquid cooling solves the actual problem
5. **It's a building technology, not a DC technology** - HVAC augmentation is not transformative

This is a science project, not a data center solution.

---

## 1. The Scale Mismatch Is Fatal

### The Math Is Devastating

**Radiative cooling capacity:** ~100 W/m² (optimistic)
**AI rack requirement:** 100-500 kW

**For a single 100kW AI rack:**
- Required panel area: **1,000 m²** (quarter acre)
- That's a 32m × 32m area
- For ONE rack

**For a 10MW AI data center:**
- Required panel area: **100,000 m²** (25 acres)
- That's 10 hectares of continuous panel surface
- Plus building footprint, access, etc.
- Total land requirement: 30+ acres minimum

### Land Cost Comparison

**Option A: Liquid cooling**
- Data center footprint: 50,000 sq ft (typical 10MW)
- Land requirement: 2-3 acres total

**Option B: Radiative cooling**
- Panel requirement: 100,000 m² = 1,000,000+ sq ft
- Land requirement: 25-30 acres minimum
- 10x the land footprint

**At $1M/acre (suburban):** $25-30M extra just for land.

### Even With Improvements, Math Fails

**Best-case future scenario:**
- Radiative cooling achieves 500 W/m² (3x current)
- 100kW rack still needs 200 m² (tennis court)
- 10MW data center still needs 20,000 m² (5 acres of panels)

**The fundamental issue:** Radiative cooling is a surface-area technology trying to solve a volume-density problem.

---

## 2. Geographic Constraints Eliminate Most Markets

### Where Data Centers Are vs Where Radiative Works

**Where radiative cooling works:**
- Arid deserts (low humidity, clear skies)
- High-altitude plateaus
- Remote areas with low water vapor

**Where data centers are:**
- Northern Virginia (humid)
- Silicon Valley (mild, but not arid)
- Singapore (tropical - fails completely)
- London (cloudy)
- Dublin (cloudy)
- Hong Kong (humid - 25 W/m² vs 61 W/m² in dry climate)

### The Numbers

**Performance by location:**
| Location | Radiative Cooling | Data Center Market |
|----------|-------------------|-------------------|
| Phoenix | Good | Small market |
| Stanford | 61 W/m² | Medium market |
| Hong Kong | 25 W/m² | Large market |
| Singapore | Near zero | Critical hub |
| Frankfurt | Cloudy/humid | Major hub |

**The Paradox:** The regions best for radiative cooling have small data center markets. The major data center markets are unsuitable for radiative cooling.

### Humidity Kills Performance

**Hong Kong field tests:**
- Maximum nighttime cooling: Only 38 W/m²
- Daytime: **NO OBSERVED COOLING EFFECT**

**Tropical testing (Okayama, Japan):**
- Devices reached **2.8°C ABOVE ambient** during day
- Net heat gain, not cooling

If your "cooling" technology adds heat in humid climates, it's not a cooling technology.

---

## 3. Physics Limits Are Hard Caps

### The 150 W/m² Ceiling

**Why 150 W/m² is approximately the limit:**
- Atmospheric transparency window has finite bandwidth
- Radiative heat transfer governed by Stefan-Boltzmann law
- Temperature differential to space is fixed
- These are physics constraints, not engineering problems

### No Moore's Law for Radiative Cooling

**Unlike semiconductor cooling which improves with:**
- Better materials
- Smaller channels
- Higher pressures
- More exotic fluids

**Radiative cooling is constrained by:**
- Atmospheric physics (fixed)
- Stefan-Boltzmann constant (fixed)
- Surface temperature (constrained by use case)
- Sky temperature (fixed at ~3K)

**You cannot innovate around the laws of thermodynamics.**

### The 710 W/m² Claim Is Misleading

One study achieved 710 W/m² by combining radiative AND evaporative cooling.

**Problem:** The evaporative component uses water. At that point, just use evaporative cooling directly (it's simpler and proven).

---

## 4. Liquid Cooling Already Solved the Problem

### Direct Competition

**The problem:** Cooling high-density AI racks (100kW+)

**Liquid cooling solution:**
- Direct-to-chip: Handles 250kW+ per rack
- Proven, shipping, hyperscaler-adopted
- Works in ANY climate
- Works in ANY location

**Radiative cooling "solution":**
- Requires 1,000+ m² per rack
- Only works in arid climates
- Not adopted by any hyperscaler for IT cooling
- Adds complexity without solving the core problem

### Cost Comparison

**Liquid cooling for 100kW rack:**
- System cost: $50,000-100,000
- Footprint: Standard 42U rack
- Any location: Yes

**Radiative cooling for 100kW rack (if possible):**
- Panel cost: Unknown but significant
- Land cost: 1,000 m² × $X/m²
- Only works in: Desert locations
- Actually achievable: No

### Hyperscaler Adoption

**Liquid cooling:**
- Meta: Deploying at scale
- Microsoft: Azure AI clusters
- Google: TPU deployments
- AWS: Fairwater AI campuses

**Radiative cooling:**
- Meta: None disclosed
- Microsoft: None disclosed
- Google: None disclosed
- AWS: None disclosed

The market has spoken.

---

## 5. Edge Computing Argument Is Weak

### The Bull Case for Edge

Bulls argue radiative cooling could work for edge computing:
- Smaller scale (10kW)
- "Only" 100 m² needed

### The Reality

**10kW edge pod:**
- Typical footprint: Shipping container (~30 m²)
- Required panel area: 100 m² (3x the pod)
- Roof installation: 10m × 10m

**Problems:**
1. Edge pods are often in urban areas (building rooftops)
2. Urban areas are heat islands (reduced performance)
3. Glare from reflective panels creates liability
4. Maintenance access to 100m² of panels adds cost
5. Most edge locations have grid power - just use a small chiller

**The competitor:** A $5,000 mini-split AC unit.

### Edge Market Isn't Desperate

Edge computing operators have options:
- Small chillers work fine at 10kW scale
- Air cooling is adequate for many edge workloads
- Liquid cooling is available for high-density edge

Radiative cooling solves a problem that doesn't exist at edge scale.

---

## 6. Building HVAC ≠ IT Cooling

### What SkyCool Actually Does

**SkyCool's market:** Building HVAC augmentation
**SkyCool's claim:** 10-40% improvement in HVAC efficiency

**Translation:**
- Reduces building envelope cooling load
- Does NOT cool IT equipment directly
- Is an HVAC optimization, not a DC cooling solution

### The Distinction Matters

**Building HVAC:**
- Comfortable human temperatures (20-25°C)
- Modest heat loads (W per square meter of floor)
- Can be augmented by marginal improvements

**IT Equipment Cooling:**
- Precise temperature control required
- Massive heat loads (kW per square meter)
- Requires purpose-built cooling solutions

A 20% reduction in building HVAC doesn't help when IT generates 40x more heat than the building envelope.

---

## 7. Economic Analysis Is Unfavorable

### SkyCool ROI Claims

**As an HVAC add-on:** 10-40% efficiency improvement

**For a data center:**
- Building HVAC is ~5-10% of total cooling load
- IT cooling is ~90-95% of total cooling load
- 30% improvement on 10% of load = 3% total improvement
- Not transformative

### Opportunity Cost

**Capital spent on radiative cooling:**
- Panels, installation, land
- Maintenance and cleaning
- Integration systems

**Same capital spent on liquid cooling:**
- Directly addresses the cooling problem
- Works in any location
- Proven ROI models

### The Marginal Utility Problem

If you've already invested in:
1. Liquid cooling (handles IT load)
2. Economizers (handles heat rejection)
3. High ambient tolerance (handles building HVAC)

...what problem does radiative cooling solve that isn't already addressed?

---

## 8. Orbital Computing Is a Red Herring

### The Bull's Space Argument

"Orbital computing will drive radiative cooling R&D that transfers to terrestrial."

### The Reality

**Orbital cooling constraints:**
- No atmosphere (no humidity problem)
- No clouds (no variability)
- No air convection (different physics)
- Vacuum environment (different materials)

**Terrestrial constraints:**
- Atmosphere present
- Humidity variable
- Clouds common
- Convection exists

**Technology transfer is limited** because the constraints are fundamentally different.

### Orbital Scale Is Tiny

**SpaceX "1 million satellites":**
- Aspirational, not approved
- Each satellite: Maybe 1-10kW compute
- Total: 1-10 GW (maybe, eventually)

**Terrestrial data centers:**
- Already 300+ GW globally
- Growing 10%+ annually
- Orbital is a rounding error

---

## 9. What Would Need to Be True for Bears to Be Wrong

### Required Breakthroughs

1. **10x cooling power improvement** - From 100 W/m² to 1,000 W/m²
   - No known path to this
   - Would require different physics

2. **Works in humid climates** - Solve the water vapor absorption problem
   - This IS an atmospheric physics constraint
   - Not obviously solvable

3. **Dramatic cost reduction** - 90%+ cheaper than today
   - Materials are already commodity-scale
   - Land costs aren't reducible

4. **Integration that works at IT level** - Cool racks, not buildings
   - Requires solving the scale problem
   - No proposed mechanism

### Probability Assessment

| Required Breakthrough | Probability by 2035 |
|----------------------|---------------------|
| 10x cooling power | <5% |
| Humidity solution | <10% |
| 90% cost reduction | ~20% |
| IT-level integration | <5% |
| ALL of the above | <1% |

---

## 10. Conclusion: Science Project, Not Solution

### Honest Assessment

**Radiative cooling is:**
- Interesting physics
- Proven for HVAC augmentation
- Potentially useful for buildings
- A small market opportunity

**Radiative cooling is NOT:**
- A data center cooling solution
- Scalable to IT workloads
- Competitive with liquid cooling
- Geographically universal
- Investable as a DC thesis

### Investment Recommendation

**Avoid exposure to radiative cooling as a data center thesis.**

- The scale mismatch is fundamental
- Geographic constraints eliminate major markets
- Liquid cooling already solved the problem
- There's no investment thesis beyond speculative R&D

**If you want building HVAC exposure:** SkyCool has a valid market, but it's not data center cooling.

**If you want data center cooling exposure:** Invest in liquid cooling companies with proven hyperscaler deployments.

### Final Verdict

**Score: 1.5 / 5.0** - Avoid

This is a technology looking for a problem that doesn't exist at the scale where data centers operate. The bulls are conflating "interesting science" with "investable opportunity."

The bear case is simple: **you can't fight physics, and the physics don't work for data centers.**
