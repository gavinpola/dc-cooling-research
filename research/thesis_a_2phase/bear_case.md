# Bear Case: 2-Phase Direct-to-Chip Cooling May NOT Dominate

**Thesis:** 2-phase direct-to-chip liquid cooling will NOT become the dominant cooling approach for data centers, even for AI workloads.

**Date:** April 13, 2026

---

## Executive Summary

While 2-phase cooling has technical merits, multiple converging forces may prevent it from achieving market dominance:

1. **Single-phase liquid cooling is "good enough"** and scaling rapidly
2. **PFAS regulatory risk** threatens the entire fluorocarbon fluid ecosystem
3. **Operational complexity** creates adoption resistance
4. **Supply chain concentration** creates dangerous dependencies
5. **The market is bifurcating** - not consolidating around two-phase

The bulls are conflating "liquid cooling wins" with "two-phase wins." These are not the same claim. Single-phase direct-to-chip and single-phase immersion may capture the market while two-phase remains a niche.

---

## 1. Single-Phase Is Already Good Enough

### Performance Gap Is Narrowing

**Microchannel Single-Phase Catches Up:**
- Advanced single-phase systems with microchannels achieve **15,000 W/m²·K** heat transfer coefficients
- CoolIT Systems: **0.015°C/W thermal resistance** - matching or exceeding some two-phase claims
- 300 H100 GPUs maintained at **62°C junction temps** using single-phase with 25°C inlet water

**The 15,000 W/m²·K Threshold:**
- Most AI GPUs don't need the theoretical maximum of two-phase (23,000+ W/m²·K)
- H100 at 700W is being cooled effectively with single-phase today
- Even Blackwell at 1,200W is being handled by enhanced single-phase designs

### Hyperscalers Are Deploying Single-Phase

**The Reality of Current Deployments:**
- AWS Fairwater: **Single-phase** closed-loop liquid cooling
- CoolIT holds significant share of GB200 cooling alongside Vertiv
- Most "liquid-cooled" deployments today are single-phase, not two-phase

**Quote from Industry:**
> "Most liquid-cooled capacity in use today is single-phase direct liquid cooling. Use of two-phase direct liquid cooling likely to grow gradually." - Motivair/Schneider Electric

### Simpler Operations = Faster Adoption

**Single-Phase Advantages:**
- No phase-change dynamics to manage
- No vapor handling systems required
- Simpler leak detection (liquid-only, no vapor)
- Well-understood fluid dynamics
- Lower-skilled technician requirements
- Standard plumbing practices apply

**Data Center Operators Are Conservative:**
- Colocation providers prefer proven, simple systems
- Enterprise IT departments lack liquid cooling expertise
- Single-phase represents a smaller leap from air cooling

---

## 2. PFAS Regulatory Risk Is Existential

### 3M Exit Was Just the Beginning

**Timeline of Regulatory Pressure:**
- January 2025: 3M ceased Novec 7500 production
- End of 2025: 3M exits ALL PFAS production
- EU PFAS restriction proposal advancing
- US EPA PFAS regulations tightening

**What Is PFAS:**
- Per- and polyfluoroalkyl substances ("forever chemicals")
- Includes fluorocarbons used in two-phase cooling
- Associated with environmental and health concerns
- Regulatory scrutiny accelerating globally

### The Alternatives Have Problems

**HFO Refrigerants (R-1234ze, etc.):**
- Marketed as non-PFAS, but regulatory definitions evolving
- Lower GWP doesn't mean zero environmental impact
- Supply chains not yet scaled
- Performance characteristics differ from Novec

**BestSolv "Similar Molecules":**
- Claimed to be "NOT classified as PFAS under proposed EPA definition"
- Key word: "proposed" - definitions can change
- Regulatory uncertainty creates business risk

**The Cost Reality:**
- Fluorocarbon fluids cost **an order of magnitude more** than hydrocarbon single-phase fluids
- Two-phase fluids must be "regularly replenished at hundreds of dollars per gallon"
- Regulatory uncertainty adds risk premium

### Single-Phase Escapes This Risk Entirely

**Hydrocarbon-Based Single-Phase Fluids:**
- ElectroSafe (GRC) and similar: No PFAS concerns
- Multiple global suppliers (no single-vendor risk)
- Non-volatile, reclaimable fluids
- Established supply chains
- Lower regulatory scrutiny

**Strategic Implication:**
Any enterprise CFO comparing "proven single-phase with no regulatory risk" vs "better-performing two-phase with PFAS uncertainty" may choose de-risking over optimization.

---

## 3. Operational Complexity Creates Barriers

### Phase Change Is Harder to Control

**Two-Phase System Challenges:**
- Must manage liquid-vapor equilibrium
- Pressure fluctuations during load changes
- Potential for vapor lock in cold plates
- Condensation management at HRU
- More complex control systems

**The Orientation Problem:**
> "Unlike passive thermosiphon systems that require condensers above evaporators..."

Even "pumped two-phase" requires careful system design. Single-phase works in any orientation with simpler considerations.

### Leak Consequences Differ

**Single-Phase Leak:**
- Liquid pooling - visible, containable
- Standard liquid detection works
- Clean-up relatively straightforward

**Two-Phase Leak:**
- Both liquid and vapor escape
- Vapor can spread further, harder to detect
- Some fluids are heavier than air (accumulate in pits/trenches)
- Potential for rapid evaporation = rapid fluid loss

### Maintenance Complexity

**Two-Phase Requirements:**
- Specialized technician training for phase-change systems
- More sophisticated monitoring equipment
- Tighter tolerances on system pressures
- Refrigerant handling certifications potentially required

**Industry Reality:**
Most data center technicians are trained for electrical and air-handling systems. The labor pool for liquid cooling expertise is already constrained - two-phase adds another layer.

---

## 4. Supply Chain Is Dangerously Concentrated

### Vendor Lock-In Risk

**The Bulls' Own Evidence:**
- Vertiv holds **70%+ of volume share** for GB200 racks
- "Remaining share largely shared by Motivair and CoolIT"

This concentration is presented as "industry direction" by bulls. Bears see it as **single point of failure risk**.

### Two-Phase Vendor Ecosystem Is Thin

**Pure-Play Two-Phase Companies:**
- ZutaCore (private, no disclosed funding)
- Accelsius (2022 founding, Johnson Controls investment)
- LiquidStack (SoftBank-backed, Series C 2026)

**Compare to Single-Phase Ecosystem:**
- CoolIT Systems (established, multiple customers)
- Asetek (public company, diversified)
- Multiple hydrocarbon fluid suppliers
- Standard plumbing component suppliers

### 3M Exit Demonstrated Supply Chain Fragility

When 3M announced PFAS exit:
- Entire two-phase immersion segment scrambled for alternatives
- Customer confidence shaken
- Highlighted dependency on single chemical supplier

**Lesson:** Two-phase cooling depends on narrow chemical supply chains. Enterprise procurement officers are trained to avoid such dependencies.

---

## 5. The Market Is Bifurcating, Not Consolidating

### Three Viable Architectures Coexist

**1. Single-Phase Direct-to-Chip (DTC):**
- CoolIT, JetCool/Flex, Asetek
- Water or water-glycol based
- Hyperscaler adoption proven
- Retrofit-friendly

**2. Single-Phase Immersion:**
- GRC, Submer, Asperitas
- Hydrocarbon dielectric fluids
- Tank-based, good for HPC
- No PFAS concerns

**3. Two-Phase (DTC or Immersion):**
- ZutaCore, Accelsius, LiquidStack
- Fluorocarbon or refrigerant-based
- Highest performance ceiling
- Highest regulatory/operational risk

### Each Has Its Market Segment

**Single-Phase DTC:**
- Enterprise AI deployments
- Colocation providers
- Retrofit applications
- Conservative operators

**Single-Phase Immersion:**
- HPC clusters
- Crypto mining (where operational)
- Edge deployments
- Sustainability-focused operators

**Two-Phase:**
- Bleeding-edge AI training
- Hyperscaler R&D
- Extreme density requirements (500kW+ racks)
- Operators with specialized expertise

### "Dominant" Is Not "Only"

The bulls claim two-phase will "dominate." But even their evidence shows:
- Multiple technologies coexisting
- Different solutions for different use cases
- No single technology taking >50% of all cooling

---

## 6. Economic Arguments Have Caveats

### TCO Models Have Assumptions

**The Bull's $111M Savings Claim:**
Based on 10MW data center, 10-year horizon, comparing immersion to air cooling.

**Problems:**
1. Compares to **air cooling**, not single-phase liquid
2. Immersion (two-phase) vs direct-to-chip economics differ
3. Doesn't include regulatory compliance costs
4. Doesn't include specialized labor premium
5. Doesn't include fluid replacement costs at scale

### Fluid Costs Scale Non-Linearly

**Two-Phase Fluid Economics:**
- 4 gallons per 100kW rack (bull's number)
- "Hundreds of dollars per gallon" for replenishment
- Large deployment (10MW = 100 racks): 400+ gallons
- Annual replenishment costs can be significant
- Regulatory-driven fluid changes = stranded inventory

**Single-Phase Comparison:**
- Higher initial volume (100+ gallons per rack)
- But: **Non-volatile** = minimal replenishment
- **Reclaimable** = fluid assets not consumables
- Multiple suppliers = competitive pricing

### PUE Comparisons Cherry-Pick

**Bulls cite PUE of 1.02 (BitFury Tbilisi):**
- This is an outlier, not a baseline
- Achieved with immersion in cold climate
- Not representative of typical deployments

**Realistic PUE Ranges:**
- Well-designed single-phase DTC: **1.10-1.20**
- Two-phase DTC: **1.05-1.15**
- Difference: **5-10%**, not transformative

Is 5% efficiency worth PFAS risk, operational complexity, and supply chain concentration?

---

## 7. The AI Density Argument Has Limits

### Most Data Centers Don't Need 250kW Racks

**Current Reality:**
- Average enterprise rack: **8-15kW**
- High-density colocation: **20-40kW**
- AI training clusters: **80-120kW**

**Only hyperscaler AI training** pushes 120-250kW+ densities. This is a small (though growing) segment of total data center capacity.

### Hyperscalers Build Custom, Not Buy Standard

**Google, Meta, Microsoft Reality:**
- Design custom cooling solutions in-house
- Don't buy "off-the-shelf" from Vertiv
- May use two-phase OR single-phase based on facility
- Aren't loyal to cooling technology vendors

**Implication:** Hyperscaler "adoption" doesn't create standard market. They're not buying from the same vendors enterprises will use.

### GPU TDP Trajectory May Flatten

**Moore's Law Considerations:**
- Chip efficiency improving alongside TDP growth
- Not all AI advances require higher wattage
- Inference workloads (larger market) use lower power than training
- Next-gen architectures may prioritize efficiency

The assumption of "ever-increasing TDP" may not hold. If GPUs plateau at 1-2kW, single-phase remains viable.

---

## 8. Historical Precedents Suggest Caution

### "Inevitable" Technologies That Didn't Dominate

**Solid State Drives (SSDs) vs HDDs:**
- SSDs are "technically superior" in every way
- 15+ years later: HDDs still huge market for cold storage
- Coexistence, not replacement

**Fiber to the Home:**
- "Inevitable" since 1990s
- 30 years later: copper DSL still in use globally
- Last mile economics created coexistence

### Two-Phase Has Been "The Future" for a Decade

**Allied Control** (BitFury predecessor):
- Demonstrated PUE 1.02 in **2015**
- Microsoft tested at same time
- 10+ years later: still "emerging"

**Why So Slow?**
- Operational complexity
- Fluid costs and availability
- Lack of standardization
- Risk-averse enterprise market

---

## 9. What Would Need to Be True for Bears to Win

### Signposts to Watch

**1. Single-Phase Continues to Scale:**
- CoolIT, JetCool achieving 150kW+ racks with single-phase
- Microchannel improvements close performance gap
- Enterprises standardize on single-phase DTC

**2. PFAS Regulations Tighten:**
- EU PFAS ban includes data center fluids
- US EPA broadens PFAS definitions
- Two-phase fluid suppliers face constraints

**3. Market Remains Fragmented:**
- No single cooling technology exceeds 40% share by 2030
- Different solutions for different use cases persist
- Two-phase remains HPC/hyperscaler niche

**4. GPU TDP Growth Slows:**
- Next-gen GPUs focus on efficiency
- 1.5-2kW becomes standard ceiling
- Single-phase handles without extreme measures

**5. Operational Complexity Proves Costly:**
- Two-phase deployments experience higher incident rates
- Specialized labor costs exceed efficiency savings
- Enterprises choose "good enough" over "optimal"

---

## 10. Conclusion: Two-Phase Will Be Important, Not Dominant

### The Realistic Scenario

**By 2030:**
- Total liquid cooling market: **$30-40B**
- Two-phase (DTC + immersion): **15-25%** of liquid cooling
- Single-phase DTC: **40-50%** of liquid cooling
- Single-phase immersion: **15-20%** of liquid cooling
- Hybrid/other: **10-20%**

**Two-phase wins:**
- Bleeding-edge AI training
- Extreme density (250kW+ racks)
- Operators with specialized expertise
- Where efficiency optimization is existential

**Single-phase wins:**
- Enterprise AI deployments
- Retrofit applications
- Risk-averse operators
- Regulatory-constrained markets

### The Bear's Verdict

Two-phase direct-to-chip is a **superior technology** that will capture a **significant niche** but will NOT achieve market dominance because:

1. Single-phase is "good enough" for 80% of use cases
2. PFAS regulatory risk creates existential uncertainty
3. Operational complexity limits adoption beyond specialists
4. Supply chain concentration creates enterprise risk
5. The market will bifurcate across multiple solutions

**Invest in liquid cooling broadly. Don't bet the farm on two-phase specifically.**
