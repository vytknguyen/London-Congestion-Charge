# London-Congestion-Charge-Programme

This project raised by the interest in applying **Revenue and Pricing Management** theories to the London Congestion Charge programme, as to reduce emissions level and generate funds to reinvest in improving public transportation services. 

<img src="https://images.prismic.io/drive-electric/123f964a-4bf3-4964-9d90-dca6b40ffc5f_congestion-charge-ulez-map.webp?auto=compress,format&w=812&fit=clip" align="center" width="600" /></a>

## Project Description

London is considering an extension to its Congestion Charge programme, a daily charge for driving a vehicle within the charging zone between the hours of 07:00 and 18:00, Monday to Friday. The extension explores the revenue and environmental impact of introducing a two-tier congestion pricing policy for peak and non-peak traffic periods.

The City conducted a survey to learn more about the willingness to pay of drivers that may enter the charging zone during the peak and non-peak hours. In total, 345 such drivers have responded to the survey and their maximum willingness to pay for peak and non-peak periods is reported in the accompanying supplementary data file. Assume that the respondents represent a total of 192,000 drivers the City estimates that may potentially enter the charging zone.

A main factor that determines emissions per car is the average travel speed, which in turn is influenced by the number of drivers entering the charging zone. The relationship between the number of drivers and average speed is given by the following:

*(The regression relationships will change over time, hence, this needs to be updated as the point of performing an analysis.)*

**Average Speed (in km/h) = 30 – 0.0625 * (# of cars in thousands, ‘000)**

Further, the emissions per car, which is generally measured in grams of CO2 per kilometre, can be approximated by a piecewise linear function as follows:

**Emissions per car (g/km):**
  - **= 617.5 – 16.7 * (Average Speed) if Average Speed < 25 km/h**
  - **= 235.0 – 1.4 * (Average Speed) if Average Speed > 25 km/h**

### 🅿️ Scenario 1

If the programme’s objective were solely to maximise revenue and a single congestion charge were to be applied across both peak and non-peak hours, which price would maximize the total revenue? With this price in effect, what is the total level of emissions?

<img align="left" width="300" src="https://github.com/vytknguyen/London-Congestion-Charge/blob/main/SinglePriceDemand.png?raw=true"/></a>

<img align="center" width="300" src="https://github.com/vytknguyen/London-Congestion-Charge/blob/main/SinglePriceRevenue.png?raw=true"/></a>

**💡 Insights:** 

**If a single congestion charge were to be charged across both peak and non-peak hours, the optimal revenue is £1349009 achieved at the price level £8.**

### 💨 Scenario 2

If the programme’s objective were solely to maximise revenue and a peak period pricing strategy is to be implemented, with the price for the non-peak period set at £7, what price would we recommend for the peak period? Also noting the resulting revenue and emissions and compare the findings with those from scenario 1.

<img align="left" width="250" src="https://github.com/vytknguyen/London-Congestion-Charge/blob/main/NonPeakDemandvsPeakPrice.png?raw=true"/></a>

<img align="left" width="250" src="https://github.com/vytknguyen/London-Congestion-Charge/blob/main/PeakDemandvsPeakPrice.png?raw=true"/></a>

<img width="250" src="https://github.com/vytknguyen/London-Congestion-Charge/blob/main/RevenuevsPeakPrice.png?raw=true"/></a>

**💡 Insights:** 

**When Non-peak periods have a base price of £7, the optimal revenue is £1371826 at the optimal price for the Peak-hours slot is £9. Level of emssisions for this price point is 37110 (g/km)**

### 🚗 Scenario 3

Suppose now that the programme’s objective is to minimize emissions rather than maximizing revenue. However, the City would like to ensure that the programme can self-sustain its operation and that a sufficient portion of the revenue is allocated to reinvest in the public transportation infrastructure. Overall, the City requires that the revenue should not fall below £1.1 million per day. Assuming a non-peak period price of £7, what
price would we recommend for the peak period? Please compare the resulting revenue and emissions level with that of scenario 2.

**💡 Insights:**

The main goal is to optimise the revenue, at base price of £7:
- Optimal peak price: £9
- Optimal revenue: £1,371,826
- Total level of emissions: 37,110 (g/km)

When setting the constraints to minimise emissions level:
- Optimal peak price: £14
- Optimal revenue: £1,183,868
- Total level of emissions: 27,310 (g/km)

Obviously, by raising the price, the total level of emissions has improved significantly, at which price the generated funds can self-sustain its operation.

**Analysis is delivered in July 2022.**

<img align="left" alt="R" width="32px" src="https://www.r-project.org/logo/Rlogo.png"/></a>
<img align="left" alt="ggplot2" width="26px" src="https://statsandr.com/blog/2020-08-21-graphics-in-r-with-ggplot2_files/graphics-in-r-with-ggplot2.png"/></a>
<img alt="GitHub" width="26px" src="https://avatars.githubusercontent.com/u/9919?s=200&v=4"/></a>
