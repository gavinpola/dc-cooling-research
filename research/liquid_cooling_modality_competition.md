# Liquid Cooling Modality Competition: What Wins for Feynman (2028)?

**Research Date:** April 13, 2026

---

## The Real Question

The "liquid vs air" debate is settled—liquid wins. The real question is: **which liquid cooling modality dominates as TDP climbs toward 4-6kW per module?**

---

## 1. The TDP Trajectory

| Architecture | Year | TDP (Single) | TDP (Dual/Module) | Cooling Required |
|--------------|------|--------------|-------------------|------------------|
| Hopper (H100) | 2022 | 700W | - | Air or liquid |
| Blackwell (B200) | 2024 | ~1,000W | 1,200W | Liquid mandatory |
| Blackwell Ultra | 2025 | ~1,200W | 1,400W | Liquid mandatory |
| Rubin (R100) | 2026 | ~1,500W | 2,000-2,300W | Advanced liquid |
| **Feynman** | **2028** | **~2,000W+** | **4,400-6,000W** | **??? (this analysis)** |

**Key Insight:** Feynman introduces 3D logic die stacking—multiple GPU dies stacked on top of each other. This isn't just higher TDP; it's a fundamental thermal architecture challenge.

---

## 2. Liquid Cooling Modality Breakdown

### A. Single-Phase Direct-to-Chip (D2C)
**Current Leaders:** CoolIT, Asetek, Vertiv

**How it works:** Cold plate sits on chip, water circulates, heat transfers through thermal interface material (TIM).

| Metric | Value |
|--------|-------|
| Practical ceiling | ~1,500-2,000W |
| Flow rate for 1kW | ~1.5 L/min |
| Thermal resistance | 0.05-0.12 °C/W |

**Verdict for Feynman:** ❌ **NOT VIABLE** - Cannot handle 4-6kW modules

---

### B. Two-Phase Direct-to-Chip (D2C)
**Current Leaders:** ZutaCore, Accelsius

**How it works:** Coolant boils at chip surface, phase change absorbs more heat, vapor condenses in CDU.

| Metric | Value |
|--------|-------|
| Practical ceiling | ~3,000-4,000W |
| Flow rate for 1kW | ~0.3 L/min (5x less than single-phase) |
| Thermal resistance | 0.02-0.03 °C/W |

**Advantages:**
- 5x lower flow rates (less pump energy, less erosion)
- 50% better thermal resistance than single-phase
- More uniform temperature distribution

**Challenges:**
- PFAS regulatory risk (though HFO alternatives emerging)
- Higher initial cost
- More complex CDU

**Verdict for Feynman:** ⚠️ **MARGINAL** - Handles current Rubin, struggles with 6kW Feynman modules

---

### C. Immersion Cooling (Single-Phase)
**Current Leaders:** GRC, Submer, Asperitas

**How it works:** Entire server submerged in dielectric fluid.

| Metric | Value |
|--------|-------|
| Practical ceiling | ~50-100kW per tank |
| Heat flux handling | Lower than D2C |

**Advantages:**
- No PFAS concerns (hydrocarbon fluids)
- Simpler fluid handling
- Good for HPC workloads

**Challenges:**
- Operational complexity (hardware access)
- Lower heat flux capacity than D2C
- Tank-based constraints

**Verdict for Feynman:** ❌ **NOT VIABLE** - Heat flux too low for chip-level density

---

### D. Immersion Cooling (Two-Phase)
**Current Leaders:** LiquidStack (Trane)

**How it works:** Servers submerged, fluid boils directly off components.

| Metric | Value |
|--------|-------|
| Practical ceiling | ~250kW per tank |
| Operational complexity | Highest |

**Verdict for Feynman:** ⚠️ **POSSIBLE BUT COMPLEX** - Heat flux capability exists but operational challenges remain

---

### E. Microfluidic/Embedded Cooling ⭐ THE BREAKTHROUGH
**Current Leaders:** TSMC (IMC-Si), Microsoft Research, JetCool (Flex)

**How it works:** Microchannels etched directly into silicon backside, coolant flows within microns of transistors.

| Metric | Value |
|--------|-------|
| Demonstrated ceiling | 2,600W+ (TSMC) |
| Theoretical ceiling | 10kW+ |
| Thermal resistance | 0.01-0.02 °C/W (near zero TIM) |
| Flow rate | 2-3 L/min for 2kW |

**TSMC's Direct-to-Silicon Approach:**
- Micropillar arrays etched into silicon backside
- 3×3 compartmentalized microfluidic layout
- θJA as low as 0.055 °C/W at 40 ml/s
- **No thermal interface material (TIM)** - direct silicon-to-coolant contact

**Why This Wins for 3D Stacking:**
- Can cool **from the backside** of stacked dies
- Essential for Feynman's logic-on-logic stacking
- Integrated into TSMC's SoIC wafer-on-wafer bonding

**Verdict for Feynman:** ✅ **MOST LIKELY WINNER** - Only technology that addresses 3D stacking thermal challenge

---

## 3. The 2028 Prediction

### Most Likely Scenario (55%)

**Hybrid: Two-Phase D2C + Embedded Microfluidics**

- Two-phase D2C handles rack-level heat rejection
- Embedded microfluidics (TSMC's IMC-Si) handles chip-level heat extraction
- CDUs evolve to support both

**Why hybrid wins:**
1. Two-phase infrastructure already deploying at scale (2026-2027)
2. TSMC embeds microfluidics into packaging (manufacturing integration)
3. NVIDIA works with TSMC on custom packaging anyway
4. Economics favor leveraging both investments

### Alternative Scenario (30%)

**Pure Embedded Microfluidics (TSMC-led)**

- TSMC's direct-to-silicon becomes standard for all high-TDP chips
- Two-phase becomes "legacy" for 1-2kW devices
- Microfluidics handles 2-6kW+ modules

**Why this could happen:**
- TSMC controls 80% of advanced AI chip packaging
- Vertically integrated solution (foundry + packaging + cooling)
- Performance advantage is significant (3x better than cold plates)

### Unlikely Scenario (15%)

**Single-Phase Holds On**

- GPU efficiency improvements slow TDP growth
- Feynman delayed or uses chiplet approach to spread heat
- Single-phase + immersion handles most deployments

---

## 4. Investment Implications

### Thesis Update

| Modality | 2025-2027 | 2028+ (Feynman era) |
|----------|-----------|---------------------|
| Single-phase D2C | **Dominant** | Declining |
| Two-phase D2C | **Rising fast** | Stable (mid-density) |
| Immersion | Niche (HPC) | Niche |
| **Embedded/Microfluidic** | **Emerging** | **Dominant for high-end** |

### Who Wins

**Clear Winners:**
1. **TSMC** - Owns the manufacturing integration for embedded cooling
2. **JetCool (Flex)** - Microconvective technology, TSMC collaboration potential
3. **Two-phase D2C players (ZutaCore, Accelsius)** - Bridge technology through 2027

**Challenged:**
1. **Single-phase D2C (CoolIT, Asetek)** - Ceiling problem
2. **Pure immersion plays** - Wrong heat flux profile for AI

**Unknown:**
1. **Vertiv** - Has 70%+ GB200 share, but technology is single-phase focused
2. **NVIDIA's role** - May vertically integrate cooling if thermal becomes limiting

### Watch Signals

1. **TSMC packaging announcements** - IMC-Si commercialization timeline
2. **Microsoft deployments** - Their microfluidics research going to production
3. **Rubin cooling specs** - What NVIDIA requires for 2,300W modules
4. **JetCool-TSMC partnership** - Any formal collaboration
5. **ZutaCore/Accelsius non-PFAS fluid launch** - 2026 commitment

---

## 5. Sources

### NVIDIA Feynman Architecture
- [Tom's Hardware: Nvidia Enterprise GPU Roadmap](https://www.tomshardware.com/tech-industry/semiconductors/nvidia-enterprise-roadmap-rubin-rubin-ultra-feynman-and-silicon-photonics)
- [TweakTown: NVIDIA Feynman 2028](https://www.tweaktown.com/news/110521/nvidia-updates-roadmap-with-new-details-on-its-next-gen-gpu-feynman-coming-in-2028/index.html)
- [Igor's Lab: Feynman 3D Stacking Thermal Challenge](https://www.igorslab.de/en/starting-in-2028-nvidia-will-apparently-stack-true-logic-dies-in-feynman-for-the-first-time-turning-25d-into-a-thermal-tightrope-walk/)
- [Tom's Hardware: Future AI Processors 15,360W](https://www.tomshardware.com/pc-components/cooling/future-ai-processors-said-to-consume-up-to-15-360w-massive-power-draw-will-demand-exotic-immersion-and-embedded-cooling-tech)

### Two-Phase vs Single-Phase Performance
- [IDTechEx: Two-Phase Cold Plate Cooling 2026-2027](https://www.idtechex.com/en/research-article/two-phase-cold-plate-cooling-will-take-off-as-early-as-2026-2027/34068)
- [IDTechEx: Two-Phase Liquid Cooling Future of GPUs](https://www.idtechex.com/en/research-article/two-phase-liquid-cooling-the-future-of-high-end-gpus/33862)
- [Schneider Electric: Rise of Direct-to-Chip Cooling](https://blog.se.com/datacenter/2026/01/29/the-rise-direct-to-chip-cooling-top-ai-cooling-system/)

### Microfluidic/Embedded Cooling
- [Microsoft Source: Microfluidics Breakthrough](https://news.microsoft.com/source/features/innovation/microfluidics-liquid-cooling-ai-chips/)
- [Tom's Hardware: Microsoft Microfluidic Channels](https://www.tomshardware.com/pc-components/liquid-cooling/microsoft-develops-breakthrough-chip-cooling-method-microfluidic-channels-can-cut-peak-temps-by-up-to-65-percent-outperform-conventional-cold-plates-by-up-to-3x)
- [SemiWiki: TSMC Direct-to-Silicon Liquid Cooling](https://semiwiki.com/semiconductor-manufacturers/362017-breaking-the-thermal-wall-tsmc-demonstrates-direct-to-silicon-liquid-cooling-on-cowos/)
- [Tom's Hardware: Data Center Cooling State of Play 2025](https://www.tomshardware.com/pc-components/cooling/the-data-center-cooling-state-of-play-2025-liquid-cooling-is-on-the-rise-thermal-density-demands-skyrocket-in-ai-data-centers-and-tsmc-leads-with-direct-to-silicon-solutions)

### PFAS Alternatives
- [C&EN: Data Centers Take the Plunge](https://cen.acs.org/business/Data-centers-take-plunge/103/web/2025/08)
- [DCD: Chemours Opteon 2P50](https://www.datacenterdynamics.com/en/news/chemours-launches-two-phase-immersion-cooling-fluid/)
- [ZutaCore: Two-Phase DLC Not Immersion](https://blog.zutacore.com/zutacore-blog/two-phase-dlc-not-immersion-liquid-cooling)

---

## Document Metadata

**Purpose:** Analysis of intra-liquid-cooling competition for next-gen AI chips
**Companion to:** Data Center Cooling Investment Research
**Last Updated:** April 13, 2026
