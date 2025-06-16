# Stock Price Simulation using Monte Carlo Method

This repository provides a simple Python implementation for simulating stock price movements using the **Monte Carlo method**. It models stock price dynamics over time using the geometric Brownian motion process and visualizes multiple simulations.

## 📁 File

- `Stock_prices_using_monte_carlo_simulation.py`:  
  Runs 100 simulations of a stock's future price path based on specified drift and volatility using Monte Carlo techniques.

## 🧠 Concept

Stock price at time \( t+1 \) is modeled as:

\[
S{t+1} = S(t) * exp[(mu - 0.5 * sigma ** 2) + sigma * Z]
\]

Where:
- \( S(0) \): Initial stock price  
- \( \mu \): Expected return (drift)  
- \( \sigma \): Volatility  
- \( Z \sim N(0, 1) \): Standard normal variable

This simulation runs for **252 trading days** (1 year) and averages over 100 independent paths.

## 📊 Output

- Line plot of the average simulated stock price path over time.
- Console output displaying the predicted final price.

## 🔧 How to Use

### Prerequisites

Install required packages:

```bash
pip install numpy pandas matplotlib
