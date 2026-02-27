# Simulation-of-Solidification-Aluminium
Numerical simulation of cooling and solidification behaviour in aluminium alloy using Python (Finite Difference Method).
# Simulation of Solidification – Aluminium

## Simulation of Solidification and Cooling Behavior in Aluminium Alloy Using Python.

---

## 📌 Project Overview

This project presents a numerical simulation of the cooling and solidification behaviour of a 2 cm thick aluminium alloy slab using Python.

The simulation is developed using the **Finite Difference Method (FDM)** to solve the one-dimensional transient heat conduction equation.  

The model predicts temperature evolution, phase transformation, and important solidification parameters during cooling from liquid state to solid state.

---

## 🎯 Objectives

The main objectives of this project are:

- Simulate the cooling curve at the center of the slab  
- Determine the solid fraction distribution  
- Calculate the final temperature distribution  
- Compute important thermal and solidification parameters  

---

## ⚙️ Material Properties and Input Parameters

- Density (ρ) = 2700 kg/m³  
- Thermal Conductivity (k) = 180 W/m·K  
- Specific Heat Capacity (Cp) = 900 J/kg·K  
- Latent Heat of Fusion (L) = 397,000 J/kg  
- Melting Temperature (Tm) = 660°C (933 K)  
- Slab Thickness = 0.02 m  
- Initial Temperature = 750°C  
- Ambient Temperature = 25°C  

---

## 🧮 Methodology

The simulation is based on:

- One-dimensional transient heat conduction equation  
- Explicit finite difference scheme  
- Phase change modelling using latent heat consideration  
- Time-stepping numerical approach  

Thermal diffusivity is calculated as:

α = k / (ρ Cp)

The Fourier number is used to analyze heat diffusion behaviour and numerical stability.

---

## 📊 Outputs Obtained

The following results are generated from the simulation:

1. Cooling Curve at the slab center  
2. Solid Fraction Distribution  
3. Final Temperature Distribution  
4. Mass of the slab  
5. Sensible heat removed  
6. Latent heat released  
7. Total heat removed  
8. Solidification time  
9. Maximum cooling rate  
10. Thermal diffusivity  
11. Fourier number  
12. Thermal gradient  
13. Solidification front velocity  

---

## 💻 Tools & Technologies Used

- Python  
- NumPy  
- Matplotlib  
- Google Colab  

---

## 📈 Significance of the Project

This project demonstrates the application of numerical heat transfer principles in metallurgical process simulation.

It helps in understanding:

- Cooling behaviour of metals  
- Solidification mechanisms  
- Heat transfer during casting  
- Computational modelling in materials science  

---

## 🚀 Future Improvements

- Extension to 2D simulation  
- Inclusion of convection boundary conditions  
- Modelling of alloy solidification range  
- Implementation of implicit numerical schemes  

---

## 👨‍🔬 Author

**Dhrubajyoti Bhattacherjee**  
Bachelor of Mechanical Engineering  
Interest Area: Materials Science & Metallurgical Simulation


## Source Code

The full simulation notebook is available here:

[Open the Jupyter Notebook]

(Solidification_Simulation_Aluminium.01.ipynb)


## Project Report

The complete research report can be downloaded below:

[Download the full report here]

(Solidification_Simulation_Report.pdf)
