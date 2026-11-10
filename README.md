# How Do Cold-Nights Affect Vertical Snow Temperature Gradients and Near-Isothermal Snowpack Structure?

## 2026 ATOC 4500-5500 Capstone Final Project — Polar Ice & Climate
**Authors:** Cece, Jordan, Anna  
**Institution:** University of Colorado Boulder  
**Term:** Spring 2026

---

## 📌 Project Overview
This repository contains the data, analysis scripts, and visualization code evaluating how ambient air temperature fluctuations—specifically overnight cold periods and subsequent daytime warming—influence the internal thermodynamic structure, vertical temperature gradients, and grain metamorphism of a seasonal alpine snowpack. 

By analyzing physical field measurements alongside regional SNOTEL automated weather station data, this project characterizes the transition of the winter snowpack from a high cold-content reservoir to a near-isothermal, melt-ready system.

## 🔬 Research Question & Hypothesis
* **Core Question:** How do cold-nights affect vertical snow temperature gradients and near-isothermal snowpack structure?
* **Hypothesis:** Internal, lower-density layers within the mid-snowpack act as thermal insulation barriers. This insulation limits immediate responses to superficial diurnal temperature ranges, preserving historical subfreezing cold-content even as ambient air temperatures climb toward melting conditions.

---

## 📊 Data Sources & Methods
The analysis pairs regional meteorology with direct physical stratigraphy gathered near the **Niwot Ridge SNOTEL C1 station** (Colorado, USA):
1. **Automated Meteorological Data:** Daily minimum (\(T_{min}\)) and maximum (\(T_{max}\)) ambient air temperatures, snow water equivalent (SWE), and total depth records sampled during March 2026.
2. **Field Stratigraphy Profiles:** Vertical profile data collected across two distinct field days:
   * **March 4, 2026:** Representing a snowpack developed under sustained, severe overnight subfreezing conditions (3-day average \(T_{min} \approx -4.22^\circ\text{C}\)).
   * **March 27, 2026:** Representing a snowpack exposed to significant late-season daytime warming (3-day average \(T_{min} \approx +1.74^\circ\text{C}\)).

### Key Analytical Techniques
* **3-Day Diurnal Windows:** Calculated rolling averages of meteorological parameters preceding field days to minimize high-frequency noise and accurately assess the antecedent cold-content.
* **Thermodynamic Profiling:** Evaluated physical temperature gradients (°C/cm) mapped continuously from the surface down to the basal boundary layer.
* **Structural Metamorphism Tracking:** Monitored changes in density (kg/m³) and crystal grain sizes to trace historical phase-change signatures trapped within the layers.

---

## 📈 Key Findings
* **Thermal Lag & Insulation:** A persistent low-density mid-layer acts as an insulating blanket. This layer allows the upper snowpack to respond quickly to air temperatures while isolating deeper layers, maintaining subfreezing temperatures on March 4.
* **Isothermal Transition:** Over the course of March, the internal energy deficit was overcome. By March 27, the entire vertical column achieved an isothermal state resting at a uniform 0°C, indicating a system primed for rapid spring melt.
* **Hysteresis in Grain Growth:** Large depth-hoar crystals observed at the base of the March 4 profile reflect antecedent thermal gradients rather than immediate ambient conditions, proving that morphological changes lag behind current weather.

---

## 📁 Repository Structure
```text
├── Data/
│   ├── Fieldwork_near_Niwot_SNOTEL_March4_March27_2026.csv   # Raw manual snow pit data
│   └── NIWOT_snowtel_20261001-20260327.csv                   # SNOTEL meteorological dataset
├── Notebooks/
│   └── Capstone_Project_Analysis.ipynb                        # Primary Jupyter Notebook containing code
├── Figures/
│   ├── March_Tmin_Diurnal_Comparison.png                     # Time-series and 3-day diurnal plots
│   └── Snowpack_Isothermal_Warming_Profiles.png              # Vertical temperature & grain size profiles
└── README.md                                                 # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites
To run the analysis and reproduce the figures, ensure you have Python 3.12+ installed along with the following ecosystem libraries:
```bash
pip install numpy pandas matplotlib scipy
```

### Running the Analysis
1. Clone this repository to your local directory.
2. Ensure the data paths within the script point correctly to your local environment file directories.
3. Run the complete notebook pipeline to generate data figures:
```bash
jupyter notebook Notebooks/Capstone_Project_Analysis.ipynb
```

---

## 📚 References
* Burns, S. P., Molotch, N. P., Williams, M. W., Knowles, J. F., Seok, B., Monson, R. K., Turnipseed, A. A., & Blanken, P. D. (2014). *Snow temperature changes within a seasonal snowpack and their relationship to turbulent fluxes of sensible and latent heat.* Journal of Hydrometeorology, 15(1), 117–142.
* Jennings, K. S., Kittel, T. G. F., & Molotch, N. P. (2018). *Observations and simulations of the seasonal evolution of snowpack cold content and its relation to snowmelt and the snowpack energy budget.* The Cryosphere, 12, 1595–1614.
