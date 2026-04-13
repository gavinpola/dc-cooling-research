# Synthesis: Space-Based Passive Radiative Cooling

**Date:** April 13, 2026

---

## Thesis Statement

**Claim:** Passive radiative cooling to space could dramatically reduce or eliminate active mechanical cooling in data centers.

---

## Bull vs Bear Summary

| Dimension | Bull Argument | Bear Argument | Assessment |
|-----------|---------------|---------------|------------|
| **Physics** | Atmospheric window is real; cooling works | 150 W/m² ceiling is physics constraint | Bear wins - hard limits |
| **Scale** | Edge computing has smaller needs | 500-5,000x scale mismatch | Bear wins decisively |
| **Geography** | Works well in arid regions | Major DC markets are humid/cloudy | Bear wins on markets |
| **Economics** | Zero water, zero electricity | Land costs, marginal benefit | Bear wins on TCO |
| **Competition** | Complementary to liquid cooling | Liquid cooling already solved problem | Bear wins on alternatives |
| **Future Potential** | Early-stage, room to improve | Physics limits not bypassable | Bear wins on trajectory |
| **Edge Computing** | Viable at 10kW scale | Even edge has better options | Bear wins weakly |
| **Orbital** | Space computing needs it | Different constraints, no transfer | Bear wins on relevance |

**Overall:** Bear case is overwhelmingly stronger.

---

## Key Claims Assessment

### Bull Claims - Probability Assessment

| Claim | Probability | Rationale |
|-------|-------------|-----------|
| Radiative cooling physics work | **95%** | Proven at Stanford, SkyCool deployments |
| Can achieve 100 W/m² in ideal conditions | **80%** | Demonstrated repeatedly |
| 10-40% HVAC efficiency improvement | **70%** | SkyCool commercial results (for buildings) |
| Meaningful for edge computing | **25%** | Math barely works; better alternatives exist |
| Significant DC market impact by 2035 | **10%** | Scale mismatch is fundamental |
| Becomes standard DC component | **5%** | No path to solving core constraints |

### Bear Claims - Probability Assessment

| Claim | Probability | Rationale |
|-------|-------------|-----------|
| Scale mismatch prevents DC adoption | **95%** | 1,000 m² per 100kW rack is impractical |
| Humidity constraints limit geography | **90%** | Physics; observed in field tests |
| Liquid cooling is superior alternative | **95%** | Proven, deployed, works everywhere |
| No path to 10x performance improvement | **85%** | Physics constraints, not engineering |
| This remains building HVAC technology | **85%** | SkyCool's actual market |

---

## Critical Analysis

### The Fundamental Problem

**For a data center cooling technology to be viable:**
1. Must handle the heat load (kW)
2. Must fit in available space (m²)
3. Must work at the deployment location
4. Must be cost-competitive with alternatives

**Radiative cooling fails criteria 1, 2, and 3:**

| Criterion | Requirement | Radiative Cooling | Pass/Fail |
|-----------|-------------|-------------------|-----------|
| Heat load | 100+ kW/rack | ~100 W/m² (1,000x gap) | FAIL |
| Space | Fit on/near building | 1,000+ m²/rack | FAIL |
| Location | Work in major DC markets | Fails in humid climates | FAIL |
| Cost | Competitive with alternatives | Marginal benefit, high land cost | BORDERLINE |

### Where Radiative Cooling Has a Market

**Building HVAC augmentation:**
- Warehouses, commercial buildings
- Reduces envelope cooling load
- 21-65% savings demonstrated
- THIS IS A VALID MARKET

**But it's not data center cooling.**

### The Edge Computing Mirage

Bulls propose edge computing as viable use case.

**Analysis:**
- 10kW edge pod: 100 m² required
- Urban rooftops: Limited space, glare issues
- Grid-connected sites: $5,000 mini-split is competitor
- Off-grid remote: Possible niche, but tiny market

**Verdict:** Edge computing is not desperate enough for radiative cooling.

---

## Scoring Using Framework

| Dimension | Score | Weight | Weighted | Rationale |
|-----------|-------|--------|----------|-----------|
| Technical Feasibility | 2 | 20% | 0.40 | Works at small scale; fails at DC scale |
| Market Timing | 1 | 15% | 0.15 | Not commercially viable for DCs |
| Capital Efficiency | 1 | 15% | 0.15 | Land costs, marginal benefit |
| Operational Cost | 3 | 15% | 0.45 | Zero water/electricity is real benefit |
| Scalability | 1 | 15% | 0.15 | Fundamentally unscalable to DC needs |
| Competitive Moat | 2 | 10% | 0.20 | SkyCool has IP but limited DC relevance |
| Risk Profile | 2 | 10% | 0.20 | Low technical risk; high market risk |

**Weighted Score: 1.70 / 5.00**

**Interpretation:** Avoid for data center investment thesis.

---

## Realistic Scenarios

### Most Likely Outcome (70% probability)

**Radiative cooling remains a building HVAC technology:**
- SkyCool grows in warehouse/commercial market
- Never achieves meaningful DC adoption
- Occasionally integrated into modular/edge builds
- Remains <0.1% of DC cooling market

### Modest Success Scenario (25% probability)

**Becomes niche component:**
- Standard feature in Nordic/desert DC designs
- 10-15% of new DC builds include some radiative panels
- Provides 3-5% of total cooling in installations where used
- Achieves $500M-1B market size by 2035

### Bull Case Scenario (5% probability)

**Breakthrough changes game:**
- Material advance achieves 500+ W/m² sustained
- Hybrid systems become standard
- Achieves $5B+ market size by 2035
- Becomes meaningful layer in cooling stack

---

## Investment Implications

### Direct Exposure: Not Recommended

**SkyCool Systems:**
- Valid company, wrong market for DC thesis
- Building HVAC is their actual opportunity
- No disclosed DC deployments or customers

### Indirect Exposure: Neutral

**Companies that might benefit:**
- Modular DC providers (if they integrate)
- Edge infrastructure players
- Building materials companies

**But:** Exposure would be tiny portion of their business

### Recommended Position: None

**For DC cooling investment:**
- Focus on liquid cooling (Thesis A)
- Monitor for breakthrough announcements
- Don't allocate capital based on current state

---

## Signposts to Monitor

### Would Change Assessment to Positive

1. **Hyperscaler pilot announcement** - Meta/Google/AWS tests radiative cooling
2. **10x performance breakthrough** - >1,000 W/m² demonstrated
3. **Humidity solution** - Works in Singapore/Hong Kong demonstrated
4. **SkyCool DC customer** - Signed deal with DC operator

### Would Confirm Negative Assessment

1. **SkyCool pivots away from DCs** - Focuses entirely on building HVAC
2. **5+ years with no DC deployment** - Current status continues
3. **Competing liquid cooling advances** - Makes radiative even less relevant

---

## Final Verdict

### Assessment Summary

**Radiative cooling for data centers is:**
- Theoretically interesting
- Practically impractical
- Solving the wrong problem
- Not investable as DC thesis

**The core issue is simple:**
- Data centers need to dissipate 100+ kW per rack
- Radiative cooling delivers ~100 W/m²
- The gap is 500-5,000x
- No proposed mechanism bridges this gap

### Thesis Score and Recommendation

**Score: 1.70 / 5.00** - Avoid

**Recommendation:**
- Do NOT invest based on radiative cooling for DC thesis
- Monitor for breakthrough announcements (unlikely)
- If building HVAC exposure desired, SkyCool may be valid
- Liquid cooling (Thesis A) is the actual opportunity

**Confidence Level:** 90%

This is one of the clearest "no" verdicts in the analysis. The physics constraints are fundamental, not engineering problems. The scale mismatch is not closable with foreseeable technology. The market opportunity is in building HVAC, not data center cooling.

**Final Word:** Interesting science does not equal investable opportunity. Radiative cooling is the former, not the latter.
