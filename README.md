# Lucas Tree Asset‐Pricing Project

This repository implements the classic Lucas (1978) tree model of asset pricing.  
We start from a simplified theoretical model, then write a code to conduct comparative statics and micro-moment calibration.

---

## Project Overview

1. **Model & Theory**  
   We derive the recursive pricing equation  
   \[
     p(y) \;=\;\mathbb{E}\Bigl[\beta\,\frac{u'(y')}{u'(y)}\,(y'+p(y'))\Bigr]
   \]
   under CRRA utility \(u(c)=c^{1-\gamma}/(1-\gamma)\).  
2. **Numerical Solution**  
   We discretize the dividend (or consumption) process via Rouwenhorst’s method, solve the fixed-point problem \(f = T f\) by value‐function iteration, and recover the equilibrium price function \(p(y)\).  
3. **Micro-Moment Calibration**  
   We calibrate the coefficient of relative risk aversion \(\gamma\) (holding \(\beta\) at 0.95) to match the historical U.S. **equity premium** (6 % p.a.), using simulated equity returns and the model’s stochastic discount factor.
