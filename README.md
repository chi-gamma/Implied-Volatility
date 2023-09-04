# Implied-Volatility

The implied volatility of an option contract is the forward-looking volatility input into a theoretical model, such that the model price 
matches the market price and this mapping between the option price and implied volatility is a unique one-to-one mapping.
There is no closed-form formula to determine the implied volatility from an option price hence it is calculated using numerical approximation methods.

The Newton–Raphson algorithm which is used in this project can return precise results in very few steps if a good initial guess is provided.
Given these definitions
S - current price of underlying
K - strike price of option contract
T - time to maturity of option contract
r - risk-free rate
C - price of call option
I explore two-methods of a good initial guess.
The Brenner & Subrahmanyam approximation: 
$$&sigma;=\sqrt{2&pi;\over T} {C-&delta; \over S}$$
where $`&delta;={(S-X)\over 2}`$ and $`X={Ke^{-rT}}`$

