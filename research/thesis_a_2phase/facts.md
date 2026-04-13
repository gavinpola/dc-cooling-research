# 2-Phase Direct-to-Chip Liquid Cooling: Comprehensive Research Facts

**Research Date:** April 12, 2026
**Thesis:** 2-phase direct-to-chip liquid cooling using dielectric fluids or refrigerants will become the dominant cooling approach for high-density AI data centers.

---

## 1. How It Works

### Two-Phase Heat Transfer Mechanics

At the heart of two-phase cooling lies the use of latent heat of vaporization to absorb and transport heat more efficiently than either air or single-phase liquid systems. ([Chatsworth, 2024](https://www.chatsworth.com/en-us/resources/blogs/2024/what-is-two-phase-direct-to-chip-liquid-cooling))

**The Evaporation-Condensation Cycle:**

1. **Cold Plate Installation:** A cold plate is mounted directly onto the chip's surface (CPU or GPU), allowing cooling liquid to flow through it and form a cooling layer.

2. **Evaporation Phase:** The fluid (typically a refrigerant) evaporates inside an evaporator at the heat source, absorbing massive amounts of energy without significant temperature increase. As the refrigerant absorbs heat from the chip, it undergoes a phase change, transforming from liquid to vapor. ([Data Centre Solutions](https://datacentre.solutions/blogs/58393/under-the-hood-how-two-phase-direct-to-chip-liquid-cooling-works))

3. **Condensation Phase:** The vaporized refrigerant travels to a Heat Rejection Unit (HRU) or condenser where it condenses back into liquid, dissipating heat into a secondary fluid (typically facility water). ([ZutaCore Blog](https://blog.zutacore.com/zutacore-blog/what-is-closed-loop-two-phased-liquid-cooling-system))

4. **Cycle Completion:** Once condensed, the HRU directs the liquid refrigerant back to the manifold in the back of the cabinet, which distributes it to each server for the next cycle.

Coolant Distribution Units (CDUs) pump liquid or refrigerant through cold plates, where the coolant absorbs heat from the server and evaporates. The resulting vapor then returns to the CDU, where it condenses back into liquid through a heat exchange process. ([Vertiv, 2026](https://www.vertiv.com/en-asia/about/news-and-insights/articles/blog-posts/pumped-two-phase-direct-to-chip-cooling-advancing-ai-data-center-efficiency/))

### Key Advantages Over Single-Phase

**Superior Heat Transfer:**
- In two-phase systems, the heat transfer coefficient (h value) is often significantly higher where the phase change (vaporization and condensation) is occurring. ([Asperitas](https://www.asperitas.com/knowledge-hub/single-phase-vs-two-phase-immersion-cooling))

**High Power Handling:**
- Two-phase direct-to-chip cooling handles thermal design power (TDP) over 2,500 watts, while immersion cooling typically struggles above 700 watts. ([ZutaCore Blog](https://blog.zutacore.com/zutacore-blog/two-phase-dlc-not-immersion-liquid-cooling))

**Waterless Operation:**
- The cold plates do not use water at all. The dual phase pool boiling approach uses a heat transfer fluid to evacuate the heat from the chips via liquid to vapor phase change. ([ZutaCore Blog](https://blog.zutacore.com/zutacore-blog/what-is-closed-loop-two-phased-liquid-cooling-system))

**Low Fluid Requirements:**
- A 100kW rack using two phase direct-to-chip technology uses less than 4 gallons of heat transfer fluid, vs. immersion cooling that needs over 100 gallons per rack. ([ZutaCore Blog](https://blog.zutacore.com/zutacore-blog/two-phase-dlc-not-immersion-liquid-cooling))

### Comparison: Two-Phase vs Single-Phase

Two-phase cooling relies on a fluid engineered to intentionally boil at operating temperatures. In contrast, single-phase DTC cooling uses water-based coolant that remains liquid as it absorbs heat. Cost-effective and reliable for moderate heat loads, this method is ideal for data centers prioritizing affordability and simplicity, though it may have lower heat transfer capacity. ([Data Centre Solutions](https://datacentre.solutions/blogs/58393/under-the-hood-how-two-phase-direct-to-chip-liquid-cooling-works))

---

## 2. Heat Transfer Coefficients

### Two-Phase Cooling Performance

**Reported Heat Transfer Coefficients:**
- Companies like Allied Control and Iceotope have developed commercial two-phase solutions achieving heat transfer coefficients exceeding **10,000 W/m²·K**. ([NADDOD Blog](https://www.naddod.com/blog/single-phase-vs-two-phase-immersion-cooling-in-data-centers))

- Two-phase fluids enable **10 to 100 times greater heat transfer capacity** than single-phase alternatives. ([Lipoly](https://lipoly.com/en/industries/two-phase-vs-single-phase-immersion-cooling/))

- Some advanced single-phase systems utilizing microchannel technology achieve heat transfer coefficients up to 15,000 W/m²·K. ([NADDOD Blog](https://www.naddod.com/blog/single-phase-vs-two-phase-immersion-cooling-in-data-centers))

**Microchannel Boiling:**
- Heat transfer coefficient values ranged from **5,000 to 20,000 W/m²K** in cryogenic nitrogen microchannel experiments. ([ScienceDirect, 2025](https://www.sciencedirect.com/science/article/pii/S0011227525000049))

- The heat transfer coefficient on chips can increase from 600 to **5,700 W/m²·K** with surface wettability modifications. ([ScienceDirect, 2025](https://www.sciencedirect.com/science/article/abs/pii/S0017931025011317))

- Chen et al. achieved a heat transfer coefficient of **23,200 W/m²·K** using HFE-7100 with crossed mini channels and capillary wick strategy. ([Accelsius](https://accelsius.com/wp-content/uploads/A-Practical-Metric-for-Cold-Plate-Thermal-Performance-in-Two-Phase-Direct-to-Chip-Cooling.pdf))

**Why Two-Phase Has Higher Heat Transfer:**
- Latent heat of vaporization allows the dielectric fluid to absorb massive amounts of heat without significant temperature rise. Its heat transfer coefficient is **50–100 times higher** than forced-air cooling, as the liquid-vapor transition creates turbulent fluid movement that eliminates the stagnant thermal boundary layer. ([Soeteck](https://soeteck.com/en/news-and-insights/blogs/two-phase-liquid-immersion-cooling/))

- Two-phase immersion cooling leverages both latent heat (from phase change) and sensible heat, enabling it to handle heat fluxes that are **5–10 times higher** than single-phase systems—critical for supporting 50+ kW/rack densities. ([Dixon Valve Blog](https://blog.dixonvalve.com/single-phase-vs-two-phase-cooling))

### Single-Phase Cooling Performance

Major technology providers including 3M, Submer, and LiquidStack have established mature single-phase solutions with operational temperatures typically ranging from 40°C to 90°C, with heat transfer coefficients generally between **500-2000 W/m²K** depending on fluid properties and flow conditions. ([NADDOD Blog](https://www.naddod.com/blog/single-phase-vs-two-phase-immersion-cooling-in-data-centers))

---

## 3. Coolants and Fluids

### Refrigerant Types

**R-1234ze (HFO-1234ze):**
- Global Warming Potential (GWP): **Less than 1** (99.9% lower than R-134a)
- Ozone Depletion Potential (ODP): **Zero**
- Safety Classification: **A2L** (non-flammable according to ASHRAE standard 34)
- Properties: Great thermal and chemical stability, low toxicity, highly compatible with majority of materials
- Patent: Developed and patented by Honeywell
- Source: ([Kaltra](https://www.kaltra.com/r-1234ze), [Honeywell](https://advancedmaterials.honeywell.com/us/en/products/air-conditioning-refrigeration-and-heating/solstice-hfos/solstice-ze-r-1234ze))

**HFO-1336mzz(Z) (cis-CF3CH=CHCF3):**
- GWP: **2** (ultra-low)
- Properties: Non-flammable HydroFluoro-Olefin (HFO), surprisingly high chemical stability at high temperatures
- Applications: Designed as foam blowing agent but suitable for Organic Rankine Cycles, high temperature heat pumps, and commercial chillers
- Performance: Requires 36.5%–41% lower pump power and enables up to 17% higher net cycle efficiencies than HFC-245fa
- Source: ([KTH](https://www.energy.kth.se/applied-thermodynamics/key-research-areas/heating-systems/low-gwp-news/r1336mzz-z-ett-nytt-hogtemperaturkoldmedium-med-bra-egenskaper-1.501202))

**HFO-1336mzz(E) (trans isomer):**
- GWP: **18**
- Boiling point: **7.5°C (45.5°F)**
- Critical temperature: **137.7°C (279.9°F)**
- ODP: **Zero**
- Properties: Non-flammable, low GWP, favorable toxicity profile, chemically stable up to 250°C for 7 days
- Applications: Waste heat recovery, high temperature heat pumps (HTHP), Organic Rankine Cycle (ORC)
- Source: ([Novel Working Fluid PDF](https://www.w-refrigerant.com/wp-content/uploads/2020/10/Novel-Working-Fluid-HFO-1336mzzE-for-Use-in-Waste-Heat-Recovery-Applications.pdf))

### 3M Novec Fluids (Discontinued)

**Key Properties:**
- 3M Novec Engineered Fluids are hydrofluoroether-based (HFE) fluids
- Not classified as flammable, non-oil-based, low toxicity, non-corrosive
- Good material compatibility and thermal stability
- High dielectric constants (may lead to insertion losses in high-frequency applications)
- Boiling points: Novec 649 (49°C) and Novec 7000 (34°C) dominated commercial deployments
- Source: ([3M Data Sheet](https://multimedia.3m.com.cn/mws/media/1801351O/data-center-immersion-cooling-aplications-with-3m-novec-engineered-fluids-line-card.pdf), [Dynalene](https://www.dynalene.com/immersion-coolants-for-data-centers-selection-criteria/))

**3M Exit from Production:**
- Effective **January 15, 2025**, 3M officially ceased production of 3M Novec 7500
- 3M announced exit from production of per- and polyfluoroalkyl substances (PFAS) by end of 2025
- This includes discontinuing entire line of Novec and Fluorinert fluids (known as "forever chemicals")
- Source: ([DCD](https://www.datacenterdynamics.com/en/news/two-phase-cooling-will-be-hit-by-epa-rules-and-3ms-exit-from-pfas-forever-chemicals/), [Best Technology Inc](https://www.besttechnologyinc.com/3m-novec-replacements/))

### Alternative Fluids (3M Novec Replacements)

**Galden PFPE (Syensqo/Solvay):**
- Perfluoropolyether (PFPE) fluids
- Good dielectric properties, exceptional chemical stability
- Operate at very low and very high temperatures in aggressive conditions
- Note: Also classified as PFAS
- Source: ([Sales and Service Inc](https://salesandserviceinc.com/3M-Replacement-Fluids/))

**BestSolv Engineered Fluids:**
- BestSolv Exact Molecule replacements: Match 3M Novec chemically (classified as PFAS under U.S. EPA definition)
- BestSolv Similar Molecule replacements: Use different HFE molecule, NOT classified as PFAS under U.S. EPA proposed definition
- Source: ([Best Technology Inc](https://www.besttechnologyinc.com/3m-novec-replacements/))

**PROMOSOLV NEO Line:**
- PFAS-free alternatives
- Ultra-low to no GWP
- Ideal for sustainable future and green 3M Novec replacement
- Source: ([Inventec](https://www.inventec.dehon.com/looking-for-a-3m-novec-replacement/))

**TMC Fluids:**
- TMC HFE-347E: 3M Novec 7100 equivalent offering similar chemistry and physical properties
- Source: ([TMC Industries](https://tmcindustries.com/collections/immersion-cooling))

**INVENTEC THERMASOLV:**
- High-performance dielectric cooling fluids designed for electronic and electrical devices
- Source: ([Inventec](https://www.inventec.dehon.com/looking-for-a-3m-novec-replacement/))

### Supply Chain and Cost Considerations

**Cost Differences:**
- Fluorocarbon-based two-phase coolants such as 3M Novec typically cost **an order of magnitude more** than hydrocarbon-based single-phase fluids like ElectroSafe from GRC
- When using over 300 gallons of fluid in a single rack, additional costs can be significant
- Fluorocarbon fluids cost multiples of hydrocarbon fluids, with the gap compounding at rack scale
- Unlike single-phase fluids, fluorocarbon-based coolants must be regularly replenished at **hundreds of dollars per gallon**
- Source: ([Asperitas](https://www.asperitas.com/knowledge-hub/single-phase-vs-two-phase-immersion-cooling), [Lipoly](https://lipoly.com/en/industries/two-phase-vs-single-phase-immersion-cooling/))

**Supply Chain Concerns:**
- Single-phase fluids offer "optionality"—a broad ecosystem of vendors
- Two-phase cooling often depends on a narrow chemical supply base, creating vendor lock-in and potential exposure to discontinuation risks
- 3M has exited production of Novec and all PFAS-based products entirely
- Single-phase immersion fluids are non-volatile, available from multiple global suppliers, and typically reclaimable
- Source: ([Lipoly](https://lipoly.com/en/industries/two-phase-vs-single-phase-immersion-cooling/), [DCD](https://www.datacenterdynamics.com/en/news/two-phase-cooling-will-be-hit-by-epa-rules-and-3ms-exit-from-pfas-forever-chemicals/))

**Regulatory Considerations:**
- For dielectric fluids, the 2026 focus is on navigating new PFAS regulations
- Two-phase fluids are typically much more expensive and volatile than single-phase fluids
- Environmental impact (GWP) and potential regulatory scrutiny (PFAS) are significant considerations
- Source: ([Energy Solutions](https://energy-solutions.co/articles/sub/data-center-cooling-liquid-immersion-vs-air))

---

## 4. Key Companies

### JetCool Technologies

**Company Background:**
- Founded: 2019 as MIT Lincoln Laboratory spin-off
- Origin: Team led by Bernie Malouin spent five years at MIT Lincoln Laboratory developing the technology
- Status: **Acquired by Flex on November 14, 2024**
- Source: ([Tracxn](https://tracxn.com/d/companies/jetcool-technologies/__HxtpaKkfaDCdrBXQ6FZ1Xd2rGqHmeXtd3PjQ_OhpXcE), [JetCool About](https://jetcool.com/about/))

**Technology:**
- **Microconvective cooling**: Patented single-phase direct-to-chip liquid cooling technology
- Uses arrays of fluid jets to cool high-power devices
- Unlike heat sinks or traditional microchannel cold plates that pass fluid over a surface, cooling jets route fluid directly at the surface
- Creates an **order-of-magnitude improvement** in heat transfer
- Customers achieve **18% power savings**, use higher coolant temperatures over 60°C, and eliminate water consumption
- Source: ([JetCool Technology](https://jetcool.com/technology/))

**Funding:**
- Total funding: **$28.7M over 5 rounds** from 6 investors
- Series A (October 2023): **$17 million** led by Bosch Ventures, with participation from In-Q-Tel, Raptor Group, and Schooner Capital
- ARPA-E COOLERCHIPS program: Up to **$1,265,747** from U.S. Department of Energy
- Source: ([Tracxn](https://tracxn.com/d/companies/jetcool-technologies/__HxtpaKkfaDCdrBXQ6FZ1Xd2rGqHmeXtd3PjQ_OhpXcE), [JetCool Series A](https://jetcool.com/post/series-a/), [Street Insider](https://www.streetinsider.com/Globe+Newswire/JETCOOL+Technologies+Inc.+Selected+to+Receive+Over+$1.2M+in+Federal+Funding+to+Develop+More+Efficient+Cooling+for+Data+Centers/21642907.html))

**Customers and Deployments (2026):**
- Collaborated with **Broadcom** to deliver liquid cooling for next-generation AI XPUs (March 2026)
- Expanded partnership with **Sabey Data Centers** to accelerate sustainable high-density compute (January 2026)
- **Sandia National Laboratories** utilizing JetCool liquid cooling modules for HPC cluster
- Trusted by OEMs, hyperscalers, and chipmakers
- Source: ([Tracxn](https://tracxn.com/d/companies/jetcool-technologies/__HxtpaKkfaDCdrBXQ6FZ1Xd2rGqHmeXtd3PjQ_OhpXcE), [JetCool](https://jetcool.com/))

**Acquisition Impact:**
- Flex acquisition bolsters data center and power portfolio to help hyperscale and enterprise customers solve power, heat, and scale challenges in AI era
- Brings together JetCool's advanced direct-to-chip liquid cooling and Flex's expertise across IT and power infrastructure, global manufacturing, and vertical integration
- Source: ([Tracxn](https://tracxn.com/d/companies/jetcool-technologies/__HxtpaKkfaDCdrBXQ6FZ1Xd2rGqHmeXtd3PjQ_OhpXcE))

### ZutaCore

**Company Background:**
- Founded: 2016
- Headquarters: Redefining sustainable cooling solutions
- Technology: Patented two-phase HyperCool technology
- Source: ([ZutaCore](https://zutacore.com))

**Technology:**
- **HyperCool**: Waterless, direct-to-chip liquid cooling using two-phase technology
- At chip level, uses dielectric heat transfer fluid that absorbs heat through controlled boiling process
- As fluid vaporizes, carries heat away from processor to Cooling Distribution Unit (CDU) where it condenses and recirculates
- Closed-loop process enables precise, on-demand cooling responding instantly to changing workload conditions
- Reduces energy consumption by up to **82%**
- Source: ([ZutaCore](https://zutacore.com), [ZutaCore Blog](https://blog.zutacore.com/press-releases/waterless-two-phase-cooling-for-nvidia-rtx-pro-6000))

**Key Products:**
- **OmniTherm Cold Plate**: Enables waterless two-phase cooling for NVIDIA RTX PRO 6000 Blackwell Server Edition GPUs in single-slot PCIe form factor; supports up to **600W per GPU**
- **Two-Phase Sidecar Solution**: Industry's first for hyperscalers; enables cooling up to **240kW** using hot swappable components; designed to handle heat from high-power GPUs in high-density racks; fits within standard data center infrastructures without facility water loops
- Source: ([ZutaCore Press](https://blog.zutacore.com/press-releases/waterless-two-phase-cooling-for-nvidia-rtx-pro-6000), [PR Newswire](https://www.prnewswire.com/news-releases/zutacore-announces-the-industrys-first-two-phase-sidecar-solution-at-the-ocp-apac-summit-enables-240kw-cooling-power-with-no-facility-water-302522011.html))

**Hyperscaler Relevance:**
- CTO My Truong: "Many of the world's largest hyperscale data centers rely solely on air cooling, which makes it extremely difficult to support the thermal demands of next-generation AI GPUs. Our sidecar solution addresses this challenge directly, cooling up to **two 120kW racks or four 60kW racks** using a closed-loop, facility water-free two-phase system."
- Hyperscalers don't want water in facilities due to risk of leakage and high maintenance
- Source: ([Storage Review](https://www.storagereview.com/news/zutacore-unveils-two-phase-sidecar-cooling-system-for-high-density-ai-workloads))

**Deployments:**
- Global AI-as-a-Service (AIaaS) leading provider chose HyperCool for AI servers with deployments starting **Q3 2024**
- First platform: **Dell Technologies XE9680**, delivered via UNICOM Engineering's global services
- HyperCool qualified by **Intel and AMD**
- Deployed in server manufacturers including **Dell, SuperMicro, ASUS, Pegatron**
- Source: ([ZutaCore Solutions](https://zutacore.com/solutions))

**Funding:**
- Specific funding information not found in search results

### Accelsius

**Company Background:**
- Founded: **2022** by Innventure LLC
- Headquarters: Texas
- Technology: Commercializing technology developed by **Nokia's Bell Labs**
- Source: ([Innventure](https://www.innventure.com/companies/accelsius))

**Technology:**
- Two-phase, direct-to-chip liquid cooling platform
- Cooling capability: **4500W+ per socket**
- **NeuCool** thermal resistance: Industry-leading **0.020°C/W** at 700W+ TDP (H100 GPU)
- Uses waterless, low-pressure, dielectric refrigerant with **zero Ozone Depletion Potential**
- Source: ([Accelsius](https://accelsius.com/accelsius-unveils-neucool-with-unrivaled-thermal-performance-for-ai-data-centers/))

**Products:**
- **NeuCool IR150**: Rack-level, two-phase liquid cooling system combining compute space and cooling infrastructure in single enclosure
- Handles up to **150kW per rack**
- Supports NVIDIA Blackwell GPUs with enough thermal headroom for next-generation architectures
- Supports warm-water cooling up to **45°C (ASHRAE W45 standard)**, enabling more free cooling and reducing reliance on chillers
- Source: ([TechEdge AI](https://techedgeai.com/accelsius-debuts-neucool-ir150-a-plug-and-play-150kw-liquid-cooling-rack-for-ai-data-centers/))

**Performance Demonstrations:**
- In-row two-phase CDU paired with retrofitted cold plates on four-way H100 server cooled fully loaded **250kW rack** even when fed with facility water at **40°C**—well above conventional thresholds
- Source: ([Data Center Frontier](https://www.datacenterfrontier.com/cooling/article/55281394/coolit-and-accelsius-push-data-center-liquid-cooling-limits-amid-soaring-rack-densities))

**Cost Savings:**
- **35% OpEx savings** over single-phase direct-to-chip
- **8–17% total cost of ownership savings**
- pPUE values: **1.05 to 1.10** (vs. traditional air-cooled PUE of 1.3-1.6)
- Source: ([Accelsius](https://accelsius.com/why-two-phase-is-the-winning-choice-vs-single-phase/), [Data Center Knowledge](https://www.datacenterknowledge.com/cooling/how-two-phase-liquid-cooling-is-solving-the-thermal-crisis))

**Funding:**
- **Multi-million dollar strategic investment** from Johnson Controls (October 2025)
- Source: ([Johnson Controls](https://www.johnsoncontrols.com/media-center/news/press-releases/2025/10/06/johnson-controls-announces-investment-in-data-center-liquid-cooling-company-accelsius))

**Deployments:**
- **DarkNX** plans to deploy NeuCool at 300 MW AI data center campus in Ontario
- CEO Josh Claman: **Three-quarters** of Accelsius's current pipeline consists of production opportunities rather than proof-of-concept scenarios
- Source: ([Data Center Knowledge](https://www.datacenterknowledge.com/cooling/how-two-phase-liquid-cooling-is-solving-the-thermal-crisis))

### LiquidCool Solutions

**Company Background:**
- Founded: **2006** by Daren Klum and Chad Attlesey
- Headquarters: Rochester, Minnesota
- Initial products: High-performance gaming systems and engineering workstations
- Current focus: Immersion-cooled server systems for data centers
- Source: ([Tracxn](https://tracxn.com/d/companies/liquidcool-solutions/__UMCrfDa03-oFAlVuoyd2v3A2URWD3_D9MDw-onEmg6w))

**Technology:**
- **Total Liquid Immersion with Directed-Flow (TIDF)**: Patented technology
- Only company combining Total Liquid Immersion with Directed Flow (direct-to-chip) in standard 19″ vertical rack
- Employs **single-phase immersion** (note: not two-phase)
- Designed to be installed into standard IT racks (not tank-based)
- By eliminating internal fans, chillers, and air handling systems, LCS systems reduce data center energy use by **30% or more** compared to air-cooling
- Source: ([LiquidCool](https://liquidcoolsolutions.com/immersion-cooling-technology/))

**Funding:**
- Total: **$5.18M over 4 funding rounds** (2 Seed, 2 Early-Stage)
- Largest round: Series A for **$3.58M** (October 2013)
- Investors: FUND4SE, StarTec Investments, Wells Fargo Innovation Incubator, Capital Midwest Fund, Cornerstone Angels, DataQube
- DataQube investment: **April 27, 2022** in Series B round
- Source: ([Tracxn](https://tracxn.com/d/companies/liquidcool-solutions/__UMCrfDa03-oFAlVuoyd2v3A2URWD3_D9MDw-onEmg6w))

**Customers & Partnerships:**
- ServerDomes partnered with LiquidCool (October 2023)
- DataQube collaboration in edge data center projects
- MIRIS (Norway's leader in Green Real Estate Technology) partnership (January 2020)
- Strategic Alliance with Dedicated Computing for liquid cooled technical computing solutions (May 2013)
- Source: ([LiquidCool](https://liquidcoolsolutions.com/))

**Recognition:**
- NREL referred to LiquidCool technology as the **"Gold Standard"** for cooling building-connected data centers
- **Solar Impulse Foundation** certified as provider of profitable, efficient green energy solutions (2021)
- IN2 program ($10-million program funded by Wells Fargo Foundation, co-administered by NREL on behalf of U.S. DOE) supported LiquidCool's testing and validation
- Source: ([LiquidCool](https://www.liquidcoolsolutions.com/in2-company-liquidcool-solutions-successfully-completes-first-round-of-testing/))

### Asetek

**Company Overview:**
- Publicly traded: Asetek Inc. listed as key player in data center liquid cooling market
- Products: Ingrid platform for B2B applications
- Source: ([Globe Newswire](https://www.globenewswire.com/news-release/2026/02/17/3239044/0/en/Data-Center-Liquid-Cooling-Market-to-Witness-28-7-CAGR-Driven-by-AI-Adoption-Investments-and-Sustainability-Targets.html))

**Ingrid Platform for AI/HPC:**
- Designed for B2B applications
- Offers customizable inlet/outlet orientations, smart thermal sensing, acoustic efficiency
- Addresses unique needs of HPC and AI workloads
- 2025: Secured **$35 million minimum volume commitment** from returning top-tier customer for high-end liquid cooling solutions based on Ingrid platform
- Deliveries scheduled: **Q2 2026** (first product), **Q4 2026** (second product)
- Source: ([Asetek AI/HPC](https://www.asetek.com/company/about-asetek/asetek-heritage-technology/data-center/technology-for-data-centers/ai-hpc/))

**Asetek Emma (G8) V2 Pump:**
- Nominal speed: Approximately **3,600 RPM**
- Triple-layer noise-reduction pump cover reduces air-borne noise and structure-borne vibrations
- Dedicated mode switch for three different pump speed profiles
- Source: ([Technetbook](https://www.technetbooks.com/2026/03/noctua-asetek-liquid-cooling.html))

**Partnership with Noctua:**
- Flagship AIO liquid coolers completed Production Validation Test (PVT) phase
- Planned launch: **Q2 2026**
- Source: ([Asetek Press](https://www.asetek.com/press-releases/noctua-and-asetek-announce-flagship-aio-liquid-coolers-complete-pvt-phase-targeted-for-q2-2026-launch/))

**Technology:**
- Asetek's patented liquid cooling technology in data centers redefines energy efficiency and sustainability
- Source: ([Fierce Network](https://www.fierce-network.com/cloud/cooling-tech-made-space-heads-data-centers-mikros-ceo-says))

### CoolIT Systems

**Company Overview:**
- Working directly with world's top semiconductor, server and hyperscale technology companies
- Designs and mass-produces highly optimized liquid cooling solutions
- Source: ([CoolIT](https://www.coolitsystems.com/))

**Focus:**
- Advanced Technologies Group pushing boundaries of **single-phase liquid cooling**
- Advancing innovations in system architecture, materials, and coolants
- Exploring emerging and alternative thermal technologies in parallel
- Source: ([CoolIT](https://www.coolitsystems.com/))

**Performance Data:**
- Production deployment: **300 NVIDIA H100 GPUs** maintained **62°C junction temperatures** at full load using just **25°C inlet water**
- Microchannel designs achieve **0.015°C/W thermal resistance**
- Coolant Distribution Modules support **300kW in 8U form factor**
- Source: ([ByteBridge](https://www.bytebt.com/direct-to-chip-cooling-liquid-cooling-ai-data-centers/))

**Note:**
- CoolIT Systems is primarily known for **single-phase** direct liquid cooling solutions
- Two-phase direct-to-chip cooling space led by other companies like Vertiv, ZutaCore, and Accelsius
- Source: ([DCD](https://www.datacenterdynamics.com/en/broadcasts/dcdkeeping-it-cool-hybrid-2025/2025/single-phase-versus-two-phase-direct-to-chip-liquid-cooling/))

### LiquidStack

**Company Background:**
- Leads in high-performance two-phase immersion cooling
- Target customers: Hyperscale, cloud service providers, AI workloads
- Predecessor: Bitfury deployed 40MW 2-phase immersion-cooled data center in Republic of Georgia (first of its kind)
- 120MW 2-phase immersion-cooled data center deployed in Azerbaijan (largest liquid-cooled data center ever built)
- Source: ([LiquidStack About](https://liquidstack.com/about-us))

**Funding:**
- Series C (January 2026): **USD 75 million** led by SoftBank Vision Fund
- Purpose: Triple tank capacity at new Singapore plant, targeting Asia-Pacific hyperscale demand
- Source: ([Facilities Dive](https://www.facilitiesdive.com/news/liquidstack-touts-modular-scalable-data-center-coolant-distribution-unit/749676/))

**Technology:**
- Single phase and two phase immersion cooling solutions
- Cooling capacity: Up to **252kW** in 48U rack with modular form factors
- Tanks rated to **252 kW** with passive circulation loop requiring no pumps
- 2-phase immersion cooling tanks reduce space by **90%**, use less energy
- Source: ([LiquidStack](https://liquidstack.com/), [GIGABYTE](https://www.gigabyte.com/Solutions/liquidstack-two-phase))

**Key Customers & Deployments:**
- **Microsoft**: Tested LiquidStack's two-phase immersion systems supporting power densities up to **250 kW per rack**; system installed at Microsoft's Quincy data center
- **NTT Data**: Tested at Tokyo data center, resulted in **97% less cooling energy** than traditional cooling systems
- **Wiwynn**: Invested in LiquidStack
- **GIGABYTE Partnership**: Joined forces with LiquidStack and 3M to offer Two-Phase Immersion Cooling solution
- Source: ([DCD](https://www.datacenterdynamics.com/en/analysis/liquid-cooling-a-new-phase/))

**Market Position:**
- Specialist suppliers Green Revolution Cooling, Submer, LiquidStack, and Asperitas collectively held around **35% of tank shipments in 2025**
- LiquidStack will begin quoting orders for GigaModular CDU units in **mid-Q1 2026**
- Source: ([Mordor Intelligence](https://www.mordorintelligence.com/industry-reports/immersion-cooling-market-in-data-centers))

**Large-Scale Deployment:**
- One 40MW two-phase immersion facility uses less than **2 liters of fluid per kW**
- 12kW 1U modules housed in **250kW tanks** using 48-53ºC water to cool
- Same tanks sized for up to **500kW** to accommodate next-generation hardware
- Source: ([Electronics Cooling](https://www.electronics-cooling.com/2024/10/power-density-in-the-context-of-two-phase-immersion-cooling/))

### Vertiv

**Company Position:**
- Leading player in liquid cooling, holding **70%+ of volume share** for first batch of GB200 racks shipped
- Remaining share largely shared by Motivair and CoolIT
- Reported **60% year-over-year increase** in organic orders in Q3 2025
- Source: ([EnkiAI](https://enkiai.com/data-center/vertiv-liquid-cooling-dominating-ai-data-centers-in-2025))

**Two-Phase Technology:**
- **Pumped Two-Phase (P2P) Direct-to-Chip Cooling**
- With cooling systems consuming up to 40% of AI data center's total energy, P2P direct-to-chip cooling reduces cooling energy consumption by up to **82%**
- Source: ([Vertiv](https://www.vertiv.com/en-us/about/news-and-insights/articles/blog-posts/pumped-two-phase-direct-to-chip-cooling-advancing-ai-data-center-efficiency/))

**Key Products:**
- **CoolChip CDU**: Designed to support liquid cooling within high density environments; suitable for direct-to-chip and rear door cooling applications
- **CoolChip CDU 600**: Liquid-to-liquid coolant distribution unit for in-row deployment; targets high-density AI and HPC installations
- **MegaMod HDX** (announced January 2026): Scalable, hybrid cooling solution; delivers capacity up to **10 MW**; accommodates rack densities from **50 kW to more than 100 kW per rack**
- Source: ([Vertiv CoolChip](https://www.vertiv.com/en-us/products-catalog/thermal-management/high-density-solutions/vertiv-coolchip-cdu/), [PR Newswire](https://www.prnewswire.com/news-releases/vertiv-introduces-new-modular-liquid-cooling-infrastructure-solution-to-support-high-density-compute-requirements-in-north-america-and-emea-302661073.html))

**Intel Gaudi3 Collaboration:**
- Collaborated with Intel in late 2023 to develop and test P2P direct-to-chip system for **Gaudi3 accelerator**
- Handled up to **160kW per rack**
- Liquid cooled solution tested up to **160kW accelerator power** using facility water from **17°C up to 45°C**
- Air-cooled solution tested up to **40kW of heat load** in warm ambient air data centers up to **35°C**
- Source: ([Vertiv Intel](https://www.vertiv.com/en-us/about/news-and-insights/corporate-news/vertiv-collaborates-with-intel-on-liquid-cooled-solution-for-the-intel-gaudi3-ai-accelerator-platform/))

**Customer Deployments:**
- **Compass Data Centers**: Partnered on system that can switch from air to liquid cooling; initial units deployed Q1 2025 as part of planned multi-year, multi-billion dollar supply arrangement
- **Elea (Brazil)**: Ordered hundreds of CDUs to support liquid cooling for AI applications at São Paulo sites; first phase of **$300 million** AI data center initiative delivered in 2025
- Source: ([DCD](https://www.datacenterdynamics.com/en/news/vertiv-to-deliver-cooling-units-to-compass/))

**Technology Readiness:**
- Study "Maturation of Pumped Two-Phase Liquid Cooling to Commercial Scale-Up Deployment" indicates P2P direct-to-chip liquid cooling achieved:
  - Technology Readiness Level (TRL): **7**
  - Commercial Readiness Level (CRL): **2**
- Source: ([Vertiv](https://www.vertiv.com/en-us/about/news-and-insights/articles/blog-posts/pumped-two-phase-direct-to-chip-cooling-advancing-ai-data-center-efficiency/))

### Boyd Thermal (Acquired by Eaton)

**Acquisition:**
- Power and cooling firm **Eaton** signed agreement to acquire Boyd Thermal business of Boyd Corporation from Goldman Sachs Asset Management for **$9.5 billion**
- Source: ([DCD](https://www.datacenterdynamics.com/en/news/eaton-acquires-boyd-thermal-for-95bn-to-further-liquid-cooling-portfolio/))

**Technology:**
- Overlapping technology portfolio enables liquid, immersion, two phase, and air-cooling innovation to co-exist
- Two-phase cooling solutions spread, transport, and dissipate high heat loads with two-phase vapor chambers, thermosiphon systems, and heat pipe assemblies
- Two-phase immersion cooling uses dielectric liquid that absorbs heat, vaporizes and condenses back into liquid form through continuous cycle
- Source: ([Boyd](https://www.boydcorp.com/thermal/single-phase-vs-two-phase-immersion-cooling.html))

**Products:**
- Delivers both single-phase and two-phase immersion cooling
- Offerings include CDUs, cold plates, and cooling loops
- Extreme air-cooling solutions leverage speed and low temperature differential of two-phase technologies
- Source: ([Boyd](https://www.boydcorp.com/industries/cloud-data-center.html))

**Enhanced Capabilities:**
- Durbin Group acquisition enhanced Boyd's development efforts for current and next-generation thermal management
- Durbin Group's expertise in single and two-phase liquid cooling systems
- Source: ([Business Wire](https://www.businesswire.com/news/home/20240710283918/en/Beyond-Liquid-Cooling-Boyd-Strengthens-AI-Cooling-Innovation-Capabilities-with-Durbin-Group-Acquisition))

**Eaton Portfolio Post-Acquisition:**
- Expertise across broad range of technologies
- Traditional and advanced air and liquid cooling systems, heat exchangers, conduction cooling, and two-phase heat transfer
- Source: ([Eaton](https://www.eaton.com/us/en-us/company/news-insights/news-releases/2025/eaton-signs-agreement-to-acquire-boyd-thermal--expanding-solutio.html))

### Motivair (by Schneider Electric)

**Key Products:**
- **MCDU-70** (Newest/Highest Capacity): Delivers cooling for up to **2.5 megawatts (MW)** of power; highest-capacity CDU available from Motivair; at 2.5 MW each, six MCDU-70s can provide 4+2 redundancy for 10MW designs
- **MCDU-50**: Delivers up to **1.7MW** of robust cooling capacity for AI and HPC workloads
- **MCDU-45 and MCDU-55**: First purpose-built CDUs for optimized installation in utility corridors
- Source: ([Motivair Press](https://www.motivaircorp.com/news/motivair-by-schneider-electric-announces-new-cdu-with-capability-to-scale-to-10mw-and-beyond-for-next-gen-ai-factories-69705c3655f8517e99086bbd/), [Schneider Electric](https://www.se.com/us/en/about-us/newsroom/news/press-releases/motivair-by-schneider-electric-announces-new-cdu-with-capability-to-scale-to-10mw-and-beyond-for-next-gen-ai-factories-69705c3655f8517e99086bbd/))

**Scalability:**
- Portfolio spanning from **105kW up to 2.5MW per unit**, supporting factory-scale growth
- Utilizing Schneider Electric's EcoStruxure software, CDUs operate as centralized system
- Ability to scale to **10MW+** for next-gen HPC, AI and accelerated computing workloads
- Source: ([ARC Advisory](https://www.arcweb.com/blog/motivair-schneider-electric-introduces-25-mw-cdu-scalable-ai-hpc-data-centers))

**AI Cooling Context:**
- GPUs that power AI Factories generate **20 to 50 times more heat** than traditional CPUs
- Organizations deploying AI clusters grappling with extreme rack power densities projected to reach **1MW and beyond**
- Source: ([Motivair MCDU-50](https://www.motivaircorp.com/news/motivair-mcdu-50-future-ready-cooling-for-ai/))

**Technology Focus:**
- Most liquid-cooled capacity in use today is **single-phase direct liquid cooling**
- Use of two-phase direct liquid cooling likely to grow gradually, with adoption accelerating as chip-level TDP and thermal flux exceed practical limits of single-phase systems
- Until then, deployments likely to remain focused on pilots and early large-scale implementations
- Source: ([DCD](https://www.datacenterdynamics.com/en/opinions/the-rise-of-direct-to-chip-cooling-as-a-top-ai-cooling-system/))

---

## 5. Deployments

### Hyperscaler Deployments (2025-2026)

**Meta:**
- Deploying two-phase immersion cooling in AI-focused data centers
- Committed **$800 million** to liquid-cooled AI data center in Indiana
- Debuted **140 kW liquid-cooled rack** at OCP Global Summit 2024
- Source: ([Data Centers](https://www.datacenters.com/news/why-liquid-cooling-is-becoming-the-new-standard-in-hyperscale-facilities), [Network World](https://www.networkworld.com/article/4149069/why-ai-rack-densities-make-liquid-cooling-nonnegotiable.html))

**Microsoft:**
- Tested two-phase immersion cooling for AI training clusters, reporting **30% energy efficiency gain** and increased hardware reliability
- Deployed "Sidekick" liquid cooling systems with direct-to-chip cold plates for Azure Maia AI Accelerator chips
- Exploring advanced cooling technologies including microfluidics
- Azure AI clusters shifted to liquid cooling
- Advanced AI supercomputer unveiled in 2025 features exclusively liquid-cooled racks supporting GPT-Next training workloads
- Source: ([Data Centers](https://www.datacenters.com/news/why-liquid-cooling-is-becoming-the-new-standard-in-hyperscale-facilities), [Introl](https://introl.com/blog/liquid-cooling-mainstream-tipping-point-2025))

**Google:**
- Using custom-built liquid-cooled racks in Tensor Processing Unit (TPU) deployments
- TPU deployments shifted to liquid cooling
- Source: ([Data Centers](https://www.datacenters.com/news/why-liquid-cooling-is-becoming-the-new-standard-in-hyperscale-facilities))

**AWS:**
- Fairwater AI campuses: Atlanta site operational **October 2025**, Wisconsin expected early **2026**
- Represent paradigm shift in design using closed-loop liquid cooling systems that **eliminate operational water consumption**
- Source: ([Data Center Knowledge](https://www.datacenterknowledge.com/hyperscalers/hyperscalers-in-2026-what-s-next-for-the-world-s-largest-data-center-operators-))

### Power Densities Achieved

**Rack-Level Densities:**
- Two-phase cooling delivers PUE of 1.01 to 1.03 and supports rack densities of **150 to 250-plus kW**
- LiquidStack offers tanks rated to **252 kW** with passive circulation loop requiring no pumps
- Vertiv, NVIDIA, and Binghamton University evaluated P2P direct-to-chip system featuring Vertiv in-row R2L CDU with cooling capacity of **160 kW**; CDU handled IT loads up to **170 kW** during testing
- LiquidStack provides cooling for up to **252kW** in 48U rack
- Source: ([Soeteck](https://soeteck.com/en/news-and-insights/blogs/two-phase-liquid-immersion-cooling/), [Vertiv](https://www.vertiv.com/en-asia/about/news-and-insights/articles/blog-posts/pumped-two-phase-direct-to-chip-cooling-advancing-ai-data-center-efficiency/))

**Component-Level Capabilities:**
- ACT reports over **500 W/cm² heat flux capability** in two-phase cold plates
- NVIDIA GPU roadmap-aligned designs scale from rack to facility
- ZutaCore OmniTherm: Two-phase, direct-to-chip cold plate supporting sustained performance at up to **600W per GPU** for PCIe-based AI and HPC servers
- Source: ([ACT](https://www.1-act.com/resources/blog/data-center-cooling-systems/), [ZutaCore](https://zutacore.com/solutions))

**Next-Generation Systems:**
- NVIDIA Blackwell GPUs (GB200/GB300) operating at **1,200-1,400W**
- Vera Rubin systems targeting **600kW per rack**
- Designs being explored for **500-kW racks** assuming 48U OCP rack equipped with 46 1U servers, each housing 9 GPUs rated at 1 kW each
- Source: ([Network World](https://www.networkworld.com/article/4149069/why-ai-rack-densities-make-liquid-cooling-nonnegotiable.html), [Chilldyne](https://chilldyne.com/high-power-liquid-cooling-design-direct-to-chip-solution-requirements-for-500-kw-racks/))

**Meta Deployment:**
- Meta committed $800 million to liquid-cooled AI data center in Indiana
- Debuted **140 kW liquid-cooled rack** at OCP Global Summit 2024
- Source: ([Network World](https://www.networkworld.com/article/4149069/why-ai-rack-densities-make-liquid-cooling-nonnegotiable.html))

**Large-Scale Two-Phase Immersion:**
- One 40MW two-phase immersion facility uses less than 2 liters of fluid per kW
- 12kW 1U modules housed in 250kW tanks using 48-53ºC water to cool
- Same tanks sized for up to **500kW** to accommodate next-generation hardware
- Source: ([Electronics Cooling](https://www.electronics-cooling.com/2024/10/power-density-in-the-context-of-two-phase-immersion-cooling/))

### Real-World Performance Data

**NVIDIA H100 Systems:**
- Accelsius demonstrated in-row two-phase CDU paired with retrofitted cold plates on four-way H100 server cooled fully loaded **250kW rack** even when fed with facility water at **40°C**
- CoolIT Systems production deployment: 300 NVIDIA H100 GPUs maintained **62°C junction temperatures** at full load using just **25°C inlet water**
- Source: ([Data Center Frontier](https://www.datacenterfrontier.com/cooling/article/55281394/coolit-and-accelsius-push-data-center-liquid-cooling-limits-amid-soaring-rack-densities), [ByteBridge](https://www.bytebt.com/direct-to-chip-cooling-liquid-cooling-ai-data-centers/))

**GB200 NVL72 (NVIDIA Blackwell):**
- Power consumption: **120 kilowatts** continuously
- Delivers **1.4 exaflops** of AI compute in single rack
- NVIDIA mandates liquid cooling with strict specifications: inlet temperature **20-25°C**, flow rate **80 liters per minute**, pressure drop not exceeding **1.5 bar**
- Cooling system maintains junction temperatures below **75°C** despite continuous 120kW heat generation
- System is "fully liquid cooled design" with **45°C coolant going in and 65°C coolant coming out**
- Source: ([Introl](https://introl.com/blog/gb200-nvl72-deployment-72-gpu-liquid-cooled), [NVIDIA](https://www.nvidia.com/en-us/data-center/gb200-nvl72/))

**Intel Gaudi3:**
- Gaudi 3 AI accelerator chip packaged in standard OAM card consuming up to **900W with air cooling**
- Power envelope (TDP) rises to **1200W with liquid cooling**
- Grace-Blackwell Superchip (GB200) combines 72 Arm core CPU with pair of **1,200W GPUs**
- Back-of-envelope calculation suggests GB200 part capable of drawing **2,700W** under peak load
- Source: ([Electronic Design](https://www.electronicdesign.com/technologies/embedded/article/55017637/electronic-design-intel-rolls-out-gaudi-3-accelerator-chip-for-large-ai-clusters), [FiberMall](https://www.fibermall.com/blog/nvidia-gb200-superchip.htm))

### Market Context

**Overall Growth:**
- In 2025, hyperscalers like Google, Meta, AWS, and Microsoft are rolling out liquid-cooled environments across newest facilities
- Data center immersion cooling market reached **$4.87 billion in 2025** and will grow to **$11.10 billion by 2030** at 17.91% CAGR
- Single-phase systems retain largest market share due to installation familiarity, yet two-phase designs win pilots where extreme density and pump-free architectures prove essential
- Source: ([Data Centers](https://www.datacenters.com/news/why-liquid-cooling-is-becoming-the-new-standard-in-hyperscale-facilities))

**Investment Scale:**
- Hyperscaler capex for "big five" (Amazon, Alphabet/Google, Microsoft, Meta/Facebook, Oracle) widely forecast to exceed **$600 billion in 2026**, 36% increase over 2025
- Roughly **75%, or $450 billion**, of that spend directly tied to AI infrastructure (servers, GPUs, datacenters, equipment)
- Source: ([IEEE ComSoc](https://techblog.comsoc.org/2025/12/22/hyperscaler-capex-600-bn-in-2026-a-36-increase-over-2025-while-global-spending-on-cloud-infrastructure-services-skyrockets/))

**Rack Density Evolution:**
- Average data center rack power density increased by **38% from 2022 to 2024**
- Power densities now pushing **80 kW to 120 kW** in AI clusters
- GPU power consumption has escalated beyond air cooling capability for dense AI deployments
- Source: ([Introl](https://introl.com/blog/liquid-cooling-mainstream-tipping-point-2025))

---

## 6. Economics

### Capital Expenditure (CAPEX)

**Immersion Cooling vs Air Cooling:**
- Based on TCO model, immersion cooling offers **41% CAPEX savings** compared to air cooling
- Immersion cooling requires significantly lower initial investment compared to air cooling
- Source: ([Profile IT](https://www.profileits.com/understanding-the-total-cost-of-ownership-tco-for-a-10-mw-ai-data-center-air-cooling-vs-immersion-cooling/))

**Single-Phase Immersion Costs:**
- Building system to cool 1 MW of server equipment costs approximately **$1 million**
- Comparable direct-to-chip system costs roughly **$650,000**
- For large-scale data centers with average capacities around 100 MW, costs become prohibitive
- Capital intensity for single-phase immersion ranges from **$3,500-6,500 per kW** including tanks, fluid, pumping infrastructure, and heat rejection
- Source: ([Data Center Knowledge](https://www.datacenterknowledge.com/cooling/data-center-cooling-methods-costs-vs-efficiency-vs-sustainability))

**Retrofit Costs:**
- Retrofit costs for liquid cooling run **$2-3M/MW**, but can deliver 40% energy savings for AI infrastructure
- Source: ([Energy Solutions](https://energy-solutions.co/articles/sub/data-center-cooling-liquid-immersion-vs-air))

**Air Cooling CAPEX:**
- Air cooling is proven and widely adopted with lower upfront costs compared to liquid cooling systems
- Most data centers already have necessary infrastructure in place
- Upfront costs primarily involve fans, air conditioning units (CRAC/CRAH systems), and ductwork
- Components widely available, making air cooling cheaper to deploy initially
- Source: ([Data Centers](https://www.datacenters.com/news/liquid-cooling-vs-air-cooling-which-one-will-dominate-data-centers-in-2025))

### Operational Expenditure (OPEX) & Energy Efficiency

**OPEX Savings:**
- Immersion cooling offers **39% reduction in annual OPEX** compared to air cooling
- Driven by lower energy and maintenance needs
- Source: ([Profile IT](https://www.profileits.com/understanding-the-total-cost-of-ownership-tco-for-a-10-mw-ai-data-center-air-cooling-vs-immersion-cooling/))

**Energy Efficiency:**
- Cooling accounts for **30–40%** of data center's total energy bill
- Air-cooled facilities typically operate at PUE of **1.4 to 1.6**, meaning 40–60% extra energy consumed just to remove heat
- Well-designed direct-to-chip system can achieve PUE of **1.05 to 1.15**
- For 10MW data center, that difference translates to millions of dollars saved per year in electricity alone
- Reducing PUE from 1.4 (air) to 1.1 (liquid) on 10 MW IT load saves **3 MW continuously**—**26,280 MWh per year**
- Equivalent to **$2.6-5.2M annually** and **~11,000 tons CO2 reduction per year**
- Liquid immersion cuts cooling costs by **40%** and uses **90% less water**
- Source: ([Introl](https://introl.com/blog/liquid-vs-air-cooling-ai-data-centers), [ZutaCore Blog](https://blog.zutacore.com/zutacore-blog/air-cooled-vs-liquid-cooled-server-racks-and-data-centers-roi))

**Two-Phase Specific Savings:**
- Accelsius reports **35% OpEx savings** over single-phase direct-to-chip
- Pumped two-phase direct-to-chip cooling reduces cooling energy consumption by up to **82%**
- Source: ([Accelsius](https://accelsius.com/why-two-phase-is-the-winning-choice-vs-single-phase/), [Vertiv](https://www.vertiv.com/en-us/about/news-and-insights/articles/blog-posts/pumped-two-phase-direct-to-chip-cooling-advancing-ai-data-center-efficiency/))

**Supermicro DLC-2:**
- Reduces data center power consumption by up to **40%** compared to air-cooled installations
- Total cost of ownership decreases by up to **20%**
- Source: ([Supermicro](https://www.supermicro.com/en/pressreleases/supermicros-dlc-2-next-generation-direct-liquid-cooling-solutions-aims-reduce-data))

### Total Cost of Ownership (TCO)

**10-Year TCO Analysis:**
- Over decade, immersion cooling offers **$110,994,371 in savings** compared to air cooling
- **39% reduction in TCO** for 10 MW data center
- Combined impact of lower upfront costs and reduced operational expenses
- Source: ([Profile IT](https://www.profileits.com/understanding-the-total-cost-of-ownership-tco-for-a-10-mw-ai-data-center-air-cooling-vs-immersion-cooling/))

**TCO Components:**
- Most people understand basic concepts of TCO: sum of initial capital expenditures (CapEx) added to ongoing and long-term operational expenditures (OpEx)
- Third factor should be included: business continuity
- Typical data center TCO evaluations for server with life span of 2-3 years very different than long-term critical power requirements of complete data center with life span of 10-15 years
- Source: ([United Metal](https://unitedmetal.com/total-cost-of-ownership-for-data-center-cooling-equipment-capex-opex/), [Data Center Frontier](https://www.datacenterfrontier.com/voices-of-the-industry/article/11431525/working-toward-a-total-cost-of-ownership-metric-for-cooling))

**Accelsius TCO Advantage:**
- **8–17% total cost of ownership savings**
- Source: ([Accelsius](https://accelsius.com/why-two-phase-is-the-winning-choice-vs-single-phase/))

### Return on Investment (ROI) & Payback Period

**Payback Periods:**
- Organizations should target payback periods within **60-75% of expected infrastructure lifecycle** (typically 7-10 years) to ensure positive ROI
- Upgrading to liquid cooling plates delivers full ROI within **two to three years** for most AI data centers through:
  - **20–40%** reduction in cooling energy consumption
  - Lowers PUE from 1.5+ to below 1.2
  - Extends server hardware lifespan by **2–4 years**
  - Enables **2–3 times higher compute density** per square meter
- For new high-density deployments (>40 kW/rack), payback is **less than 1 year** through energy savings and reduced floor space
- Retrofits typically see payback in **1.5-3 years**
- Source: ([Data Center Knowledge](https://www.datacenterknowledge.com/cooling/using-a-total-cost-of-ownership-tco-model-for-your-data-center), [ZutaCore Blog](https://blog.zutacore.com/zutacore-blog/air-cooled-vs-liquid-cooled-server-racks-and-data-centers-roi))

**When Liquid Cooling Makes Sense:**
- Despite high upfront cost, liquid cooling pays for itself over time through:
  - Reduced power consumption
  - Longer hardware lifespan (due to lower thermal stress)
  - Lower maintenance costs
- Some government incentives and sustainability programs support liquid cooling adoption, improving ROI
- Source: ([Introl](https://introl.com/blog/liquid-vs-air-cooling-ai-data-centers))

### Power Usage Effectiveness (PUE) Measurements

**Two-Phase PUE Values:**
- Allied Control claimed PUE ratio of **1.02** (October 2015) through two-phase immersion cooling using 3M Novec 7100 fluid
- Traditional air-cooled data centers typically achieve PUE values **1.3 to 1.6**
- Two-phase cooling zones can achieve pPUE values as low as **1.05 to 1.10**
- Kanbur et al. found optimal PUE values of **1.15** at maximum operation loads
- In testing, partial power usage effectiveness (PPUE) of **1.042** achieved at 100% heat load (86 kW)
- Best practice examples have PUE values below 1.2, with lowest reaching **1.02** (BitFury's DC in Tbilisi)
- Source: ([Wikipedia](https://en.wikipedia.org/wiki/Power_usage_effectiveness), [Data Center Knowledge](https://www.datacenterknowledge.com/cooling/how-two-phase-liquid-cooling-is-solving-the-thermal-crisis), [MDPI](https://www.mdpi.com/1996-1073/14/5/1395))

**Comparative PUE Analysis:**
- Air cooling: Average PUE of **1.4-1.5**
- Liquid cooling: Average PUE of **1.1-1.2**
- Two-phase cooling: Average PUE of **1.5-1.6** with average Energy Savings Ratio (ESR) of **35%-40%**
- Many immersion cooling deployments achieve PUE **<1.05** by eliminating traditional CRAC and CRAH units
- Source: ([ScienceDirect](https://www.sciencedirect.com/science/article/pii/S2666123324000916), [NSF](https://par.nsf.gov/biblio/10654765-immersion-cooling-data-centers-comprehensive-review-benefits-challenges-future-directions))

**PUE Limitations:**
- PUE can be misleading when comparing efficiency of air and liquid cooling
- Total Usage Effectiveness (TUE) provides more accurate measure of efficiency
- Analysis by Vertiv and NVIDIA documented **18.1% reduction in facility power** and **10.2% reduction in total data center power** by transitioning from 100% air cooling to 75% direct-to-chip liquid cooling
- While total data center power reduced by more than 10%, PUE for facility dropped by only **3.3%**
- Source: ([Vertiv](https://www.vertiv.com/en-us/about/news-and-insights/articles/blog-posts/understanding-the-limitations-of-pue-in-evaluating-liquid-cooling-efficiency))

### OCP TCO Tool

The OCP Cooling Environments Project Total Cost of Ownership (TCO) tool helps model, evaluate and compare different datacenter power and cooling scenarios from TCO perspective with CAPEX and OPEX. It empowers users with open, unbiased, peer reviewed, transparent tools to help make more informed and data-driven decisions on power and cooling strategies. ([OCP](https://www.opencompute.org/ai-marketplace/products/735/total-cost-of-ownership-model-for-liquid-cooled-data-centers))

---

## 7. Components Required

### Coolant Distribution Units (CDUs)

**Core Function:**
- CDUs pump liquid or refrigerant through cold plates where coolant absorbs heat from server and evaporates
- Resulting vapor returns to CDU where it condenses back into liquid through heat exchange process
- Source: ([Vertiv](https://www.vertiv.com/en-asia/about/news-and-insights/articles/blog-posts/pumped-two-phase-direct-to-chip-cooling-advancing-ai-data-center-efficiency/))

**Two-Phase CDU Characteristics:**
- Unlike single-phase systems that depend on large volumes and high flow rates, Two-Phase CDUs deliver coolant directly to cold plates mounted on processors
- Liquid absorbs heat, vaporizes, and returns to CDU where it condenses and recirculates
- Creates continuous, closed-loop cycle maximizing thermal transfer while minimizing energy consumption
- System operates at much lower pressure, drastically reducing risk of leaks and minimizing maintenance
- Source: ([ACT](https://www.1-act.com/thermal-solutions/data-center-solutions/coolant-distribution-units/), [Boyd](https://www.boydcorp.com/thermal/liquid-cooling-systems/coolant-distribution-unit-cdu.html))

**Core Components:**
- CDU comprises heat exchanger, circulating pumps, coolant monitoring sensors, and programmable logic controller receiving inputs and feedback from all coolant monitoring devices
- Source: ([Supermicro](https://www.supermicro.com/en/glossary/cdu))

### Pumps

**Pump Types and Functions:**
- Primary and secondary pumps circulate coolant in both loops
- Secondary pumps push coolant through IT equipment
- Primary pumps circulate facility water through heat exchanger
- CDUs include integrated pumps that circulate coolant through secondary loop, ensuring consistent flow across direct-to-chip cold plates or rear-door heat exchangers
- High-availability CDUs typically equipped with redundant pumps and automatic switchover functionality to maintain continuous operation in case of component failure
- Source: ([nVent](https://www.nvent.com/en-us/data-solutions/coolant-distribution-unit), [Vertiv Understanding CDUs](https://www.vertiv.com/en-us/about/news-and-insights/articles/educational-articles/understanding-coolant-distribution-units-cdus-for-liquid-cooling/))

### Cold Plates

**Integration and Design:**
- CDUs integrate with cold plates custom designed to maximize interface with CPUs and GPUs through machined custom geometries and skylines for maximum heat transfer to liquid cooling system
- Four distinct forms of liquid cooling technologies used in data centers:
  1. Direct-to-chip liquid cooling employing single-phase microfin routed cold plates
  2. Direct-to-chip liquid cooling employing two-phase cold plates
- Source: ([Boyd](https://www.boydcorp.com/thermal/liquid-cooling-systems/coolant-distribution-unit-cdu.html))

**Performance:**
- ACT reports over **500 W/cm² heat flux capability** in two-phase cold plates
- CoolIT microchannel designs achieve **0.015°C/W thermal resistance**
- Source: ([ACT](https://www.1-act.com/resources/blog/data-center-cooling-systems/))

### Manifolds

**Function and Design:**
- High reliability manifolds safely direct liquid throughout server rack
- Cooling systems may consist of two row manifolds, eight rack manifolds, and multiple cooling loops equipped on thermal test vehicles
- Quick disconnect in-rack manifolds allow for rapid servicing and reduce leak risk, simplifying maintenance tasks
- Coolant handling manifolds enable up to 4 cooling loops to exit either top or bottom of CDU to support both raised floor and overhead configurations
- Source: ([nVent](https://www.nvent.com/en-us/data-solutions/coolant-distribution-unit), [ASME](https://asmedigitalcollection.asme.org/electronicpackaging/article/147/4/041109/1220069/Liquid-to-Liquid-In-Row-Coolant-Distribution-Unit))

### Additional Components

**Control and Monitoring:**
- Motorized valves regulate flow of coolant based on real-time system demands
- Valves work in coordination with control system to adjust for changing thermal loads, optimizing temperature differentials across heat exchanger
- CDUs equipped with filters, typically **50 microns**, to keep water supply contaminant and debris free and protect server cold plate integrity
- Most systems feature integrated leak detection, intelligent flow monitoring devices, and alarm features to maintain system performance and protect data center equipment
- Source: ([Eaton](https://www.eaton.com/us/en-us/catalog/thermal-management-solutions/coolant-distribution-unit-cdu.html), [Vertiv Understanding CDUs](https://www.vertiv.com/en-us/about/news-and-insights/articles/educational-articles/understanding-coolant-distribution-units-cdus-for-liquid-cooling/))

**Two-Phase Immersion Cooling Scenarios:**
- Utilize high-thermal-conductivity media such as electronic fluorinated fluids and mineral oils
- Source: ([Corestar Tech](https://www.corestartech.com/blog/what-is-coolant-distribution-units-cdu-for-data-center-cooling/))

---

## 8. Patents and Intellectual Property

### Company-Specific Patents

**ZutaCore:**
- Patented two-phase **HyperCool** technology
- Direct to chip, waterless, dielectric cooling solution
- Includes control software
- Source: ([ZutaCore](https://zutacore.com))

**JetCool:**
- **Patented microconvective cooling** (single-phase direct-to-chip liquid cooling technology)
- Foundation of product portfolio
- Innovative product suite uses patented microconvective cooling technology
- Source: ([JetCool](https://jetcool.com/technology/))

**Accelsius:**
- **NeuCool platform**: Two-phase, direct-to-chip cooling solution
- Accelsius Thermal Simulation Rack: **Patent-pending system** with Load Simulation Sleds
- Source: ([Innventure](https://www.innventure.com/news/accelsius-unveils-two-phase-cooling-reference-design-demonstrating-billions-in-potential-energy-savings))

**Asetek:**
- Patented liquid cooling technology in data centers
- Source: ([Fierce Network](https://www.fierce-network.com/cloud/cooling-tech-made-space-heads-data-centers-mikros-ceo-says))

**ATS:**
- 13 active patents on their technology
- Source: ([Fierce Network](https://www.fierce-network.com/cloud/cooling-tech-made-space-heads-data-centers-mikros-ceo-says))

### Foundational Patents

**U.S. Patent 11,464,137 (issued October 4, 2022):**
- **"Active control for two-phase cooling"**
- Provides controllable cooling for two-phase cooling systems
- Intrachip two-phase evaporative cooling minimizes thermal resistance and achieves lower temperature gradient between chip junction and local refrigerant temperature
- Lowers thermal resistance to about **0.04 C/W or less**
- Two-phase heat transfer involving small cavity channels in heat sink provides large heat transfer surface per unit of flow area near heat source
- Source: ([Justia Patents](https://patents.justia.com/patent/11464137))

**US20180076113A1 (IBM):**
- **"Chip package for two-phase cooling and assembly process thereof"**
- Covers devices with integrated cooling structures for two-phase cooling and methods of assembly
- Chip manifold can be affixed to chip with interface located between chip manifold and manifold cap
- Source: ([Google Patents](https://patents.google.com/patent/US20180076113A1/en))

**US20080128109A1 (Intel):**
- **"Two-phase cooling technology for electronic cooling applications"**
- Device to efficiently boil and distribute liquid vapor using high efficiency heat exchanger technology
- Incorporates high heat spreading capability of two-phase heat transfer physics
- Evaporation/boiling permits heat load from discrete component to be efficiently spread via vapor transport to entire HEX fin array
- Makes both spreading resistance and air-side convective resistance superior to air-cooled technologies alone
- Source: ([Google Patents](https://patents.google.com/patent/US20080128109A1/en))

**Patent Application 20230403822:**
- **"Scalable Two-Phase Cooling Plates"**
- Addresses historical limitations where microchannel configurations limited to small devices with sizes at ~cm length
- Challenge to implement effective two-phase cooling to large devices with length of ~10 cm due to scaling effects
- Invention made with government support under N00014-16-1-2956, awarded by Office of Naval Research (ONR)
- Source: ([Justia Patents](https://patents.justia.com/patent/20230403822))

**US6498725B2:**
- **"Method and two-phase spray cooling apparatus"**
- Compact, lightweight, and efficient evaporative spray cooling system for removing high heat fluxes
- For surfaces of devices such as micro-electronic chips, metal, mirrors, and lasers
- Uses expanding metastable two-phase flow and method of controlling spray for optimum heat flux removal
- Source: ([Google Patents](https://patents.google.com/patent/US6498725))

**US20200003500A1:**
- **"High performance two-phase cooling apparatus"**
- Two-phase cooling devices (including heat pipes, thermal ground planes, vapor chambers and thermosiphons)
- At least three substrates: metal with wicking structure, intermediate substrate and backplane
- Fluid contained within wicking structure and vapor cavity for transporting thermal energy, driven by capillary forces
- Source: ([Google Patents](https://patents.google.com/patent/US20200003500A1/en))

**US12051637B1:**
- **"Direct to chip application of boiling enhancement coating"**
- Source: ([Google Patents](https://patents.google.com/patent/US12051637B1/en))

### Patent Trends

**Industry-Wide Analysis:**
- Since 2015, technological shift from air to liquid cooling can be identified on level of patent activities
- Patent analysis indicates liquid cooling will continue to gain importance in future and could be combined with other approaches in form of hybrid cooling
- Development of wide band-gap power electronics over last two decades stimulated tremendous research into high-performance liquid cooling solutions for high heat flux (200–1000 W/cm²) power semiconductor devices
- Promising technologies separated into four categories:
  1. Single-phase jet impingement cooling
  2. Microchannel cooling
  3. Phase change or two-phase cooling
  4. Near-junction including direct chip cooling
- Source: ([ResearchGate](https://www.researchgate.net/publication/381272054_Analysis_of_Cooling_Technologies_in_the_Data_Center_Sector_on_the_Basis_of_Patent_Applications), [IEEE Xplore](https://ieeexplore.ieee.org/document/10041820/))

---

## 9. Market Share and Adoption

### Single-Phase vs Two-Phase Market Share (2025)

**By Coolant Type:**
- Single-phase hydrocarbon fluids accounted for **45.37%** of data center liquid cooling market size in 2025
- Two-phase fluorocarbon fluids set to expand at **25.64% CAGR**
- Source: ([Globe Newswire](https://www.globenewswire.com/news-release/2026/02/04/3232076/28124/en/Data-Center-Liquid-Cooling-Market-Report-2026-16-16-Bn-Opportunities-Trends-Competitive-Landscape-Strategies-and-Forecasts-2020-2025-2025-2030F-2035F.html))

**By Cooling Method:**
- Single-phase direct liquid cooling expected to remain prevailing architecture for most deployments through end of decade
- Single-phase cooling segment expected to account for largest market share during forecast period
- Delivers effective results through dependable performance and straightforward implementation
- Source: ([Mordor Intelligence](https://www.mordorintelligence.com/industry-reports/data-center-liquid-cooling-market))

**Two-Phase Growth Drivers:**
- Two-phase fluids growing faster than single-phase coolants
- Provide higher heat-transfer coefficients enabling operators to serve AI racks exceeding 30 kW
- Source: ([Mordor Intelligence](https://www.mordorintelligence.com/industry-reports/data-center-liquid-cooling-market))

### Two-Phase Immersion Cooling Market Size

- Global two-phase data center liquid immersion cooling market size valued at **USD 431.4 million in 2025**
- Projected to grow from **USD 496.7 million in 2026** to **USD 1612.4 million by 2034**
- Exhibiting CAGR of **15.90%**
- Source: ([Fortune Business Insights](https://www.fortunebusinessinsights.com/two-phase-data-center-liquid-immersion-cooling-market-113122))

### Overall Market Growth (2025-2030)

- Single phase cooling market projected to grow by **$7 billion**
- Two phase cooling market projected to grow by **$4 billion**
- Over next five years from 2025 to 2030
- Source: ([Globe Newswire](https://www.globenewswire.com/news-release/2026/02/04/3232076/28124/en/Data-Center-Liquid-Cooling-Market-Report-2026-16-16-Bn-Opportunities-Trends-Competitive-Landscape-Strategies-and-Forecasts-2020-2025-2025-2030F-2035F.html))

### Total Liquid Cooling Market

- Data center liquid cooling market witnessing robust expansion
- Anticipated to grow from **$5.1 billion in 2025** to **$6.41 billion in 2026**
- Representing compound annual growth rate (CAGR) of **25.7%**
- Projected to expand from **USD 6.6 billion in 2026** to **USD 38.4 billion by 2033**
- Registering CAGR of **28.7%**
- Source: ([Globe Newswire](https://www.globenewswire.com/news-release/2026/02/04/3232076/28124/en/Data-Center-Liquid-Cooling-Market-Report-2026-16-16-Bn-Opportunities-Trends-Competitive-Landscape-Strategies-and-Forecasts-2020-2025-2025-2030F-2035F.html), [Globe Newswire Feb 2026](https://www.globenewswire.com/news-release/2026/02/17/3239044/0/en/Data-Center-Liquid-Cooling-Market-to-Witness-28-7-CAGR-Driven-by-AI-Adoption-Investments-and-Sustainability-Targets.html))

### Technology Breakdown

**Direct-to-Chip Dominance:**
- Direct-to-chip systems hold largest share at **42.85%** of 2025 revenue
- Direct-to-chip solutions continue to dominate because they retrofit into existing racks
- Two-phase immersion systems advancing fastest as operators pursue still higher thermal efficiencies
- Source: ([Globe Newswire](https://www.globenewswire.com/news-release/2026/02/04/3232076/28124/en/Data-Center-Liquid-Cooling-Market-Report-2026-16-16-Bn-Opportunities-Trends-Competitive-Landscape-Strategies-and-Forecasts-2020-2025-2025-2030F-2035F.html))

### Regional Highlights for Two-Phase Immersion

**North America:**
- Dominated global two-phase liquid immersion cooling market with share of **41.30% in 2025**
- Source: ([Fortune Business Insights](https://www.fortunebusinessinsights.com/two-phase-data-center-liquid-immersion-cooling-market-113122))

**Europe:**
- Contributed approximately **USD 122.1 million** to global two-phase immersion market in 2025
- Accounting for **28.30%** share
- Expected to reach **USD 140.3 million in 2026**
- Source: ([Fortune Business Insights](https://www.fortunebusinessinsights.com/two-phase-data-center-liquid-immersion-cooling-market-113122))

### Future Outlook

**2026-2027 Predictions:**
- Single-phase immersion achieving mainstream acceptance in hyperscale AI infrastructure
- **120-150 MW annual deployment rate** (up from 80-100 MW in 2024-2025)
- OEM-integrated solutions from Dell, HPE, and Lenovo offering factory-validated immersion-ready servers
- Source: ([Energy Solutions](https://energy-solutions.co/articles/sub/data-center-cooling-liquid-immersion-vs-air))

**2028-2030 Outlook:**
- Two-phase immersion expected to transition from niche HPC applications to broader AI training market
- As fluid costs decline (USD 35-60/liter from USD 50-90) and material compatibility improves
- Source: ([Energy Solutions](https://energy-solutions.co/articles/sub/data-center-cooling-liquid-immersion-vs-air))

**Current Standard (2026):**
- Cold plate technology (direct liquid cooling / DLC) is the **2026 standard** of enterprise AI deployments
- In this design, chip liquid cold plate is put on processor through which coolant is circulated
- Source: ([AC/DC EC Fan](https://www.acdcecfan.com/server-cooling-solutions-for-2026/))

---

## 10. Challenges and Reliability

### Leak Detection and Prevention

**Leak Detection Requirements:**
- Leak detection systems require integration with facility-wide safety networks, triggering immediate containment protocols and system isolation procedures
- Two-phase systems demand more sophisticated monitoring due to phase change dynamics:
  - Pressure-temperature correlation tracking
  - Vapor quality measurements
- Source: ([Quality Magazine](https://www.qualitymag.com/articles/99290-ensuring-reliability-in-data-centers-the-evolving-role-of-leak-testing))

**Best Practices:**
- Leaks tend to occur at couplings and joints, not at piping walls
- Best practice recommends specifying leak detection sensors for piping most prone to leaks:
  - At connections (couplings, welds, threaded, crimped)
  - In drip pans
  - By cooling coils
  - By heat exchangers
- Refrigerant leak detection sensors should be installed in areas where leak would gather and trigger alarm to start safety measures
- Release mitigation controls, such as automatic shut-off valves, can limit amount of released refrigerant
- Handheld refrigerant leak detectors with long, flexible probe can locate low ppm level leaks for servicing and maintenance
- Source: ([IoThrifty](https://www.iothrifty.com/blogs/news/data-center-leak-detection-and-monitoring-for-liquid-cooled-systems))

### Reliability Testing Challenges

**Fluid Degradation Monitoring:**
- Chemical stability of dielectric fluids under continuous operation
- Potential contamination pathways
- Effects of fluid aging on cooling performance
- Lack of standardized assessment protocols creates significant uncertainty regarding maintenance schedules and operational economics
- Source: ([Eureka PatSnap](https://eureka.patsnap.com/report-reliability-testing-protocols-for-two-phase-immersion-data-centers))

**Electrical Safety:**
- Electrical safety verification under immersion conditions remains problematic
- Current electrical safety standards developed primarily for air-cooled environments
- Require substantial adaptation for immersion scenarios
- Interaction between electrical components and dielectric fluids during fault conditions or power surges demands specialized testing approaches not yet formalized in industry standards
- Source: ([Eureka PatSnap](https://eureka.patsnap.com/report-reliability-testing-protocols-for-two-phase-immersion-data-centers))

**Pressure Testing:**
- Static pressure proofs don't show how connections behave over time
- Priority is pressure cycling that represents expected life, not impulse severity
- Use pressure-cycling pattern that looks like system's operating reality
- Run test with actual coolant at realistic temperatures
- Pick cycle count aligned to service life
- Source: ([Boyd](https://www.boydcorp.com/blog/leak-free-cooling-approach-to-prevent-liquid-cooling-loop-leaks.html))

### Regulatory and Environmental Challenges

**Two-Phase Specific Regulations:**
- Two-phase immersion cooling systems encounter additional regulatory complexity due to use of phase-change materials involving volatile organic compounds
- Montreal Protocol's restrictions on ozone-depleting substances directly impact selection of working fluids
- Regional air quality regulations limit emissions during normal operation and maintenance procedures
- Many jurisdictions require closed-loop systems with leak detection mechanisms to prevent atmospheric release of cooling fluids
- Source: ([OCP](https://www.opencompute.org/documents/2p-refrigerant-based-dlc-wp-v1-pdf-1))

**F-gas Regulation:**
- EU's F-gas regulation introduced requirements for regular leak checks of equipment containing HFCs
- Frequency depends on CO2 equivalent of fluid quantity in system
- Detecting leaks crucial for conserving refrigerants, protecting equipment, improving performance, reducing emissions, and ensuring occupational safety
- Source: ([Envigilance](https://envigilance.com/water-leak-detection/chilled-water-leak-detection/))

### Maintenance Advantages of Two-Phase Systems

**Lower Pressure Operation:**
- System operates at much lower pressure, drastically reducing risk of leaks and minimizing maintenance
- In unlikely event of leak, fluid simply evaporates, causing no harm to IT equipment (unlike water-based systems where leaks can be disastrous)
- Source: ([ZutaCore Blog](https://blog.zutacore.com/zutacore-blog/what-is-closed-loop-two-phased-liquid-cooling-system))

**Closed-Loop Benefits:**
- In closed-loop liquid cooling system, cooling fluid contained within sealed environment minimizing need for regular maintenance
- Liquid does not come into contact with external contaminants, almost never needs to be replaced or refilled
- Self-sustaining design ensures liquid's level, integrity, and viscosity remain stable indefinitely
- Translates into more reliable and low-maintenance cooling solution
- Source: ([ZutaCore Blog](https://blog.zutacore.com/zutacore-blog/what-is-closed-loop-two-phased-liquid-cooling-system))

### Adoption Barriers

**Market Barriers:**
- High initial capital expenditure: Immersion cooling installations typically cost **30-50% more** than traditional cooling systems initially
- Concerns about fluid maintenance
- Compatibility with IT equipment
- Lack of standardized reliability testing protocols impede faster market adoption
- Source: ([Eureka PatSnap](https://eureka.patsnap.com/report-reliability-testing-protocols-for-two-phase-immersion-data-centers))

**Downtime Costs:**
- Downtime is one of most expensive challenges for data-center managers
- Single leak can interrupt cooling and lead to service outages costing **hundreds of thousands of dollars per hour**
- For hyperscale operators running AI supercomputing infrastructure, costs can be even higher
- Source: ([IoThrifty](https://www.iothrifty.com/blogs/news/data-center-leak-detection-and-monitoring-for-liquid-cooled-systems))

---

## 11. Comparison: Pumped vs Passive Two-Phase

### Pumped Two-Phase (P2P) Systems

**How It Works:**
- Typically, liquid near saturation is pumped into cold plate where it starts to boil
- Cools electronics and stores energy in latent heat of fluid
- Two-phase (liquid and vapor) fluid flows to condenser where heat is removed, condensing vapor
- Single-phase (liquid) exits condenser and cycle repeats
- Source: ([Thermal Live](https://thermal.live/2019/passive-and-active-two-phase-cooling-for-power-electronics-qa/))

**Orientation Flexibility:**
- Evaporators (cold plates) can operate in all orientations
- Horizontal, vertical flow up, and vertical flow down all demonstrated simultaneously
- Military aircraft can have acceleration in any direction
- Spacecraft operate in microgravity
- With proper design, P2P cooling systems can operate on both aircraft and spacecraft
- Source: ([ACT](https://www.1-act.com/resources/pumped-two-phase-cooling/))

**Heat Flux Capability:**
- ACT demonstrated heat fluxes well over **250 W/cm²** for pumped refrigerant systems
- Source: ([ACT](https://www.1-act.com/resources/pumped-two-phase-cooling/))

**Coolant Sensitivity:**
- Pump-driven system much more robust
- Can typically handle lower coolant level
- Source: ([ACT](https://www.1-act.com/resources/pumped-two-phase-cooling/))

**Reliability Considerations:**
- Has moving parts (pumps) that can fail
- Source: ([ACT](https://www.1-act.com/resources/pumped-two-phase-cooling/))

### Passive Thermosiphon Systems

**How It Works:**
- Two-phase loop thermosyphon (TPLT) can deliver high heat loads (up to **25 kW**) over long distances without use of pump
- Natural circulation heat transfer device driven by fluid density difference and gravity
- Condenser must be placed above evaporator to favor buoyantly driven passive flow circulation
- Source: ([Boyd](https://www.boydcorp.com/thermal/two-phase-cooling/thermosiphons.html), [Wikipedia](https://en.wikipedia.org/wiki/Thermosiphon))

**Orientation Requirements:**
- Thermosiphons need consistent gravitational pull to operate since they are wickless
- Condenser must be placed above evaporator
- Source: ([ACT](https://www.1-act.com/resources/pumped-two-phase-cooling/))

**Reliability:**
- Thermosiphons are passive, two-phase thermal management components or systems that do not require mechanical pumps or other moving parts within fluid loop
- Source: ([Boyd](https://www.boydcorp.com/thermal/two-phase-cooling/thermosiphons.html))

**Heat Flux Capability:**
- With internal fin structure in LTS evaporator, heat fluxes greater than **100 W/cm²** demonstrated
- One of highest heat flux capable passive cooling solutions
- Source: ([ACT](https://www.1-act.com/resources/pumped-two-phase-cooling/))

**Coolant Sensitivity:**
- Thermosiphon systems very sensitive to low coolant level
- Losing only small amount of coolant stops circulation
- Source: ([ACT](https://www.1-act.com/resources/pumped-two-phase-cooling/))

### Applications and Use Cases

**Pumped Two-Phase Applications:**
- Military aircraft
- Spacecraft (microgravity environments)
- High-density AI data centers
- Applications requiring orientation flexibility
- Source: ([ACT](https://www.1-act.com/resources/pumped-two-phase-cooling/))

**Passive Thermosiphon Applications:**
- Two-Phase Thermosiphon (TPT) systems provide effective cooling for data centers through natural circulation driven by gravity and phase change of refrigerants
- Facilitates efficient heat transfer without moving components
- Improved reliability and energy efficiency
- Well-suited for medium to high-density power applications
- Source: ([Springer](https://link.springer.com/article/10.1186/s44147-025-00833-3))

### Energy Efficiency

**Passive Systems:**
- Studies shown heat pipes and two-phase thermosiphons can substantially reduce energy consumption
- Achieving energy saving ratio (ESR) of up to **38.7%**
- Passive two-phase cooling systems particularly favored because they eliminate need for mechanical components, thereby optimizing energy use
- Source: ([Springer](https://link.springer.com/article/10.1186/s44147-025-00833-3))

**Comparison to Single-Phase:**
- Pumped single-phase liquid loop would require substantial amount of fluid flow to achieve isothermal cooling
- Results in higher energy consumption, higher pump noise, and increased reliability concerns
- Source: ([Thermal Live](https://thermal.live/2019/passive-and-active-two-phase-cooling-for-power-electronics-qa/))

---

## 12. Additional Context

### Server OEM Support

**Dell and Supermicro:**
- Dell and Supermicro say they can cut data center power consumption by as much as **one third** by using liquid cooling directly on GPUs in racks
- Dell and Supermicro are leading suppliers of liquid-cooled racks to high-end data centers
- Ramping up production to meet expected surge in demand
- Supermicro says it can deliver over **a thousand racks per month** worldwide
- Source: ([EE Times](https://www.eetimes.com/dell-supermicro-rein-in-data-center-power/))

**Factory-Validated Support:**
- As of 2025, select **Dell PowerEdge, HPE ProLiant, Supermicro, and NVIDIA HGX servers** offer factory-validated immersion support
- Source: ([Energy Solutions](https://energy-solutions.co/articles/sub/data-center-cooling-liquid-immersion-vs-air))

### When Air Cooling Fails

- Air cooling fails at **41.3kW per rack**
- Liquid cooling handles **200kW+ per rack**
- If racks stay below 15kW, well-designed hot aisle/cold aisle containment system with precision CRAC units works fine
- Source: ([Introl](https://introl.com/blog/liquid-vs-air-cooling-ai-data-centers))

### Thermal Management for Next-Gen AI Chips

**Modern AI Chipsets:**
- Modern AI chipsets now feature thermal design power (TDP) ratings exceeding 1,000 watts:
  - Gaudi HL-2080: **600W**
  - AMD MI300X: **750W**
  - NVIDIA Blackwell GPU: **2000W**
- Source: ([Vertiv](https://www.vertiv.com/en-us/about/news-and-insights/articles/blog-posts/pumped-two-phase-direct-to-chip-cooling-advancing-ai-data-center-efficiency/))

**NVIDIA GB200 Specifics:**
- Grace-Blackwell Superchip (GB200) combines 72 Arm core CPU with pair of **1,200W GPUs**
- Back-of-envelope calculation suggests under peak load capable of drawing **2,700W**
- In B200 phase, each chip consumes 1200W, requiring more cooling space
- In GB200 Bianca board scenario with power consumption of 2700W, air velocity insufficient to provide effective cooling within 19-inch rack
- Necessitating liquid cooling solution allowing system's volume to be controlled within 1-2U range
- Source: ([FiberMall](https://www.fibermall.com/blog/in-depth-analysis-for-nvidia-gb200.htm))

---

## Sources Summary

This research compiled facts from **100+ sources** including:
- Company websites and press releases (JetCool, ZutaCore, Accelsius, LiquidStack, Vertiv, Asetek, CoolIT, Boyd, Motivair)
- Market research firms (Globe Newswire, Mordor Intelligence, Fortune Business Insights, Dell'Oro Group)
- Industry publications (Data Center Dynamics, Data Center Knowledge, Data Center Frontier, Storage Review)
- Technical sources (ScienceDirect, IEEE, MDPI, ACT, Boyd technical documentation)
- Patent databases (Justia Patents, Google Patents)
- Hyperscaler and OEM sources (NVIDIA, Intel, Microsoft, Dell, Supermicro)
- Industry blogs and analysis (Introl, EnkiAI, ByteBridge, Schneider Electric)

**Research completed:** April 12, 2026
