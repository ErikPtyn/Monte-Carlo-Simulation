****Valuation of a European Call Option using Monte Carlo Simulation
**General Idea
This project focuses on implementing a Monte Carlo simulation for pricing a European call option under the Black-Scholes-Merton (BSM) framework. The underlying asset's risk factor is assumed to follow a geometric Brownian motion, aligning with the assumptions of the BSM model.

This project is part of a financial computing initiative and serves as a demonstration of our proficiency in applying Python to financial engineering. Although the primary goal is to showcase our understanding of the theoretical framework and implementation, we have made every effort to ensure the project is as rigorous as possible within our current academic level.

Black-Scholes-Merton Model Assumptions
The risk-free interest rate is known and constant.
The underlying asset's returns follow a normal distribution.
The volatility of the asset remains constant.
No dividends are considered initially (though the model can be adjusted to include them).
No transaction costs are assumed.
The underlying asset is infinitely divisible, allowing fractional trades.
Short selling of the underlying asset is allowed.
Monte Carlo Simulation for Option Pricing
The Monte Carlo method is a numerical approach used to approximate the expected payoff of a financial derivative. It involves simulating multiple paths for the underlying asset price and computing the option payoff for each scenario. The average discounted payoff provides an estimate of the option price.

Attributes
The project includes parameters essential for pricing a European call option using Monte Carlo simulation under the BSM framework:

Initial asset price 
𝑆
0
S 
0
​
 
Strike price 
𝐾
K
Time to maturity 
𝑇
T
Risk-free interest rate 
𝑟
r
Volatility 
𝜎
σ
Number of simulations 
𝑁
N
Methods
.simulate_paths()
Generates multiple simulated paths for the underlying asset based on geometric Brownian motion.

.monte_carlo_pricing()
Estimates the option price by averaging discounted payoffs from simulated asset price paths.

.black_scholes_formula()
Provides a reference calculation using the Black-Scholes analytical formula for European options.

.compare_monte_carlo_vs_BS()
Compares the Monte Carlo estimated option price with the analytical Black-Scholes price to validate the accuracy of the simulation.

.plot_simulated_paths()
Visualizes the simulated asset price trajectories over time.

Test File
A dedicated test script is provided to instantiate options, compute their Monte Carlo prices, compare them to Black-Scholes values, and evaluate the accuracy of the simulation.

Future Enhancements
Implementing variance reduction techniques to improve Monte Carlo efficiency.
Extending the model to include dividend-paying assets.
Performing sensitivity analysis on option price with respect to input parameters.
This project serves as a foundation for exploring option pricing techniques and evaluating the robustness of the Monte Carlo approach in financial modeling.
