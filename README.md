# Stochastic Interest Rate Modelling and Yield Curve Reconstruction using the CIR Model

## Overview

This project implements, calibrates, and evaluates the Cox–Ingersoll–Ross (CIR) stochastic interest rate model on historical yield curve data. The objective is to reconstruct the entire yield curve using only the 3-Month yield as a proxy for the short-term interest rate and evaluate the model's ability to capture real-world term structure dynamics.

The project was developed as part of the Finance Club, IIT Roorkee Open Projects program.

## Key Features

* Data preprocessing and cleaning of historical yield data
* CIR model implementation from first principles
* Parameter calibration using historical market data
* Yield curve reconstruction from a single observable short-rate input
* Out-of-sample prediction and performance evaluation
* Extension of the baseline CIR framework
* Quantitative analysis of model assumptions and limitations

## Mathematical Framework

The CIR short-rate process is defined as:

dr(t) = κ(θ − r(t))dt + σ√r(t)dW(t)

where:

* κ : Mean reversion speed
* θ : Long-run mean level
* σ : Volatility parameter
* W(t) : Standard Brownian motion

The model guarantees non-negative interest rates under the Feller condition:

2κθ ≥ σ²

Using the calibrated parameters, zero-coupon bond prices and corresponding yield curves are generated and compared against observed market data.

## Results

The project evaluates:

* Calibration quality
* Yield curve reconstruction accuracy
* Out-of-sample R² performance
* Cross-sectional fit across maturities
* Impact of model extensions

## Technologies Used

* Python
* NumPy
* Pandas
* SciPy
* Matplotlib
* Scikit-Learn
* google colab

## Repository Structure

* notebooks/ : Model implementation and experiments
* images/ : Generated figures and visualizations
* data/ : Sample datasets
* docs/ : Supporting documentation

## Future Improvements

* Multi-factor CIR models
* CIR++ framework
* Jump-diffusion extensions
* Kalman filter based estimation
* Real-time yield curve forecasting

## Author

SURYA AKHIL
B.Tech, IIT Roorkee
