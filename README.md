# The Lucas Tree Model of Asset‐Pricing

This repository implements the classic Lucas (1978) tree model of asset pricing.  
We start from a simplified theoretical model, then write a code to conduct comparative statics and micro-moment calibration.

---

## Project Overview

1. **Model & Theory**  
   We derive the recursive pricing equation in a representative agent model with endowment and a single asset.  
2. **Numerical Solution**  
   We discretize the dividend (or consumption) AR(1) process via Tauchen’s method and solve the fixed-point problem by value‐function iteration, and recover the equilibrium price function.  
3. **Micro-Moment Calibration**
   We calibrate the coefficient of relative risk aversion and discount factor to match real-world risk-free rate and equity premium.
