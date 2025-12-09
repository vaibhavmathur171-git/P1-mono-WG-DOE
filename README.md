# P1-Mono Waveguide ML Design Tool

**AI-Powered Inverse Design for Optical Gratings**

## Overview

Neural network tool for inverse design of optical waveguide gratings. Input a target diffraction angle, get the required grating period instantly.

## Features

- Interactive design tool with real-time predictions
- Physics-based verification of ML predictions
- Full factorial Design of Experiments analysis
- Performance visualization and error analysis

## Model Performance

- **MAPE**: <0.5% on test data
- **Wavelength**: 550 nm (green light)
- **Training**: 10,000 synthetic samples
- **Architecture**: Optimized via DoE (60 experiments)

## Technology Stack

- Streamlit for web interface
- Plotly for interactive visualizations
- Pandas/NumPy for data processing

## Physics

Implements the grating equation:

n(sin θ_out - sin θ_in) = m·λ / Period

Where:
- n = 1.5 (refractive index)
- θ_in = 0° (normal incidence)
- m = -1 (diffraction order)
- λ = 550 nm (wavelength)

## Design of Experiments

Full factorial analysis exploring:
- Dataset sizes: 500 to 10,000 samples
- Network depths: 1 to 4 layers
- Training epochs: 50 to 200 epochs

Total: 60 configurations tested to find optimal architecture

## Quick Start

Clone and run locally:

git clone https://github.com/YOUR_USERNAME/p1-mono-waveguide.git
cd p1-mono-waveguide
pip install -r requirements.txt
streamlit run app.py

## License

MIT License

## Author

Your Name
