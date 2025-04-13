******Final Project******

**Students:** *Manuel Cervera Escalante, Sadhana Smruthi Srinivasan, and Carlos E. Rosillo Fuentes*

In our first class, we delved into the two primary investing paradigms: Fundamental and Quantitative Investing. Fundamental investing emphasizes analyzing a company's financial statements, management, industry position, and market conditions to make investment decisions. On the other hand, Quantitative Investing relies on mathematical and statistical models to identify investment opportunities, focusing less on the qualitative aspects of companies and more on numerical data.

While our class was literally Quantitative Investing, for our final project, we wanted to synthesize these two methodologies. Our goal was to create a bridge from Fundamental to Quantitative Investing. To achieve this, we proposed developing factors that incorporate metrics traditionally reserved for Fundamental analysis into the quantitative investment framework. This approach aims not only to leverage the numerical strength of quantitative methods but also to enrich it with the depth of understanding that fundamental analysis provides. By doing so, we seek to explore whether incorporating fundamental metrics can enhance the predictive power and robustness of quantitative investment strategies.

The concept of a quality factor represents a well-known "anomaly" in financial research, attracting considerable attention for its potential to identify superior investment opportunities. The construction of this quality factor has been tried several times in the past: Kozlov and Petajisto (2013) focused on accruals to measure earnings quality, and Bouchaud, Ciliberti, and Thesmar (2016) used Return on Assets as their marker of quality. Furthermore, Asness, Frazzini, and Pedersen (2013) proposed a broader approach with their Quality Minus Junk (QMJ) factor, incorporating profitability, growth, safety, and payout metrics.

The challenge in defining "quality" in the financial context, as highlighted by Hsu, Kalesnik, and Kose (2017), is its lack of a universally accepted definition, suggesting a more nuanced approach that encompasses multiple signals. Inspired by this insight, our project delves into an exploration of seven different metrics to assess their efficacy in capturing the quality factor. Through this process, we aim to identify the best performing indicators of quality and subsequently construct a composite portfolio.

The metrics we will check are:

**Return on Capital Employed**

**Return on Assets**

**Gross Profit Margin**

**Current Ratio**

**EBITDA to Total Debt Ratio**

**TTM Revenue Growth**

**Cash Flow Margin**


******Data handling and pre-processing******

For our stock data, we will use the CRSP file we used in class and for our factor construction we will complement the data with Compustat. We accessed the Compustat metrics data from the “Financial Ratios Suite by WRDS” and we used the Compustat-CRSP merged database to get the quarterly revenue for each firm.

The Financial Ratios Suite includes a variable called ‘public_date’ which is when that data became available to the market so we can merge the two datasets without worrying about lagging the information.

Our analysis revealed that the Revenue Growth Factor exhibited a negative sign, a result that warrants careful consideration in the construction of our composite portfolio. In light of this, a straightforward strategy might involve adjusting the long and short positions—longing factors with positive contributions and shorting those with negative impacts—to align with their respective signs for optimal portfolio performance.

However, rather than altering the foundational strategy of our portfolio by changing the portions we long and short based on this single factor, we will "strategically" short the Revenue Growth Factor within our overall composite portfolio.


In our analysis of the selected quality metrics, we observed a notable pattern: except for Return on Assets (ROA) and Return on Capital Employed (ROCE), there appears to be a low correlation among all the factors under consideration. This finding has significant implications for our investment strategy, particularly in terms of portfolio diversification and risk management. In the realm of quantitative investing, a low correlation between factors is generally desirable. It suggests that each factor captures different aspects of company quality and performance, thereby providing a broader, more robust foundation for investment decisions.

After a comprehensive analysis of the performance of each factor under consideration, we have made a strategic decision to refine our focus to a select group of factors for our composite portfolio. Specifically, we will only include Return on Assets (ROA), Return on Capital Employed (ROCE), Gross Profit (GP), and Revenue Growth.

We have decided to name this bespoke combination of factors the ***"Quality Investment Premium" - (QIP)***.

The QIP label reflects our commitment to identifying and leveraging the inherent value of high-quality companies through a disciplined, quantitative approach and not just using the acronym of the class.

******Conclusion******

While the Sharpe Ratio of our Quality Investment Premium (QIP) factor does not reach exceptionally high levels, it is noteworthy that incorporating fundamental metrics can yield respectable returns. This outcome underscores the viability of fundamental analysis within a quantitative framework, demonstrating that it's possible to achieve a balanced trade-off between risk and return. Our findings align with industry trends, where leading investment firms like BlackRock and Invesco have successfully marketed Quality ETFs, indicating a growing appreciation for strategies that focus on company fundamentals to drive investment performance.

Looking forward, we are intrigued by the prospect of enhancing the QIP factor through strategic modifications. Specifically, we propose rebalancing the portfolio quarterly and integrating quarterly metrics into our analysis. We believe this approach could imbue the QIP factor with a more pronounced long-term perspective, potentially smoothing out short-term volatilities and aligning more closely with the fundamental growth trajectories of the underlying investments.

***References***

Asness C., Frazzini A., and Pedersen L., 2013. Quality Minus Junk

Bouchaud J., Ciliberti S., Landier A, Simon G., and Thesmar D., 2016. The Excess Returns of Quality Stocks: A Behavioral Anomaly

Hsu J., Kalesnik V., and Kose E., 2017. What is Quality?

Kozlov M. and Petajisto A., 2013. Global Return Premiums on Earnings Quality, Value, and Size.
