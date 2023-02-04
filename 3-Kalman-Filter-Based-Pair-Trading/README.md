Use Kalman filter to implement the pair trading strategy of S&P 500 ETF and the Dow Jones Industrial ETF. The strategy is based on J.P.Morgan's reseach "Dynamical 
Systems: Kalman Filtering". See the attached pdf for detail.

(a). Derive the beta update equation (Kalman filter) for the pair trading strategy of the two ETFs (which is the same format with the last equation on page 72 in the 
document for reference). The hand-written derivation is attached.

(b). Code up the pair trading strategy and compare rolling regression vs Kalman filtering.

Critical issue: The construction of the model is highly likely to be flawed. There's no way the model achieves 100-fold return. 
Action items: 
(1). Check-up model. Some first-line items are based on random generation from uniform distribution. This might be a flawed plausible approach, as each randseed returns very different results
(2). Vectorization of trading strategies and backtesting functions
(3). Pair quality validation - correlation/cointegration check (e.g. ARCH, GARCH, etc.)
