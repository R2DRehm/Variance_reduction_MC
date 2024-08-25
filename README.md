# Variance_Reduction_MC

This repository contains five Jupyter notebooks demonstrating variance reduction techniques in Monte Carlo simulations. Below is a brief overview of each notebook:

1. **Antithetic Variable Method**:  
   This notebook introduces the antithetic variable method, a technique where negatively correlated pairs of variables are generated to reduce the variance of Monte Carlo estimates.

2. **Basket Options Pricing**:  
   This notebook explores the pricing of basket options. Techniques like control variates and antithetic variables are applied to improve the efficiency of Monte Carlo simulations used for option pricing.

3. **Control Variates Method (Delta Pricing)**:  
   Two approaches are compared for using Delta as a control variate in call option pricing:
   - **Method 1**: Adjusting the payoff \( E[\phi'(X_T^x) \cdot \frac{X_T^x}{x}] \).
   - **Method 2**: Adjusting the payoff \( E[\phi(X_T^x) \cdot \frac{W_T}{x \sigma T}] \).  
   The results show that Method 1 generally offers lower variance, while Method 2 is advantageous for specific payoff structures like digital options.

4. **Importance Sampling for Deep OTM Options**:  
   This notebook explores the use of importance sampling by shifting simulated paths to better capture scenarios that significantly impact deep out-of-the-money (OTM) options. The optimal shift \( \theta \) is determined, leading to substantial variance reduction.

5. **Comparing Variances Across Maturities**:  
   This notebook compares variance reduction techniques across different option maturities to identify which techniques are most effective depending on the context.
