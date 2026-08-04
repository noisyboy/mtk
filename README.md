# Advanced Sol-Gel Perovskite Calculator

A lightweight, interactive stoichiometric calculator designed for condensed matter physics research. This tool automates precise precursor mass calculations for synthesizing complex, high-entropy, and oxyhalide magnetocaloric perovskites via the sol-gel method.

## Features
*   **Dynamic Stoichiometry:** Handles multi-element co-doping and vacancies across the A, B, and X sites ($A_{1-x}A'_{x}B_{1-y}B'_{y}O_{3-z}X_{z}$).
*   **Real-Time Purity Adjustment:** Compensate for batch-specific precursor assay variances (e.g., 99.0% vs 99.9%) directly in the UI without modifying the underlying code.
*   **Halide Integration:** Automatically routes X-site substitutions (F, Cl, Br, I) to their respective ammonium halide precursors while dynamically adjusting the target molar mass.
*   **Chelating Agents:** Calculate precise chelating and polymerization agent masses (e.g., Citric Acid, EDTA, Glycine) based on customizable molar ratios to the total metal ions.
*   **Zero Dependencies:** A single, self-contained HTML file. No backend server, package managers, or internet connection required.

## Usage
No installation required. Simply download the `.html` file and open it locally in your web browser to start calculating precursor weights for your sample palettes.
or use it online hosted [here](https://noisboy.qzz.io/solgel)
