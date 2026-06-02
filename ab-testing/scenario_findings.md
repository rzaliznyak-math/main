# A/B Test Stopping Rules — Scenario Analysis

*Generated 2026-06-01 | 100,000 sims (100k) or 500,000 sims (500k for σ=0.5, CR≤10%) | 50 thresholds α ∈ [0.01, 0.50]*

**Dimensions:** Baseline CR (5%, 10%, 30%, 65%) × Post-Test N (100k, 250k, 500k, 2M) × Expected Effects σ (0.5, 1.0, 2.0)

**Metrics at optimal α per strategy:**
- **Projected Mean** — long-term conversion rate (test + post-test users, winner deployed)
- **Marginal Events** — incremental conversions vs no test
- **Best Rate** — % of sims where the true winner was selected
- **Avg Days** — average stopping day

---

## 1. Raw Results — All Scenarios at Optimal α

| CR | σ | PTN | Strategy | Opt α | Proj Mean | Marginal | Best Rate | Avg Days |
|---|---|---|---|---|---|---|---|---|
| 5% | 0.5 | 100k | Peeking + Best | 0.12 | 5.0011% | 2 | 55.5% | 14.4 |
| 5% | 0.5 | 100k | Peeking | 0.27 | 5.0011% | 2 | 54.4% | 9.5 |
| 5% | 0.5 | 250k | Peeking + Best | 0.14 | 5.0014% | 5 | 55.4% | 13.6 |
| 5% | 0.5 | 250k | Peeking | 0.20 | 5.0012% | 4 | 54.6% | 11.6 |
| 5% | 0.5 | 500k | Peeking + Best | 0.12 | 5.0015% | 9 | 55.5% | 14.4 |
| 5% | 0.5 | 500k | Peeking | 0.24 | 5.0013% | 8 | 54.5% | 10.3 |
| 5% | 0.5 | 2.0MM | Peeking + Best | 0.02 | 5.0017% | 35 | 55.8% | 18.8 |
| 5% | 0.5 | 2.0MM | Peeking | 0.22 | 5.0014% | 30 | 54.6% | 10.9 |
| 5% | 1.0 | 100k | Peeking + Best | 0.17 | 5.0050% | 10 | 60.3% | 12.4 |
| 5% | 1.0 | 100k | Peeking | 0.25 | 5.0046% | 9 | 59.0% | 10.0 |
| 5% | 1.0 | 250k | Peeking + Best | 0.14 | 5.0056% | 20 | 60.4% | 13.5 |
| 5% | 1.0 | 250k | Peeking | 0.24 | 5.0050% | 18 | 59.1% | 10.2 |
| 5% | 1.0 | 500k | Peeking + Best | 0.07 | 5.0060% | 36 | 60.8% | 16.2 |
| 5% | 1.0 | 500k | Peeking | 0.25 | 5.0053% | 32 | 59.0% | 10.0 |
| 5% | 1.0 | 2.0MM | Peeking + Best | 0.04 | 5.0067% | 141 | 60.9% | 17.6 |
| 5% | 1.0 | 2.0MM | Peeking | 0.22 | 5.0056% | 119 | 59.1% | 10.8 |
| 5% | 2.0 | 100k | Peeking + Best | 0.15 | 5.0166% | 33 | 68.9% | 12.7 |
| 5% | 2.0 | 100k | Peeking | 0.25 | 5.0159% | 32 | 66.6% | 9.7 |
| 5% | 2.0 | 250k | Peeking + Best | 0.11 | 5.0192% | 67 | 69.5% | 14.1 |
| 5% | 2.0 | 250k | Peeking | 0.20 | 5.0178% | 62 | 66.6% | 11.1 |
| 5% | 2.0 | 500k | Peeking + Best | 0.05 | 5.0209% | 125 | 70.0% | 16.6 |
| 5% | 2.0 | 500k | Peeking | 0.22 | 5.0188% | 113 | 66.7% | 10.5 |
| 5% | 2.0 | 2.0MM | Peeking + Best | 0.05 | 5.0228% | 479 | 70.0% | 16.6 |
| 5% | 2.0 | 2.0MM | Peeking | 0.23 | 5.0198% | 416 | 66.7% | 10.3 |
| 10% | 0.5 | 100k | Peeking + Best | 0.18 | 10.0033% | 7 | 57.4% | 12.2 |
| 10% | 0.5 | 100k | Peeking | 0.21 | 10.0031% | 6 | 56.6% | 11.2 |
| 10% | 0.5 | 250k | Peeking + Best | 0.07 | 10.0039% | 14 | 58.0% | 16.4 |
| 10% | 0.5 | 250k | Peeking | 0.23 | 10.0035% | 12 | 56.6% | 10.6 |
| 10% | 0.5 | 500k | Peeking + Best | 0.06 | 10.0044% | 26 | 58.0% | 16.8 |
| 10% | 0.5 | 500k | Peeking | 0.23 | 10.0038% | 23 | 56.6% | 10.6 |
| 10% | 0.5 | 2.0MM | Peeking + Best | 0.02 | 10.0049% | 102 | 58.1% | 18.7 |
| 10% | 0.5 | 2.0MM | Peeking | 0.23 | 10.0040% | 85 | 56.6% | 10.6 |
| 10% | 1.0 | 100k | Peeking + Best | 0.15 | 10.0128% | 26 | 64.6% | 13.0 |
| 10% | 1.0 | 100k | Peeking | 0.24 | 10.0121% | 24 | 62.6% | 10.2 |
| 10% | 1.0 | 250k | Peeking + Best | 0.10 | 10.0152% | 53 | 65.1% | 14.8 |
| 10% | 1.0 | 250k | Peeking | 0.22 | 10.0139% | 49 | 62.7% | 10.7 |
| 10% | 1.0 | 500k | Peeking + Best | 0.09 | 10.0166% | 100 | 65.2% | 15.2 |
| 10% | 1.0 | 500k | Peeking | 0.22 | 10.0145% | 87 | 62.7% | 10.7 |
| 10% | 1.0 | 2.0MM | Peeking + Best | 0.07 | 10.0180% | 379 | 65.4% | 16.1 |
| 10% | 1.0 | 2.0MM | Peeking | 0.20 | 10.0152% | 320 | 62.7% | 11.3 |
| 10% | 2.0 | 100k | Peeking + Best | 0.17 | 10.0415% | 83 | 74.2% | 11.6 |
| 10% | 2.0 | 100k | Peeking | 0.23 | 10.0402% | 80 | 72.0% | 10.0 |
| 10% | 2.0 | 250k | Peeking + Best | 0.12 | 10.0478% | 167 | 75.0% | 13.2 |
| 10% | 2.0 | 250k | Peeking | 0.23 | 10.0448% | 157 | 72.0% | 10.0 |
| 10% | 2.0 | 500k | Peeking + Best | 0.09 | 10.0514% | 309 | 75.3% | 14.2 |
| 10% | 2.0 | 500k | Peeking | 0.20 | 10.0474% | 285 | 72.1% | 10.7 |
| 10% | 2.0 | 2.0MM | Peeking + Best | 0.03 | 10.0558% | 1,172 | 75.7% | 17.0 |
| 10% | 2.0 | 2.0MM | Peeking | 0.20 | 10.0501% | 1,053 | 72.1% | 10.7 |
| 30% | 0.5 | 100k | Peeking + Best | 0.20 | 30.0190% | 38 | 63.5% | 11.3 |
| 30% | 0.5 | 100k | Peeking | 0.23 | 30.0184% | 37 | 62.5% | 10.4 |
| 30% | 0.5 | 250k | Peeking + Best | 0.09 | 30.0220% | 77 | 64.6% | 15.2 |
| 30% | 0.5 | 250k | Peeking | 0.23 | 30.0203% | 71 | 62.5% | 10.4 |
| 30% | 0.5 | 500k | Peeking + Best | 0.07 | 30.0240% | 144 | 64.8% | 16.0 |
| 30% | 0.5 | 500k | Peeking | 0.21 | 30.0208% | 125 | 62.5% | 11.0 |
| 30% | 0.5 | 2.0MM | Peeking + Best | 0.01 | 30.0262% | 549 | 65.1% | 19.1 |
| 30% | 0.5 | 2.0MM | Peeking | 0.21 | 30.0224% | 471 | 62.5% | 11.0 |
| 30% | 1.0 | 100k | Peeking + Best | 0.17 | 30.0619% | 124 | 73.8% | 11.6 |
| 30% | 1.0 | 100k | Peeking | 0.22 | 30.0602% | 120 | 71.9% | 10.2 |
| 30% | 1.0 | 250k | Peeking + Best | 0.12 | 30.0706% | 247 | 74.5% | 13.2 |
| 30% | 1.0 | 250k | Peeking | 0.22 | 30.0670% | 235 | 71.9% | 10.2 |
| 30% | 1.0 | 500k | Peeking + Best | 0.08 | 30.0762% | 457 | 74.9% | 14.7 |
| 30% | 1.0 | 500k | Peeking | 0.21 | 30.0710% | 426 | 72.0% | 10.5 |
| 30% | 1.0 | 2.0MM | Peeking + Best | 0.03 | 30.0822% | 1,726 | 75.2% | 17.0 |
| 30% | 1.0 | 2.0MM | Peeking | 0.21 | 30.0747% | 1,569 | 72.0% | 10.5 |
| 30% | 2.0 | 100k | Peeking + Best | 0.22 | 30.1667% | 333 | 83.3% | 9.3 |
| 30% | 2.0 | 100k | Peeking | 0.22 | 30.1653% | 331 | 82.4% | 9.3 |
| 30% | 2.0 | 250k | Peeking + Best | 0.14 | 30.1856% | 650 | 84.5% | 10.9 |
| 30% | 2.0 | 250k | Peeking | 0.22 | 30.1816% | 636 | 82.4% | 9.3 |
| 30% | 2.0 | 500k | Peeking + Best | 0.11 | 30.1973% | 1,184 | 84.9% | 11.7 |
| 30% | 2.0 | 500k | Peeking | 0.22 | 30.1913% | 1,148 | 82.4% | 9.3 |
| 30% | 2.0 | 2.0MM | Peeking + Best | 0.05 | 30.2098% | 4,406 | 85.5% | 13.8 |
| 30% | 2.0 | 2.0MM | Peeking | 0.21 | 30.2006% | 4,212 | 82.5% | 9.5 |
| 65% | 0.5 | 100k | Peeking + Best | 0.17 | 65.0682% | 136 | 74.5% | 11.5 |
| 65% | 0.5 | 100k | Peeking | 0.22 | 65.0662% | 132 | 72.4% | 10.2 |
| 65% | 0.5 | 250k | Peeking + Best | 0.13 | 65.0776% | 272 | 75.1% | 12.7 |
| 65% | 0.5 | 250k | Peeking | 0.21 | 65.0737% | 258 | 72.4% | 10.4 |
| 65% | 0.5 | 500k | Peeking + Best | 0.08 | 65.0844% | 506 | 75.7% | 14.6 |
| 65% | 0.5 | 500k | Peeking | 0.20 | 65.0779% | 467 | 72.4% | 10.7 |
| 65% | 0.5 | 2.0MM | Peeking + Best | 0.04 | 65.0912% | 1,916 | 76.0% | 16.4 |
| 65% | 0.5 | 2.0MM | Peeking | 0.20 | 65.0819% | 1,721 | 72.4% | 10.7 |
| 65% | 1.0 | 100k | Peeking + Best | 0.17 | 65.1811% | 362 | 84.8% | 10.2 |
| 65% | 1.0 | 100k | Peeking | 0.24 | 65.1795% | 359 | 83.1% | 8.9 |
| 65% | 1.0 | 250k | Peeking + Best | 0.12 | 65.2021% | 708 | 85.5% | 11.3 |
| 65% | 1.0 | 250k | Peeking | 0.21 | 65.1982% | 694 | 83.2% | 9.4 |
| 65% | 1.0 | 500k | Peeking + Best | 0.10 | 65.2148% | 1,289 | 85.7% | 11.9 |
| 65% | 1.0 | 500k | Peeking | 0.20 | 65.2089% | 1,254 | 83.3% | 9.6 |
| 65% | 1.0 | 2.0MM | Peeking + Best | 0.04 | 65.2284% | 4,796 | 86.1% | 14.1 |
| 65% | 1.0 | 2.0MM | Peeking | 0.20 | 65.2192% | 4,604 | 83.3% | 9.6 |
| 65% | 2.0 | 100k | Peeking + Best | 0.20 | 65.4076% | 815 | 91.8% | 8.5 |
| 65% | 2.0 | 100k | Peeking | 0.23 | 65.4065% | 813 | 91.1% | 8.2 |
| 65% | 2.0 | 250k | Peeking + Best | 0.15 | 65.4477% | 1,567 | 92.2% | 9.1 |
| 65% | 2.0 | 250k | Peeking | 0.21 | 65.4452% | 1,558 | 91.1% | 8.4 |
| 65% | 2.0 | 500k | Peeking + Best | 0.11 | 65.4707% | 2,824 | 92.5% | 9.7 |
| 65% | 2.0 | 500k | Peeking | 0.19 | 65.4669% | 2,801 | 91.1% | 8.6 |
| 65% | 2.0 | 2.0MM | Peeking + Best | 0.05 | 65.4941% | 10,376 | 92.8% | 11.0 |
| 65% | 2.0 | 2.0MM | Peeking | 0.19 | 65.4885% | 10,258 | 91.1% | 8.6 |

## 2. Effect of Baseline Conversion Rate

*Averaged across all PTN and σ values. Peeking+Best strategy.*

| CR | Opt α | Proj Mean | Marginal | Best Rate | Avg Days |
|---|---|---|---|---|---|
| 5% | 0.10 | 5.0090% | 80 | 61.9% | 15.1 |
| 10% | 0.10 | 10.0230% | 203 | 66.0% | 14.9 |
| 30% | 0.11 | 30.0951% | 828 | 74.6% | 13.7 |
| 65% | 0.11 | 65.2473% | 2,131 | 84.4% | 11.7 |

### Key observations

- **Optimal α is roughly stable to baseline CR.** Range: α=0.10 (CR=10%) to α=0.11 (CR=65%).
- **Experiment length:** Higher CR → faster stopping. CR=65% averages 11.7 days vs 15.1 days at CR=5%.
- **Best condition selection rate:** CR=65% has the highest rate (84.4%) vs CR=5% (61.9%).
- **Marginal events** scale roughly with CR (larger CR → larger absolute effect pool).

### Strategy comparison at each CR (avg over PTN, σ=1.0)

| CR | Strategy | Opt α | Proj Mean | Marginal | Best Rate | Avg Days |
|---|---|---|---|---|---|---|
| 5% | Peeking + Best | 0.10 | 5.0058% | 52 | 60.6% | 14.9 |
| 5% | Peeking | 0.24 | 5.0051% | 44 | 59.1% | 10.2 |
| 5% | Fixed Sample | 0.50 | 5.0053% | 50 | 61.0% | 20.0 |
| 10% | Peeking + Best | 0.10 | 10.0157% | 139 | 65.1% | 14.8 |
| 10% | Peeking | 0.22 | 10.0139% | 120 | 62.7% | 10.7 |
| 10% | Fixed Sample | 0.49 | 10.0141% | 134 | 65.6% | 20.0 |
| 30% | Peeking + Best | 0.10 | 30.0727% | 639 | 74.6% | 14.1 |
| 30% | Peeking | 0.21 | 30.0682% | 587 | 71.9% | 10.3 |
| 30% | Fixed Sample | 0.49 | 30.0642% | 609 | 75.3% | 20.0 |
| 65% | Peeking + Best | 0.11 | 65.2066% | 1,789 | 85.5% | 11.9 |
| 65% | Peeking | 0.21 | 65.2015% | 1,728 | 83.2% | 9.4 |
| 65% | Fixed Sample | 0.50 | 65.1760% | 1,673 | 86.2% | 20.0 |

## 3. Effect of Post-Test N

*Averaged across all CR and σ values. All strategies.*

| PTN | Strategy | Opt α | Proj Mean | Marginal | Best Rate | Avg Days |
|---|---|---|---|---|---|---|
| 100k | Peeking + Best | 0.17 | 27.5820% | 164 | 71.0% | 11.5 |
| 100k | Peeking | 0.23 | 27.5811% | 162 | 69.6% | 9.8 |
| 100k | Fixed Sample | 0.50 | 27.5531% | 106 | 72.3% | 20.0 |
| 250k | Peeking + Best | 0.12 | 27.5916% | 320 | 71.6% | 13.2 |
| 250k | Peeking | 0.22 | 27.5894% | 313 | 69.6% | 10.2 |
| 250k | Fixed Sample | 0.50 | 27.5761% | 266 | 72.3% | 20.0 |
| 500k | Peeking + Best | 0.09 | 27.5973% | 584 | 71.9% | 14.3 |
| 500k | Peeking | 0.22 | 27.5940% | 564 | 69.6% | 10.2 |
| 500k | Fixed Sample | 0.49 | 27.5887% | 532 | 72.3% | 20.0 |
| 2.0MM | Peeking + Best | 0.04 | 27.6035% | 2,173 | 72.2% | 16.3 |
| 2.0MM | Peeking | 0.21 | 27.5986% | 2,071 | 69.6% | 10.4 |
| 2.0MM | Fixed Sample | 0.50 | 27.6013% | 2,128 | 72.3% | 20.0 |

### Key observations

- **Optimal α shifts more conservative as PTN increases.** Δα = -0.14 from PTN=100k to PTN=2.0MM.
- **Marginal events grow with PTN** — more post-test exposure amplifies the value of picking the right winner. Peeking+Best at PTN=2.0MM: 2,173 vs 164 at PTN=100k.
- **Avg experiment length is unaffected by PTN** — stopping decisions depend only on the test data, not rollout size.
- **Best condition selection rate is unaffected by PTN** for the same reason.

### How PTN shifts optimal α by strategy (σ=1.0, CR=10%)

| PTN | Peeking+Best α | Peeking α | Fixed α | P+B Marginal | Fixed Marginal |
|---|---|---|---|---|---|
| 100k | 0.15 | 0.24 | 0.50 | 26 | 18 |
| 250k | 0.10 | 0.22 | 0.49 | 53 | 48 |
| 500k | 0.09 | 0.22 | 0.48 | 100 | 95 |
| 2.0MM | 0.07 | 0.20 | 0.50 | 379 | 376 |

## 4. Effect of Expected Effects (σ)

*σ = standard deviation of the ITC distribution (effect size variability across experiments)*

*Averaged across all CR and PTN values.*

| σ | Strategy | Opt α | Proj Mean | Marginal | Best Rate | Avg Days |
|---|---|---|---|---|---|---|
| 0.5 | Peeking + Best | 0.09 | 27.5272% | 240 | 63.3% | 15.1 |
| 0.5 | Peeking | 0.22 | 27.5251% | 216 | 61.5% | 10.6 |
| 0.5 | Fixed Sample | 0.50 | 27.5241% | 229 | 63.8% | 20.0 |
| 1.0 | Peeking + Best | 0.10 | 27.5752% | 655 | 71.5% | 13.9 |
| 1.0 | Peeking | 0.22 | 27.5722% | 620 | 69.2% | 10.2 |
| 1.0 | Fixed Sample | 0.50 | 27.5649% | 616 | 72.0% | 20.0 |
| 2.0 | Peeking + Best | 0.11 | 27.6785% | 1,537 | 80.4% | 12.5 |
| 2.0 | Peeking | 0.22 | 27.6751% | 1,497 | 78.1% | 9.6 |
| 2.0 | Fixed Sample | 0.50 | 27.6504% | 1,429 | 81.1% | 20.0 |

### Key observations

- **Larger σ → shorter experiments.** σ=2.0: avg 12.5 days vs 15.1 days at σ=0.5.
- **Larger σ → higher best-condition selection rate.** σ=2.0: 80.4% vs 63.3% at σ=0.5. Larger effects are easier to detect reliably.
- **Larger σ → substantially more marginal value.** σ=2.0: 1,537 vs 240 at σ=0.5.
- **Optimal α shifts more aggressive at smaller σ.** At σ=0.5, optimal α=0.09; at σ=2.0, α=0.11.

### Strategy value gap grows with σ (avg over CR, PTN)

| σ | P+B Marginal | Peeking Marginal | Fixed Marginal | P+B vs Fixed Δ |
|---|---|---|---|---|
| 0.5 | 240 | 216 | 229 | +11 |
| 1.0 | 655 | 620 | 616 | +38 |
| 2.0 | 1,537 | 1,497 | 1,429 | +108 |

## 5. Strategy Dominance — Peeking+Best vs Fixed Sample

*Across all 48 scenarios, how much does the optimal stopping rule outperform Fixed Sample at α=0.05?*

| Scenario | P+B Opt α | P+B Marginal | Fixed@0.05 Marginal | Gain | P+B Avg Days | Fixed Avg Days |
|---|---|---|---|---|---|---|
| CR=5%, σ=0.5, PTN=100k | 0.12 | 2 | 0 | +2 | 14.4 | 20.0 |
| CR=5%, σ=0.5, PTN=250k | 0.14 | 5 | 1 | +4 | 13.6 | 20.0 |
| CR=5%, σ=0.5, PTN=500k | 0.12 | 9 | 2 | +7 | 14.4 | 20.0 |
| CR=5%, σ=0.5, PTN=2.0MM | 0.02 | 35 | 9 | +26 | 18.8 | 20.0 |
| CR=5%, σ=1.0, PTN=100k | 0.17 | 10 | 3 | +7 | 12.4 | 20.0 |
| CR=5%, σ=1.0, PTN=250k | 0.14 | 20 | 6 | +14 | 13.5 | 20.0 |
| CR=5%, σ=1.0, PTN=500k | 0.07 | 36 | 11 | +25 | 16.2 | 20.0 |
| CR=5%, σ=1.0, PTN=2.0MM | 0.04 | 141 | 43 | +98 | 17.6 | 20.0 |
| CR=5%, σ=2.0, PTN=100k | 0.15 | 33 | 11 | +23 | 12.7 | 20.0 |
| CR=5%, σ=2.0, PTN=250k | 0.11 | 67 | 25 | +42 | 14.1 | 20.0 |
| CR=5%, σ=2.0, PTN=500k | 0.05 | 125 | 50 | +76 | 16.6 | 20.0 |
| CR=5%, σ=2.0, PTN=2.0MM | 0.05 | 479 | 194 | +285 | 16.6 | 20.0 |
| CR=10%, σ=0.5, PTN=100k | 0.18 | 7 | 1 | +5 | 12.2 | 20.0 |
| CR=10%, σ=0.5, PTN=250k | 0.07 | 14 | 3 | +11 | 16.4 | 20.0 |
| CR=10%, σ=0.5, PTN=500k | 0.06 | 26 | 7 | +20 | 16.8 | 20.0 |
| CR=10%, σ=0.5, PTN=2.0MM | 0.02 | 102 | 29 | +74 | 18.7 | 20.0 |
| CR=10%, σ=1.0, PTN=100k | 0.15 | 26 | 6 | +20 | 13.0 | 20.0 |
| CR=10%, σ=1.0, PTN=250k | 0.10 | 53 | 17 | +36 | 14.8 | 20.0 |
| CR=10%, σ=1.0, PTN=500k | 0.09 | 100 | 33 | +66 | 15.2 | 20.0 |
| CR=10%, σ=1.0, PTN=2.0MM | 0.07 | 379 | 129 | +250 | 16.1 | 20.0 |
| CR=10%, σ=2.0, PTN=100k | 0.17 | 83 | 30 | +53 | 11.6 | 20.0 |
| CR=10%, σ=2.0, PTN=250k | 0.12 | 167 | 76 | +91 | 13.2 | 20.0 |
| CR=10%, σ=2.0, PTN=500k | 0.09 | 309 | 152 | +157 | 14.2 | 20.0 |
| CR=10%, σ=2.0, PTN=2.0MM | 0.03 | 1,172 | 606 | +566 | 17.0 | 20.0 |
| CR=30%, σ=0.5, PTN=100k | 0.20 | 38 | 10 | +28 | 11.3 | 20.0 |
| CR=30%, σ=0.5, PTN=250k | 0.09 | 77 | 25 | +52 | 15.2 | 20.0 |
| CR=30%, σ=0.5, PTN=500k | 0.07 | 144 | 49 | +95 | 16.0 | 20.0 |
| CR=30%, σ=0.5, PTN=2.0MM | 0.01 | 549 | 192 | +357 | 19.1 | 20.0 |
| CR=30%, σ=1.0, PTN=100k | 0.17 | 124 | 45 | +79 | 11.6 | 20.0 |
| CR=30%, σ=1.0, PTN=250k | 0.12 | 247 | 112 | +136 | 13.2 | 20.0 |
| CR=30%, σ=1.0, PTN=500k | 0.08 | 457 | 223 | +234 | 14.7 | 20.0 |
| CR=30%, σ=1.0, PTN=2.0MM | 0.03 | 1,726 | 891 | +836 | 17.0 | 20.0 |
| CR=30%, σ=2.0, PTN=100k | 0.22 | 333 | 168 | +165 | 9.3 | 20.0 |
| CR=30%, σ=2.0, PTN=250k | 0.14 | 650 | 419 | +231 | 10.9 | 20.0 |
| CR=30%, σ=2.0, PTN=500k | 0.11 | 1,184 | 837 | +347 | 11.7 | 20.0 |
| CR=30%, σ=2.0, PTN=2.0MM | 0.05 | 4,406 | 3,344 | +1,062 | 13.8 | 20.0 |
| CR=65%, σ=0.5, PTN=100k | 0.17 | 136 | 50 | +86 | 11.5 | 20.0 |
| CR=65%, σ=0.5, PTN=250k | 0.13 | 272 | 128 | +143 | 12.7 | 20.0 |
| CR=65%, σ=0.5, PTN=500k | 0.08 | 506 | 256 | +251 | 14.6 | 20.0 |
| CR=65%, σ=0.5, PTN=2.0MM | 0.04 | 1,916 | 1,020 | +896 | 16.4 | 20.0 |
| CR=65%, σ=1.0, PTN=100k | 0.17 | 362 | 184 | +178 | 10.2 | 20.0 |
| CR=65%, σ=1.0, PTN=250k | 0.12 | 708 | 463 | +245 | 11.3 | 20.0 |
| CR=65%, σ=1.0, PTN=500k | 0.10 | 1,289 | 927 | +362 | 11.9 | 20.0 |
| CR=65%, σ=1.0, PTN=2.0MM | 0.04 | 4,796 | 3,705 | +1,091 | 14.1 | 20.0 |
| CR=65%, σ=2.0, PTN=100k | 0.20 | 815 | 470 | +345 | 8.5 | 20.0 |
| CR=65%, σ=2.0, PTN=250k | 0.15 | 1,567 | 1,177 | +390 | 9.1 | 20.0 |
| CR=65%, σ=2.0, PTN=500k | 0.11 | 2,824 | 2,356 | +469 | 9.7 | 20.0 |
| CR=65%, σ=2.0, PTN=2.0MM | 0.05 | 10,376 | 9,424 | +952 | 11.0 | 20.0 |

## 6. Grand Summary

### The aggressive stopping rule wins across all 48 scenarios

- **Peeking+Best always outperforms Fixed Sample at α=0.05** in terms of marginal events.
  - Minimum gain: **+2** incremental conversions
  - Maximum gain: **+1,091** incremental conversions
  - Average gain: **+229** incremental conversions
- **Experiments end earlier.** Peeking+Best averages **13.8 days** vs **20.0 days** for Fixed at α=0.05.
- **Optimal α for Peeking+Best** averages **0.10** — far more aggressive than the conventional 0.05.
- **Fixed Sample optimal α averages 0.50** — also far more aggressive than 0.05, confirming that even within fixed sample testing, α=0.05 is overly conservative.

### What moves the optimal threshold

- **Post-Test N** has the clearest directional effect on optimal α: larger rollout → slightly more conservative optimum (more at stake).
- **Baseline CR** has minimal effect on optimal α but large effect on experiment length (higher CR → faster decisions).
- **σ (effect variability)** drives value more than any other dimension. Organizations with high effect variability (startups, new features) see the largest absolute gains from switching stopping rules.

### Robustness

The qualitative finding — aggressive early stopping produces more long-term value than conventional significance testing — holds across all 48 scenarios. The magnitude varies but the direction never reverses.