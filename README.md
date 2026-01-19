# Portfolio Risk Manager
## Data
- Period: Jan 2021 - Dec 2025
- Trading days: 1205
- Usable return days: 890 out of 1205 (GOTO only started later = missing values)

## Assets
BBCA, BBRI --> Banking  
TLKM --> Telecom   
ASII --> Industrial  
GOTO --> Tech  
^JKSE --> Market benchmark (IDX)
  
## Daily Return Statistics
![alt text](daily_return_text.png)
![alt text](daily_return_statistics.png)
| Stock | Mean | Volatility | Interpretation |
| ----------- | ----------- | ----------- | ----------- |
| BBCA | +0.02% | Low | Stable, Defensive |
| BBRI | ~0% | Medium | Cyclical banking risk | 
| TLKM | -0.01% | Medium | Defensive but stagnant |
| ASII | +0.01% | Medium | Economic-cycle exposed | 
| GOTO | -0.12% | Very High | Speculative, Unstable |

## Correlation Heatmap
![alt text](heatmap.png)
Correlation:
- 1.0 --> Move together
- 0.0 --> Move independently
- -1.0 --> Hedge each other

For example:
BBCA <--> BBRI = 0.51 --> Strong banking linkage correlation
BBCA <--> GOTO = 0.1 --> Very weak correlation

## Portfolio Allocation vs Risk Contribution 
### Weights vs RISK
![alt text](barchart.png)
| Stock | Weight | Risk Contribution |
| ----------- | ----------- | ----------- | 
| BBCA | 30% | 27.3% | 
| BBRI | 25% | 28.3% | 
| TLKM | 20% | 17.8% | 
| ASII | 15% | 11.4% |
| GOTO | 10% | 15.2% | 

**GOTO contributes 50% more risk than its weight if you compare it to BBCA, the result of this is a classic volatility drag**
**Volatility drag is the hidden cost of price swings in investments, where big losses have a bigger negative impact than equivalent gains**

## Portofolio Performance
### Value Evolution
Initial Investment: Rp 100M
Final Return: Rp 85.3M
Loss: -14.7%

## Drawdown Analysis
**MAXIMUM DRAWDOWN**  
Maximum Drawdown: -30.01%  
Date of Max Drawdown: 2025-04-08


**VALUE AT RISK (95% Confidence)**    
Daily VaR (95%): -1.84%   
Monthly VaR (95%): -8.45%  
Expected Loss (95% confidence): Rp -1,843,733/day


**CONDITIONAL VALUE AT RISK (CVaR)**   
Daily CVaR (95%): -2.69%  
Average Loss in Worst 5% Scenarios: Rp -2,693,304/day

## Volatility and Diversification
- Portfolio volatility: **19.4%**
- Average individual stock volatility: **34.7%**

The diversification benefit is calculated as:

Diversification Benefit = 1 − (Portfolio Volatility / Weighted Average Volatility)

= 1 − (19.4% / 34.7%)  
= 44.01%

 
A diversification benefit above 40% indicates strong risk reduction due to imperfect
correlations between assets.


## Risk-Adjusted Performance (Sharpe Ratio)
Sharpe = -0.44 (Very poor)
**This portofolio took a lot of risk for worse than cash returns**

## Value at Risk (VaR & CVaR)
| Metric | Interpretation |
| ----------- | ----------- |
| VaR (95%) | Worst daily loss 95% of the time |
| CVaR(95%) | Average loss during worst 5% days |

VaR: -1.84% ≈ Rp 1.84M/day  
CVaR: -2.69% ≈ Rp 2.69M/day

## BETA analysis
Beta = 1.145 (Portofolio moves 14.5% more than the market)

## Stress Test
| Scenario | Portofolio Loss |
| ----------- | ----------- |
| Market crash (-20%) | -21.0% |
| Banking crisis (-30%) | -21.8% |
| Currency shock (-15%) | -15.0% |
| Rate hike | -9.5% |

## Monte-Carlo Simulation (1 Year Outlook)
Simulates 10,000 possible futures
### Outcome Probabilities

| Outcome | Probability |
|-------|------------|
| Profit | **40.5%** |
| Loss | **59.5%** |

### Return Scenarios

| Scenario | Return |
|--------|--------|
| Best 5% (95th percentile) | **+31.0%** |
| Median (Expected) | **-4.5%** |
| Worst 5% (5th percentile) | **-30.9%** |
