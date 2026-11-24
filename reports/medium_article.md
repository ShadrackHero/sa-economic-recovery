
# Is South Africa’s Economy Really Recovering? A Data-Driven Investigation

*Beyond GDP: What employment, inflation, population growth and purchasing power reveal about South Africa’s economic recovery.*

**Publication:** Medium

**Status:** Published

**Publication date:** 25 November 2026

**Published article:** [Read on Medium](https://medium.com/@shadrackherot/is-south-africas-economy-really-recovering-a-data-driven-investigation-3565d666994e)


South Africa's economy is larger than it was before the COVID-19 pandemic. Yet economic output per person remains lower, unemployment is higher, consumer prices have increased substantially, and average formal-sector purchasing power has barely improved.

How do we reconcile these seemingly conflicting economic outcomes?

By the second quarter of 2026, South Africa's real GDP was 2.24% above its pre-pandemic level. However, real GDP per capita in 2025 remained 5.36% below its 2019 level.

These two findings illustrate why measuring economic recovery through aggregate GDP alone can be misleading.

An economy can expand while struggling to create sufficient employment, keep pace with population growth and improve purchasing power.

I wanted to understand whether South Africa's economic recovery extends beyond aggregate production.

Using official Statistics South Africa data, Python and statistical modelling, I examined five dimensions of recovery:

- Real economic output
- Economic output per person
- Employment and unemployment
- Consumer prices
- Real earnings and purchasing power

The results reveal a recovery that is far more uneven than aggregate GDP figures suggest.

## Data and Methodology

The investigation uses official Statistics South Africa economic datasets covering periods between 2010 and 2026.

The analysis combines descriptive statistics, inflation adjustments, population-adjusted economic indicators, regression analysis, statistical inference and historical growth trend extrapolation.

Pre-pandemic observations from 2019 serve as the primary recovery benchmarks. The latest available observations differ across datasets because economic indicators are published at different frequencies and with different reporting schedules.

All data transformations, calculations, statistical models and visualisations are documented in a reproducible Python notebook available through the accompanying GitHub repository.

## 1. South Africa's Economy Has Recovered — But How Strongly?

The COVID-19 pandemic caused a severe contraction in South Africa's economic output. The years that followed saw a gradual recovery.

**[Insert Figure 01]**

*Figure 1: South Africa's quarterly real GDP, 2010–2026. Source: Statistics South Africa, P0441. Author's calculations and visualisation.*

By the second quarter of 2026, real GDP was approximately **2.24% higher than in the fourth quarter of 2019**.

From an aggregate output perspective, South Africa has surpassed its pre-pandemic economic level.

However, recovering lost output is not the same as establishing a stronger growth trajectory.

### Has economic growth improved?

I compared average quarterly real GDP growth across two periods, excluding the pandemic disruption and initial rebound years of 2020 and 2021.

| Period | Average quarterly growth |
|---|---:|
| 2010–2019 | 0.421% |
| 2022–2026 Q2 | 0.252% |

**[Insert Figure 02]**

*Figure 2: Average quarterly real GDP growth before and after the pandemic disruption.*

The estimated difference was −0.169 percentage points.

To assess whether this difference was statistically significant, I fitted a regression model using heteroskedasticity and autocorrelation consistent (HAC) standard errors.

The results were:

- p-value: 0.210
- 95% confidence interval: [−0.433, 0.095] percentage points

Although average quarterly growth was lower in the later period, the difference was not statistically significant at the conventional 5% significance level.

This does not establish that economic growth remained unchanged. It means the available evidence is insufficient to conclude that average growth differed statistically between the selected periods under the specified model.

**[Insert Figure 03]**

*Figure 3: South Africa's real GDP recovery index, with 2019 Q4 as the reference period.*

South Africa has recovered its pre-pandemic aggregate output. Whether it has established a stronger economic growth path is a different question.

### What if historical growth trends had continued?

To provide additional context, I fitted three log-linear GDP trend models using different pre-pandemic estimation periods.

Each historical trend was extrapolated to the second quarter of 2026 and compared with actual economic output.

**[Insert Figure 04]**

*Figure 4: Actual real GDP compared with extrapolated pre-pandemic growth trajectories.*

| Historical estimation period | Actual GDP relative to extrapolated trend |
|---|---:|
| 2010–2019 | −9.09% |
| 2013–2019 | −5.21% |
| 2015–2019 | −4.34% |

All three historical benchmarks place actual GDP below their extrapolated trajectories.

The magnitude of the gap depends considerably on the estimation period selected.

These models are descriptive benchmarks, not reliable forecasts or causal estimates of economic damage. Residual autocorrelation, particularly in the longest estimation window, also limits conventional statistical inference from the trend models.

Nevertheless, they provide useful context: recovering pre-pandemic output does not necessarily mean returning to the economic trajectory that preceded the pandemic.

## 2. A Larger Economy, but Less Output Per Person

Aggregate GDP does not account for changes in population size.

When population growth exceeds economic growth, average economic output per person can decline even as total production increases.

I calculated South Africa's real GDP per capita using annual real GDP and estimated population figures.

**[Insert Figure 05]**

*Figure 5: South Africa's real GDP and real GDP per capita, indexed to 2019.*

Between 2019 and 2025:

| Indicator | Change |
|---|---:|
| Real GDP | +1.59% |
| Estimated population | +7.34% |
| Real GDP per capita | −5.36% |

Measured in constant 2022 prices, estimated real GDP per capita declined from approximately R120,049 in 2019 to R113,619 in 2025.

South Africa produced more economic output overall, but less output per person.

GDP per capita is not equivalent to household income. It also does not account for how economic resources are distributed across society.

However, it provides an important perspective that aggregate GDP alone cannot offer.

**South Africa's economic expansion has not kept pace with population growth.**

## 3. More Employment, but a Weaker Employment Ratio

Employment is one of the most important channels through which economic growth can improve people's lives.

Using the Quarterly Labour Force Survey, I compared South Africa's labour market in the third quarter of 2019 with the corresponding quarter of 2026.

**[Insert Figure 06]**

*Figure 6: South Africa's labour market recovery. Source: Statistics South Africa, Quarterly Labour Force Survey.*

| Indicator | 2019 Q3 | 2026 Q3 |
|---|---:|---:|
| Employed people | 16.38 million | 16.84 million |
| Unemployed people | 6.73 million | 8.58 million |
| Working-age population | 38.58 million | 42.43 million |
| Official unemployment rate | 29.1% | 33.7% |
| Employment-to-population ratio | 42.4% | 39.7% |

The number of employed people increased by approximately 2.84%.

Over the same period, however, the working-age population increased by 9.96%.

Consequently, the proportion of working-age South Africans who were employed declined.

### The 1.17 million employment gap

What would employment look like if South Africa had maintained its 2019 employment-to-population ratio?

Applying the 2019 Q3 employment ratio to the 2026 Q3 working-age population produces the following benchmark:

- Benchmark employment: 18.01 million
- Actual employment: 16.84 million
- Employment gap: approximately 1.17 million

This is not an estimate of jobs lost because of COVID-19, nor does it represent available vacancies.

It measures the difference between actual employment and the employment level implied by maintaining the pre-pandemic employment ratio.

South Africa has more employed people than in 2019, but a smaller proportion of its working-age population is employed.

That distinction matters when assessing the inclusiveness of economic recovery.

## 4. What Happened to the Cost of Living?

Economic recovery is also about what people can afford.

Using South Africa's historical headline Consumer Price Index, I examined changes in the general consumer price level between October 2019 and October 2026.

**[Insert Figure 07]**

*Figure 7: Cumulative consumer price increases relative to October 2019. Source: Statistics South Africa, P0141.*

Over this period, the general consumer price level increased by approximately **38.55%**.

A representative basket of goods and services costing R1,000 in October 2019 would therefore cost approximately R1,385.50 in October 2026 if its prices increased in line with headline CPI.

Actual household experiences will differ depending on individual spending patterns.

There is also an important distinction between inflation and the price level.

When inflation falls but remains positive, prices generally continue rising, only at a slower rate.

Lower inflation does not necessarily mean lower prices.

This distinction helps explain why improvements in inflation figures may not immediately translate into a noticeable reduction in household financial pressure.

## 5. Have Salaries Kept Pace With Inflation?

Higher consumer prices make nominal salary increases difficult to interpret without accounting for purchasing power.

Using Statistics South Africa's Quarterly Employment Statistics, I compared average monthly earnings in the formal non-agricultural sector between November 2019 and May 2026.

Average monthly earnings increased from R22,500 to R30,611.

That represents a nominal increase of approximately 36%.

But how much of that increase remained after adjusting for inflation?

**[Insert Figure 08]**

*Figure 8: Nominal earnings growth compared with consumer price growth and inflation-adjusted earnings growth.*

| Indicator | Cumulative change |
|---|---:|
| Nominal average monthly earnings | +36.05% |
| Consumer prices | +35.58% |
| Real average monthly earnings | +0.35% |

Expressed in November 2019 purchasing power, average monthly earnings of R30,611 in May 2026 were equivalent to approximately R22,578.

That represents an inflation-adjusted difference of just R78 per month between the two observations.

Despite substantial nominal earnings growth, average purchasing power was almost unchanged in this comparison.

The result requires careful interpretation. These are average earnings in the formal non-agricultural sector, not median earnings or individual salary histories.

The observations also come from different calendar months, meaning seasonal earnings patterns, bonuses, overtime and changes in workforce composition may influence the comparison.

Two observations cannot establish a continuous real earnings trend or demonstrate statistically significant wage stagnation.

Nevertheless, the comparison illustrates why nominal salary increases alone provide an incomplete picture of purchasing power.

## 6. South Africa's Economic Recovery Scorecard

Examining the five dimensions together provides a broader assessment of economic recovery.

**[Insert Figure 09]**

*Figure 9: South Africa's multidimensional economic recovery scorecard.*

| Economic indicator | Change from selected pre-pandemic benchmark |
|---|---:|
| Real GDP | +2.24% |
| Real GDP per capita | −5.36% |
| Employment-to-population ratio | −2.70 percentage points |
| Consumer price level | +38.55% |
| Real average monthly earnings | +0.35% |

The indicators use different reference periods, units and economic definitions. They should not be aggregated into a single numerical recovery score.

However, they reveal an important distinction between aggregate economic recovery and broader economic well-being.

South Africa has surpassed its pre-pandemic aggregate output, while real output per person remains lower, employment growth has lagged behind working-age population growth, consumer prices have risen substantially, and average formal-sector purchasing power has changed very little between the selected earnings observations.

## 7. Limitations of the Investigation

Economic well-being cannot be fully captured by five indicators.

This investigation does not directly measure poverty, household disposable income, income inequality, wealth distribution, household debt or access to public services.

The population series was reconstructed using published annual population growth rates, which introduces approximation errors into the GDP per capita estimates.

The GDP growth comparison excludes 2020 and 2021. The HAC covariance estimator treats the retained observations as consecutive despite this calendar gap, which is a limitation of the statistical specification.

The historical GDP trajectories are sensitive to the selected estimation windows and should not be interpreted as causal counterfactuals.

The earnings comparison is also limited by its sectoral coverage, different reference months and reliance on two observations.

More broadly, the analysis does not isolate the economic effects of COVID-19, government policies, electricity constraints or other domestic and international developments.

Its purpose is to measure and contextualise economic recovery, rather than attribute its outcomes to particular causes.

## Conclusion: Is South Africa Really Recovering?

The answer depends on how recovery is defined.

If recovery means surpassing pre-pandemic aggregate economic output, then South Africa has recovered.

If it means increasing economic output per person, expanding employment opportunities in line with population growth and substantially improving purchasing power, the evidence is less encouraging.

The findings point towards **an uneven economic recovery**.

Aggregate economic growth remains important, but it is not sufficient on its own to establish that economic conditions have improved broadly.

Perhaps the more important question is no longer whether South Africa's economy has recovered, but whether its recovery is translating into meaningful improvements in people's lives.

## About the Project

This independent research project combines economic data analysis, statistical inference, regression modelling and data visualisation to investigate South Africa's economic recovery.

The accompanying repository contains:

- A reproducible Python analysis notebook
- 11 processed economic datasets
- Nine analytical visualisations
- Statistical and numerical validation procedures
- Research methodology and documentation

**Technical tools:** Python, pandas, NumPy, Matplotlib, statsmodels, Jupyter Notebook and GitHub.

### Data Sources

All primary economic data were obtained from Statistics South Africa.

- Gross Domestic Product (P0441)
- Mid-year Population Estimates (P0302)
- Quarterly Labour Force Survey (P0211)
- Consumer Price Index (P0141)
- Quarterly Employment Statistics (P0277)

### Explore the Research

The complete analysis, processed datasets, methodology and visualisations are available on GitHub.

**GitHub:** https://github.com/ShadrackHero/sa-economic-recovery

Readers are encouraged to explore the methodology, reproduce the analysis and critically engage with the findings.