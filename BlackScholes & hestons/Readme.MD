# 📊 Option Pricing Models: Black-Scholes, Heston & Hybrid Approach

## 📌 Overview

This repository presents a comprehensive study and implementation of **option pricing models** used in quantitative finance. It focuses on comparing the classical **Black-Scholes model** with the more advanced **Heston stochastic volatility model**, and proposes a **hybrid approach** that combines the strengths of both.

The project is structured as a **Phase-I research report**, with future scope for full implementation and validation.

---

## 🎯 Objectives

* Understand the fundamentals of **financial derivatives and option pricing**
* Study and implement the **Black-Scholes model**
* Analyze the **Heston stochastic volatility model**
* Compare both models in terms of:

  * Accuracy
  * Computational complexity
  * Real-world applicability
* Propose a **Hybrid Heston–Black-Scholes model**
* Formulate a **testable hypothesis for performance improvement**

---

## 🧠 Models Covered

### 1. Black-Scholes Model

* Assumes **constant volatility**
* Provides **closed-form solutions**
* Widely used in industry

**Key Equation:**

```
C = S·N(d1) − K·e^(−rT)·N(d2)
```

---

### 2. Heston Model

* Uses **stochastic (time-varying) volatility**
* Captures:

  * Volatility smile
  * Leverage effect
* More **realistic but computationally expensive**

---

### 3. Hybrid Model (Proposed)

* Uses **Heston-derived effective volatility**
* Applies it within the **Black-Scholes formula**
* Goal:

  * Maintain speed of Black-Scholes
  * Achieve accuracy close to Heston

---

## 🔬 Hypothesis

> Substituting stochastic volatility from the Heston model into the Black-Scholes formula significantly improves pricing accuracy while maintaining computational efficiency.

---

## 📊 Key Concepts

* Option Pricing
* Volatility (Historical & Implied)
* Volatility Smile & Skew
* Stochastic Processes
* Mean Reversion
* Computational Finance

---

## 🛠️ Methodology (Planned Phase-II)

1. Implement Black-Scholes model
2. Implement Heston model (Fourier-based)
3. Generate simulated market data
4. Develop hybrid model
5. Evaluate using:

   * MAE (Mean Absolute Error)
   * RMSE
   * MAPE
6. Visualize results:

   * Volatility surfaces
   * Pricing errors
   * Performance benchmarks

---

## 📈 Expected Results

* 🔹 50–70% reduction in pricing error vs Black-Scholes
* 🔹 Near-Heston accuracy
* 🔹 100–1000× faster than full Heston model

---

## 📂 Repository Structure

```
📁 option-pricing-project
│
├── 📄 report.pdf                 # Final Phase-I report
├── 📄 ieee-paper.pdf            # IEEE formatted version
├── 📄 README.md                 # Project documentation
│
├── 📁 src (future work)
│   ├── black_scholes.py
│   ├── heston_model.py
│   ├── hybrid_model.py
│
├── 📁 data
│   └── simulated_data.csv
│
├── 📁 results
│   ├── graphs/
│   └── metrics/
```

---

## 🚀 Applications

* Quantitative Trading Systems
* Risk Management
* Portfolio Optimization
* Derivatives Pricing Engines
* FinTech Platforms

---

## 📚 References

* Black, F. & Scholes, M. (1973)
* Merton, R. (1973)
* Heston, S. (1993)
* Hull, J. – *Options, Futures and Other Derivatives*

---

## 👨‍💻 Author

Ved Bajaj
COEP Technological University, Pune

---

## 🔮 Future Work

* Real market data calibration
* Extension to:

  * Jump-diffusion models
  * Rough volatility models
* Integration with **Machine Learning**
* Deployment in **real-time trading systems**

---

## ⭐ Contribution

Feel free to fork, improve, and contribute to this project!

---
