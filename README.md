# CDC Vaccination Hot-Spot Analysis: Pneumococcal Vaccine Coverage, Adults 65+ (2020)

An analysis of CDC adult vaccination data to find where older adults are least likely to be vaccinated against pneumococcal disease, presented as a briefing for a CDC Director.

**Course:** BAN5650, Clark University (MBA, Business Analytics), group project (Team Hollywood)
**Tools:** Tableau, Excel, PowerPoint
**Files:** the presentation (PDF) is in this repo

## The question
Where should a CDC Director focus attention? I identified the places and groups where pneumococcal vaccine coverage among adults 65 and older falls clearly below normal in 2020, and defined what "normal" means.

## The data
- **Source:** CDC adult vaccination coverage (public dataset, about 50,000 rows)
- **Filters:** Dimension Type = ">= 65 years", Survey Year = 2020
- **Vaccine:** Pneumococcal
- **Geography:** states and territories, then counties
- **Key fields:** Geography, Geography Type, Dimension, Estimate (%), 95% CI (%), Sample Size, FIPS

## What counts as "normal"
- **Benchmark:** the national coverage rate, **70.3%** (95% CI 69.6 to 71.0, 124,768 respondents).
- **Hot spot rule:** a place qualifies only if its entire 95% confidence interval falls below 70.3%. That way the shortfall is real and not just sampling noise.
- **Exclusions:** sub-state areas (New York City, Cook County, Philadelphia) were left out, so cities are not compared with whole states.
- **Race comparisons** use the national White non-Hispanic rate of 73.5% as the benchmark.
- County results use **FIPS codes**, because county names repeat across states (for example, Worcester County exists in both MA and MD).

## Findings: the five hot spots
1. **Puerto Rico and Guam:** fewer than one in three older adults vaccinated. Puerto Rico 31.0% (39.3 points below national) and Guam 33.4% (36.9 points below).
2. **Hawaii:** 61.9%, the lowest of the 50 states.
3. **Florida:** 64.3%, the largest sample of any low-coverage state (n = 4,621).
4. **Mississippi:** 66.6% at state level, but **9 of the 15 lowest-coverage counties in the US are in Mississippi**, mostly next to each other in the Delta (Leflore, Holmes, Washington, Humphreys, Sunflower), from a state with only 2.6% of US counties.
5. **Hispanic older adults:** more than 20 points behind White residents inside the same state, in both New Jersey and Florida. Several hot spots (Puerto Rico, New Jersey, Florida) have large Hispanic populations, which is where I would look next.

## Limitations
- Coverage figures are survey estimates. Smaller areas such as Guam have wide confidence intervals.
- The analysis covers one survey year (2020).
- "Normal" is the national rate chosen for this assignment, not an official CDC target.
- This shows where coverage is low, not why. Explaining causes would need other data.

## What I did
[WRITE 2-3 LINES: your part of the group project]
