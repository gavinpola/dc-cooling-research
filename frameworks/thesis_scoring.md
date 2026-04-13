# Thesis Scoring Framework

## Purpose
Objective, quantitative comparison of competing theses about data center cooling futures. Enables apples-to-apples comparison and clear recommendation.

## Scoring Dimensions

| Dimension | Weight | Description |
|-----------|--------|-------------|
| Technical Feasibility | 20% | Does physics support this at scale? Is it proven? |
| Market Timing | 15% | When is this commercially viable? How certain? |
| Capital Efficiency | 15% | What's the cost to deploy per MW of cooling? |
| Operational Cost | 15% | Ongoing costs: energy, maintenance, personnel |
| Scalability | 15% | Can it handle exponential AI compute growth? |
| Competitive Moat | 10% | Can a startup defend market position? |
| Risk Profile | 10% | What are failure modes and their probability? |

## Scoring Rubric

### Technical Feasibility (20%)

| Score | Criteria |
|-------|----------|
| 5 | Proven at scale, deployed in production at multiple hyperscalers |
| 4 | Proven in pilot deployments, clear path to scale |
| 3 | Lab-validated, some real-world deployment |
| 2 | Theoretical feasibility, limited real-world evidence |
| 1 | Unproven, significant physics/engineering questions |

### Market Timing (15%)

| Score | Criteria |
|-------|----------|
| 5 | Commercially viable NOW, active market |
| 4 | Viable in 1-2 years, clear catalysts |
| 3 | Viable in 3-5 years, dependent on known developments |
| 2 | Viable in 5-10 years, significant uncertainty |
| 1 | 10+ years out, or may never be viable |

### Capital Efficiency (15%)

| Score | Criteria |
|-------|----------|
| 5 | Lower capex than current solutions |
| 4 | Comparable capex to current solutions |
| 3 | 25-50% premium over current solutions |
| 2 | 50-100% premium over current solutions |
| 1 | >100% premium, cost-prohibitive |

### Operational Cost (15%)

| Score | Criteria |
|-------|----------|
| 5 | Significantly lower opex (>30% reduction) |
| 4 | Moderately lower opex (10-30% reduction) |
| 3 | Comparable opex to current solutions |
| 2 | Higher opex (10-30% increase) |
| 1 | Much higher opex (>30% increase) |

### Scalability (15%)

| Score | Criteria |
|-------|----------|
| 5 | Can scale to handle 10x current compute demand |
| 4 | Can scale to handle 5x current compute demand |
| 3 | Can scale to handle 2-3x current demand |
| 2 | Limited scalability, niche applications |
| 1 | Does not scale, dead end |

### Competitive Moat (10%)

| Score | Criteria |
|-------|----------|
| 5 | Strong IP, high switching costs, network effects |
| 4 | Good IP and integration complexity |
| 3 | Some differentiation, moderate switching costs |
| 2 | Low differentiation, easy to replicate |
| 1 | Commodity, no defensibility |

### Risk Profile (10%)

| Score | Criteria |
|-------|----------|
| 5 | Low risk, proven technology, clear market |
| 4 | Moderate risk, some technical/market uncertainty |
| 3 | Elevated risk, multiple dependencies |
| 2 | High risk, significant unknowns |
| 1 | Very high risk, many failure modes |

## Calculation

```
Weighted Score =
    (Technical × 0.20) +
    (Timing × 0.15) +
    (CapEx × 0.15) +
    (OpEx × 0.15) +
    (Scale × 0.15) +
    (Moat × 0.10) +
    (Risk × 0.10)
```

**Max Score: 5.00**

## Interpretation

| Score Range | Interpretation |
|-------------|---------------|
| 4.5 - 5.0 | Strong bet - high confidence |
| 4.0 - 4.4 | Good bet - solid fundamentals |
| 3.5 - 3.9 | Mixed - watch for developments |
| 3.0 - 3.4 | Weak - significant concerns |
| < 3.0 | Avoid - too many problems |

## Scoring Template

```markdown
## Thesis [A/B/C]: [Name]

| Dimension | Score | Rationale | Sources |
|-----------|-------|-----------|---------|
| Technical Feasibility | X | ... | [1] |
| Market Timing | X | ... | [2] |
| Capital Efficiency | X | ... | [3] |
| Operational Cost | X | ... | [4] |
| Scalability | X | ... | [5] |
| Competitive Moat | X | ... | [6] |
| Risk Profile | X | ... | [7] |

**Weighted Score: X.XX / 5.00**

### Score Breakdown
- Technical (20%): X × 0.20 = X.XX
- Timing (15%): X × 0.15 = X.XX
- CapEx (15%): X × 0.15 = X.XX
- OpEx (15%): X × 0.15 = X.XX
- Scale (15%): X × 0.15 = X.XX
- Moat (10%): X × 0.10 = X.XX
- Risk (10%): X × 0.10 = X.XX
- **Total: X.XX**
```

## Comparative Summary Template

```markdown
# Thesis Comparison Summary

| Thesis | Score | Rank | Key Strength | Key Weakness |
|--------|-------|------|--------------|--------------|
| A: 2-Phase | X.XX | X | ... | ... |
| B: Ambient | X.XX | X | ... | ... |
| C: Space | X.XX | X | ... | ... |

## Verdict
[Which thesis wins and why]
```
