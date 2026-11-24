# Is South Africa’s Economy Really Recovering? A Data-Driven Investigation

*Beyond GDP: What employment, inflation, population growth and purchasing power reveal about South Africa’s economic recovery.*

South Africa's economy is larger than it was before the COVID-19 pandemic. But does that necessarily mean South Africans are better off?

Economic recovery is often discussed through gross domestic product (GDP). While GDP is an important measure of economic performance, it does not tell the entire story.

An economy can grow while unemployment remains high, population growth outpaces economic expansion, and salaries struggle to keep up with rising consumer prices.

This raises an important question:

**Has South Africa recovered economically, or has it simply recovered statistically in terms of aggregate output?**

To investigate this question, I analysed official Statistics South Africa data spanning 2010 to 2026, focusing on five dimensions of economic recovery:

- Real GDP
- Real GDP per capita
- Employment and unemployment
- Consumer price inflation
- Real earnings and purchasing power

Using Python, statistical analysis and data visualisation, I examined whether South Africa's economic recovery extends beyond aggregate economic output.

## 1. South Africa's Economy Has Recovered — But How Strongly?

The COVID-19 pandemic caused a severe disruption to South Africa's economy. However, the years that followed saw aggregate economic output gradually recover.

**[Insert Figure 01 — South Africa's Real GDP, 2010–2026]**

By the second quarter of 2026, South Africa's real GDP was approximately **2.24% higher than in the fourth quarter of 2019**.

From an aggregate output perspective, the economy has recovered beyond its pre-pandemic level.

However, recovering lost output is not necessarily the same as achieving strong economic growth.

### Has Economic Growth Improved?

I compared average quarterly GDP growth across two periods:

| Period | Average quarterly growth |
|---|---:|
| Pre-pandemic: 2010–2019 | 0.421% |
| Post-pandemic: 2022–2026 Q2 | 0.252% |

**[Insert Figure 02 — GDP Growth Comparison]**

Although average growth was lower in the post-pandemic period, statistical testing using heteroskedasticity and autocorrelation consistent (HAC) inference produced a p-value of 0.210.

The difference was therefore not statistically significant at the conventional 5% significance level.

This does not prove that growth remained unchanged. Rather, the available evidence is insufficient to establish a statistically significant difference between the selected periods.

**[Insert Figure 03 — GDP Recovery Index]**

South Africa has recovered its pre-pandemic aggregate output, but that alone provides limited insight into the strength and sustainability of its recovery.

### What If Historical Growth Trends Had Continued?

To provide additional context, I extrapolated three historical GDP growth trends.

**[Insert Figure 04 — Actual GDP vs Historical Growth Trajectories]**

Depending on the historical period selected, actual GDP was below the extrapolated trajectory by:

- **9.09%** using the 2010–2019 trend.
- **5.21%** using the 2013–2019 trend.
- **4.34%** using the 2015–2019 trend.

These estimates are not causal measurements of economic damage caused by the pandemic. They illustrate how actual economic output compares with alternative historical growth benchmarks.

The magnitude of the gap depends on the benchmark selected, but all three comparisons place actual GDP below their extrapolated trajectories.

## 2. A Growing Economy Does Not Necessarily Mean Greater Prosperity Per Person

One of the limitations of aggregate GDP is that it does not account for population growth.

If an economy grows more slowly than its population, average economic output per person can decline even while total GDP increases.

To investigate this, I calculated South Africa's real GDP per capita using annual real GDP and population estimates.

**[Insert Figure 05 — Real GDP vs Real GDP per Capita]**

Between 2019 and 2025:

| Indicator | Change |
|---|---:|
| Real GDP | +1.59% |
| Estimated population | +7.34% |
| Real GDP per capita | −5.36% |

Real GDP per capita declined from approximately **R120,049 in 2019 to R113,619 in 2025**, measured in constant 2022 prices.

In other words, South Africa produced more economic output overall, but less economic output per person.

GDP per capita is not a direct measure of household income, nor does it capture income inequality. Nevertheless, it provides an important perspective that aggregate GDP alone cannot offer.

The economy has grown, but its growth has not kept pace with population expansion.

## 3. Has the Labour Market Really Recovered?

Employment is one of the most direct ways through which economic growth can improve people's lives.

A growing economy should ideally create opportunities for an expanding working-age population.

Using the Quarterly Labour Force Survey, I compared South Africa's labour market in the third quarter of 2019 with the third quarter of 2026.

**[Insert Figure 06 — South Africa's Labour Market Recovery]**

| Indicator | 2019 Q3 | 2026 Q3 |
|---|---:|---:|
| Employed people | 16.38 million | 16.84 million |
| Unemployed people | 6.73 million | 8.58 million |
| Working-age population | 38.58 million | 42.43 million |
| Official unemployment rate | 29.1% | 33.7% |
| Employment-to-population ratio | 42.4% | 39.7% |

At first glance, the increase in employment appears encouraging.

However, employment increased by only 2.84%, while the working-age population increased by approximately 9.96%.

The economy has added employment, but not at a pace sufficient to maintain its pre-pandemic employment-to-population ratio.

### The 1.17 Million Employment Gap

I calculated how many people would have been employed in 2026 Q3 if South Africa had maintained its 2019 Q3 employment-to-population ratio.

The benchmark suggests:

- Expected employment: approximately 18.01 million.
- Actual employment: approximately 16.84 million.
- Employment shortfall relative to the benchmark: approximately 1.17 million.

This does not mean that 1.17 million jobs were lost because of COVID-19, nor does it represent available vacancies.

It illustrates the scale of the difference between actual employment and the employment level implied by maintaining the pre-pandemic employment ratio.

South Africa has more employed people than in 2019, but a smaller proportion of its working-age population is employed.

## 4. The Rising Cost of Living

Economic recovery is not only about production and employment. It is also about what people can afford.

Using South Africa's historical Consumer Price Index, I examined how the general consumer price level changed between October 2019 and October 2026.

**[Insert Figure 07 — Cumulative Consumer Price Increase]**

Over this period, consumer prices increased by approximately **38.55%**.

To put this into perspective, a representative basket of goods and services costing R1,000 in October 2019 would cost approximately R1,385.50 in October 2026, assuming its prices increased in line with headline CPI.

This is an illustration of the cumulative change in the general price level. Individual households may experience different price increases depending on their spending patterns.

An important distinction must also be made between inflation and the price level.

When inflation decreases, prices generally continue increasing, but at a slower rate, provided inflation remains positive.

Lower inflation does not necessarily mean that goods and services have become cheaper.

This helps explain why improvements in inflation figures may not immediately translate into a noticeable reduction in household financial pressure.

## 5. Have Salaries Kept Pace With Inflation?

Rising consumer prices raise another important question: have earnings increased sufficiently to compensate for inflation?

Using Statistics South Africa's Quarterly Employment Statistics, I compared average monthly earnings in the formal non-agricultural sector between November 2019 and May 2026.

**[Insert Figure 08 — Nominal vs Real Earnings]**

Average monthly earnings increased from R22,500 to R30,611.

At face value, this represents a substantial improvement.

However, after accounting for inflation:

| Indicator | Cumulative change |
|---|---:|
| Nominal average earnings | +36.05% |
| Consumer prices | +35.58% |
| Real average earnings | +0.35% |

Expressed in November 2019 purchasing power, the average May 2026 monthly earnings of R30,611 were equivalent to approximately R22,578.

That is an improvement of just R78 per month in inflation-adjusted terms compared with November 2019.

Over approximately six and a half years, average real earnings barely increased.

These figures represent average earnings in the formal non-agricultural sector. They do not measure median earnings, informal-sector earnings or the wage growth experienced by individual employees.

Nevertheless, the comparison highlights an important economic reality:

**A substantial increase in nominal earnings does not necessarily translate into a substantial improvement in purchasing power.**

## 6. South Africa's Economic Recovery Scorecard

Bringing together all five dimensions produces a more comprehensive picture of South Africa's economic recovery.

**[Insert Figure 09 — South Africa's Economic Recovery Scorecard]**

| Economic indicator | Change |
|---|---:|
| Real GDP | +2.24% |
| Real GDP per capita | −5.36% |
| Employment-to-population ratio | −2.70 percentage points |
| Consumer price level | +38.55% |
| Real average monthly earnings | +0.35% |

The indicators use different reference periods and measure different aspects of the economy. They should not be combined into a single numerical recovery score.

However, together they reveal a consistent distinction between aggregate economic recovery and broader economic well-being.

South Africa has recovered its pre-pandemic aggregate output, but:

- Real output per person remains lower.
- Employment has not kept pace with working-age population growth.
- Consumer prices have increased substantially.
- Average formal-sector purchasing power has barely improved.

## 7. What This Analysis Cannot Tell Us

No single economic investigation can capture every dimension of national prosperity.

This analysis does not directly measure poverty, household disposable income, wealth inequality, household debt or access to public services.

Population estimates used in the GDP per capita analysis also involve approximations based on published annual growth rates.

Furthermore, the comparisons are primarily descriptive. They do not isolate the causal effects of COVID-19, government policies, electricity constraints or other economic developments.

These limitations matter because economic outcomes are influenced by multiple interconnected factors.

The objective is not to assign blame, but to assess recovery through several measurable economic indicators.

## Conclusion: Is South Africa Really Recovering?

The answer depends on how we define recovery.

If recovery means returning to pre-pandemic aggregate economic output, then South Africa has recovered.

If recovery means producing more economic output per person, expanding employment opportunities in line with population growth, and meaningfully improving purchasing power, the evidence is less encouraging.

The findings support a conclusion of **uneven economic recovery**.

Economic growth remains important, but its broader significance depends on whether it translates into improved economic opportunities and living conditions.

Perhaps the question we should be asking is no longer simply:

*Has South Africa's economy recovered?*

But rather:

**How can South Africa translate economic recovery into meaningful improvements in people's lives?**

## About the Project

This independent data analytics project was developed using official Statistics South Africa datasets, Python, statistical inference and data visualisation.

**Technical tools:** Python, pandas, NumPy, Matplotlib, statsmodels, Jupyter Notebook and GitHub.

**Data sources:**

- Statistics South Africa — Quarterly GDP (P0441).
- Statistics South Africa — Mid-year Population Estimates (P0302).
- Statistics South Africa — Quarterly Labour Force Survey (P0211).
- Statistics South Africa — Consumer Price Index (P0141).
- Statistics South Africa — Quarterly Employment Statistics (P0277).

The complete analysis, methodology, processed datasets and visualisations are available in the accompanying GitHub repository.

**GitHub repository:** [Insert repository link after publication]