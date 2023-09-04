# Implied-Volatility
In this project, I implement a fast vectorized Newton-Raphson algorithm to calculate the implied volatility of option contracts

The implied volatility of an option contract is the forward-looking volatility input into a theoretical model, such that the model price 
matches the market price. The Newton–Raphson algorithm which is used in this project can return precise results in very few steps if a good initial guess is provided.<br>
Given these definitions:<br>
S - current price of underlying<br>
K - strike price of option contract<br>
T - time to maturity of option contract<br>
r - risk-free rate<br>
C - price of call option<br>
Let $`X={Ke^{-rT}}`$ and $`&delta;={(S-X)\over 2}`$
I explore two-methods of a good initial guess.<br>
The Brenner & Subrahmanyam approximation: $`&sigma;=\sqrt{2&pi;\over T} {C-&delta; \over S}`$<br>
The Corrado & Miller approximation: $`&sigma;=\sqrt{2&pi;\over T}{1\over S+X}{\bigg(C-&delta;+\sqrt{(C-&delta;)^2-{4&delta;^2\over &pi;}}\bigg)}`$ 
 
Giuseppe Orlando


## References
<a id="1">[1]</a> 
Giuseppe, O., Giovanni, T. (2017). 
A review on implied volatility calculation. 
Journal of Computational and Applied
Mathematics, 320, 202-220.

