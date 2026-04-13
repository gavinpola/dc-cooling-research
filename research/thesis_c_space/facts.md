# Thesis C: Space-Based Passive Radiative Cooling - Research Facts

**Research Date:** April 13, 2026
**Thesis:** Passive radiative cooling to space could dramatically reduce or eliminate active mechanical cooling in data centers.

---

## 1. How Radiative Cooling Works

### The Atmospheric Transparency Window

The Earth's atmosphere has a "transparency window" between **8-13 micrometers (μm)** where atmospheric absorption is negligible. Thermal radiation at these wavelengths passes directly through to space without heating the surrounding air.

- Space temperature: ~3K (-270°C)
- This creates a massive temperature differential that can be exploited for passive heat rejection
- The sky functions as a radiative heat sink

**Sources:**
- [Stanford University School of Engineering](https://engineering.stanford.edu/news/how-new-cooling-system-works-without-using-any-electricity)
- [PMC - Radiative Cooling Principles](https://pmc.ncbi.nlm.nih.gov/articles/PMC5067572/)

### The Technology

**Stanford/SkyCool Systems Approach:**
- Panels made of thin layer of silver covered by layers of silicon dioxide and hafnium oxide
- Emits heat at infrared wavelengths between 8-13 micrometers
- Reflects ~97% of sunlight while emitting thermal energy through atmospheric window
- Can achieve sub-ambient cooling even during daytime

**Key Quote:**
> "With this technology, we're no longer limited by what the air temperature is, we're limited by something much colder: the sky and space." - Eli Goldstein, Stanford

**Source:** [Stanford Report](https://news.stanford.edu/stories/2017/09/sending-excess-heat-sky)

---

## 2. Heat Rejection Performance

### Cooling Power (W/m²)

| Configuration | Cooling Power | Conditions |
|---------------|---------------|------------|
| Theoretical maximum | ~150 W/m² | Dry, clear sky, ambient temp |
| Typical daytime | 40-100 W/m² | Direct sunlight |
| Nighttime | 65 W/m² | Clear sky |
| Humid climate (Hong Kong) | 25 W/m² | High humidity |
| Arid climate (Stanford) | 61 W/m² | Low humidity |
| Worst case (cloudy) | 14-44 W/m² | Depending on cloud height |

**Key Findings:**
- Average PDRC (Passive Daytime Radiative Cooling) system: **100-150 W/m²** theoretical
- Real-world performance varies dramatically by climate
- Humid climates see 50-70% reduction in performance

**Sources:**
- [ScienceDirect - Passive daytime radiative cooling](https://www.sciencedirect.com/science/article/pii/S2949821X24000267)
- [Wikipedia - Passive daytime radiative cooling](https://en.wikipedia.org/wiki/Passive_daytime_radiative_cooling)

### Sub-Ambient Temperature Achievement

- Dual-selective radiative cooling: ~9°C below ambient under strong sunlight
- Best conditions (arid): Up to 20.6°C below ambient
- Typical daytime: 4-6°C below ambient
- No cooling or above ambient possible in hot, humid conditions

**Source:** [Springer Nature Communities](https://communities.springernature.com/posts/enhanced-radiative-cooling-by-using-an-additional-atmospheric-transparency-window)

---

## 3. Key Companies and Research

### SkyCool Systems (Stanford Spinout)

**Founded:** By Fan, Goldstein, and Raman from Stanford
**Technology:** Passive Daytime Radiative Cooling panels
**Products:** Panels that integrate with HVAC and refrigeration systems

**Performance Claims:**
- As add-on to existing systems: 10-40% efficiency improvement
- Full replacement of AC: 80-90% energy reduction potential
- Testing locations: California, Florida, Indiana, Kansas, Nevada, Texas

**Applications:** Building HVAC augmentation, not direct data center cooling

**Source:** [SkyCool Systems](https://www.skycoolsystems.com/)

### Academic Research Centers

- **Stanford University:** Original technology development
- **UC Davis HoMEDUCS Project:** Integration with modular data centers
- **University of Colorado Boulder:** Polymer-based radiative coolers

### Orbital Data Centers (2026 Development)

**Space-based computing** is utilizing radiative cooling by necessity:

- **Starcloud:** Launched first NVIDIA H100 in orbit (November 2025)
- **Axiom Space:** Launched orbital data center nodes (January 2026)
- **SpaceX:** Filed FCC applications for up to 1 million data center satellites

**The Scale Challenge:**
> "To dissipate just 1 MW of heat while keeping electronics at 20°C, an orbital data center would require a radiator surface of approximately **1,200 square meters**—roughly the size of four tennis courts."

**Source:** [SatNews - Physics Wall](https://satnews.com/2026/03/17/the-physics-wall-orbiting-data-centers-face-a-massive-cooling-challenge/)

---

## 4. Limitations and Constraints

### Humidity Effects

- Atmospheric transmissivity in 8-13 μm range significantly lower in high humidity
- Hong Kong field tests: Only 38 W/m² maximum nighttime cooling, NO daytime cooling effect
- Tropical environments: Performance "deteriorates" due to humidity AND solar radiation

**Source:** [ScienceDirect - Humidity effects](https://www.sciencedirect.com/science/article/abs/pii/S0017931021015362)

### Cloud Cover Impact

| Cloud Base Height | Net Cooling Power |
|-------------------|-------------------|
| 1 km | 14 W/m² |
| 2 km | 22 W/m² |
| 5 km | 44 W/m² |

- Over 95% of annual hours in Beijing, London, NYC, Kuala Lumpur have cloud bases below 3 km
- Full cloud cover reduces but doesn't eliminate cooling (cloud base still cooler than ground)

**Source:** [Frontiers - Cloud cover effects](https://www.frontiersin.org/journals/energy-research/articles/10.3389/fenrg.2021.658338/full)

### Geographic Constraints

**Works well:**
- Arid climates (deserts, high plateaus)
- Low humidity regions
- Clear sky conditions

**Works poorly:**
- Tropical climates
- Humid coastal regions
- Areas with persistent cloud cover
- Urban heat islands

**Key Finding:**
> "Densely populated and humid regions are not well suitable for radiative cooling applications."

**Source:** [MDPI - Global Radiative Cooling Potential](https://www.mdpi.com/2073-4433/12/11/1379)

### Practical Glare Issue

> "The primary obstacle to PDRC implementation is the glare that may be caused through the reflection of visible light onto surrounding buildings."

---

## 5. Scale Comparison: Data Centers vs Radiative Cooling

### Data Center Cooling Requirements

| Equipment Type | Cooling Requirement |
|----------------|---------------------|
| Traditional rack | 5-10 kW/rack |
| High-density VM | 20-40 kW/rack |
| AI Inference | 30-60 kW/rack |
| AI Training | 80-200 kW/rack |
| NVIDIA GB200 NVL72 | 120 kW/rack |
| Future AI | 200-500+ kW/rack |

### Radiative Cooling Capacity

At **100 W/m²** (optimistic daytime performance):
- 1 kW cooling requires 10 m² of panels
- 10 kW rack requires 100 m² of panels
- 100 kW rack requires **1,000 m²** of panels (quarter acre)
- 1 MW data hall requires **10,000 m²** (2.5 acres)
- 10 MW data center requires **100,000 m²** (25 acres)

### The Mismatch Is Fundamental

**Single NVIDIA GB200 NVL72 rack (120kW):**
- Would require **1,200 m²** of radiative panels
- That's a 35m × 35m area (roughly 8 tennis courts)
- **FOR A SINGLE RACK**

**A 10MW AI data center:**
- Would require **100,000 m²** of panels
- That's 10 hectares (25 acres) of panel surface
- Plus the actual building footprint
- Plus access roads, etc.

---

## 6. Realistic Applications

### Where Radiative Cooling CAN Help

**Building HVAC Augmentation:**
- Reduce air conditioning loads by 10-40%
- Supplement existing cooling systems
- Lower electricity consumption for perimeter cooling

**Modular Data Centers:**
UC Davis HoMEDUCS project:
> "Integrating Skycool panels with polymer heat exchangers and cold plates can bring cooling energy consumption down to less than 5% of total power, all while using zero water."

**Edge Computing:**
- Small, distributed deployments
- Low power density applications
- Water-scarce remote locations

### Where Radiative Cooling CANNOT Help

**High-Density AI Workloads:**
- Scale mismatch is 100-1000x
- Cannot handle 100kW+ per rack densities
- Not a replacement for liquid cooling

**Tropical/Humid Locations:**
- Performance drops below useful threshold
- May provide zero or negative benefit

---

## 7. Commercial Deployments

### Building Applications

- 8,200 m² commercial warehouse with daytime radiative cooling film
- Simulation: 21.2-65.2% savings in cooling energy
- SkyCool testing in 6 US states

### Data Center Applications

**Status:** "Still in its infancy"

> "Radiative sky cooling has a promising application in data centers where cooling is required throughout the year, though currently, specialized research on this passive cooling strategy in DCs is still in its infancy."

**Source:** [ScienceDirect - Passive cooling review](https://www.sciencedirect.com/science/article/pii/S2666123324000916)

---

## 8. Summary Statistics

### Performance Envelope

| Metric | Best Case | Typical | Worst Case |
|--------|-----------|---------|------------|
| Cooling power | 150 W/m² | 60-80 W/m² | 0-30 W/m² |
| Sub-ambient temp | -20°C | -4 to -6°C | +3°C (heat gain) |
| Geographic coverage | Arid regions | Temperate | Humid tropical |
| Data center relevance | Supplemental | Marginal | None |

### Key Numbers

- Atmospheric window: 8-13 μm
- Space temperature: ~3K
- Theoretical max: ~150 W/m² at ambient temperature
- Practical daytime: 40-100 W/m² (climate dependent)
- AI rack requirement: 80-500 kW
- Scale mismatch: **500-5,000x**

---

## Document Metadata

**Research Date:** April 13, 2026
**Purpose:** Factual research for Thesis C: Space-Based Passive Radiative Cooling
**Verdict Preview:** Highly speculative - scale mismatch makes this impractical for direct data center cooling
