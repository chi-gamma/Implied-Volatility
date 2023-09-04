# Implied-Volatility

The implied volatility of an option contract is the volatility input into a theoretical model, such that the model price matches the market price.
In contrast to historical realized volatility, implied volatility is forward-looking.
The mapping between the option price and black-scholes model implied volatility is a unique one-to-one mapping.
There is no closed-form to determine the implied volatility from an option price hence it is calculated using numerical approximation methods.

The Newton–Raphson algorithm which is used in this project can return precise results in very few steps if a good initial guess is provided.
I explore two-methods of a good initial guess: The Brenner & Subrahmanyam approximation and the Corrado-Miller approximation.
