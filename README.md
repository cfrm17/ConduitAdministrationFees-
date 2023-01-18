# Conduit Administration Fees Process

Accounting requires the ability to forecast conduit administration fees. a simple stationary lognormal model for the fees is presented. Initially, the stationarity of the sweep fees is tested by measuring the level of mean reversion. Using a Dickey-Fuller statistical test the conduits are checked for approximate stationarity. Next, assuming the raw fee data is stationary, the proposed lognormal form of the model is investigated. A Jarque-Bera statistical test formalizes this step.


The Canadian conduits are shown to mean revert relatively fast. For these fee processes, a stationary model seems appropriate. The results for the US conduits are inconclusive though,
and on quantitative grounds alone it is difficult to justify a stationary process assumption. Associated Dickey-Fuller test results for the US conduits are not clear cut, and the fees do not appear to mean revert quickly. 

One potential problem is that observed conduit administration fee data is not corrected for reconsideration events. Displayed trending may actually be attributable to this fact. Results from further quantitative tests using supplied reconsideration event data are consistent with this theory. Ultimately, qualitative arguments based on knowledge of conduit fee evolution are needed to address the stationarity of the US conduits. Given the stationary property however, using a lognormal model for all of the conduits appears reasonable based on the Jarque-Bera results obtained using currently available fee data.

Projected fee values are required to receive preferential accounting treatment. A basic stationary process with an appropriate volatility was approved to forecast the conduit administration fees. This certification was made based on the historical data available at the time (see https://finpricing.com/lib/IrCurveIntroduction.html)
.
It is important to understand the general form of the stochastic process modeling conduit
administrations fees. Sweep fees are assumed to be described by a mean reverting process. Specifically, using F(t) to represent the sweep fee at time t we suppose that

 

where dWt is a standard Brownian motion process and log Ft is the natural logarithm of Ft.
The parameters a, μ and _ represent the speed of reversion, the mean reversion level and the volatility of the process respectively.

The solution to Equation (1) is known to be given by

 

where Zt+_t _ N(0, 1).

In order to investigate Ft it is useful to further define Yt = log Ft. With this substitution in mind we may rewrite Equation (1) and Equation (2) as

 

and

 

respectively. The motivation for this transformation lies in the form of Equation (4). Rearranging slightly, we may write

 

This form better illustrates the autoregressive nature of the process that is dependent on the speed of reversion. That is, if a is close to 0, _ is close to 0 and the process Yt is essentially geometric Brownian motion. On the other hand, if a is sufficiently large, _ approaches -1 and Yt is essentially stationary.

Assuming the speed of reversion is large, which is to say that the process Yt reverts quickly,
Equation (4) becomes

 

In terms of the actual conduit administration fee, Ft, this is

 

In terms of μ0 and _0 the process Yt follows

 

For each conduit, the proposed model in Equation (8) will be calibrated and used to forecast
sweep fees over a specific period. Previously the projected time horizon was 1 year, but it has been shortened to better coincide with the time between reconsideration events [5]. For Canadian conduits the forecast length of time will be 3 months, while for US conduits the projected time will be 1 month. GSG will use 3 years, or n = 36, previous historical data points to determine the model volatility, _0. Specifically, let ti represent a month end time. 

Model parameters will be based on observed conduit administration fees at some prior times t1, t2, . . . , tn, for example. Using 3 years worth of data that includes reconsideration events should produce a conservative estimate of the volatility. The model mean can not be estimated from historical data in the same way though, because the effect of reconsideration events on this parameter is not clear. Instead, GSG will set μ0 so that the expected value of Ft is the current sweep fee value. That is, once _0 is determined, μ0 is chosen to satisfy μ0e−1/2_02
= F0 or μ0 = e1/2_02F0.

