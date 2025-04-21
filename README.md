---

# HGWMPA: Hybrid Grey Wolf and Marine Predators Algorithm for Global Optimization

This repository provides the MATLAB implementation of **HGWMPA**, a hybrid metaheuristic algorithm combining the exploration capabilities of the Marine Predators Algorithm (MPA) with the exploitation efficiency of Grey Wolf Optimization (GWO). It is designed for solving complex global optimization problems with enhanced convergence speed and solution quality.

## 📁 Repository Contents

The ZIP file includes six MATLAB scripts required to run the HGWMPA algorithm:

| File Name          | Description |
|--------------------|-------------|
| `HGWMPA.m`         | Main algorithm that integrates Grey Wolf Optimization (GWO) and Marine Predators Algorithm (MPA) dynamics. |
| `initialization.m` | Initializes the search agent positions within specified upper and lower bounds. |
| `levy.m`           | Generates Levy flight-based random numbers for MPA-style random walks. |
| `Get_F.m`          | Defines benchmark test functions (e.g., F1 to F23) and returns their lower/upper bounds and objective function handles. |
| `func_plot.m`      | Plots 2D/3D visualizations of the test functions. |
| `main.m` or `demo.m`| Main demo file (integrated in HGWMPA.m in this version). Runs the optimization and plots results. |

## 📈 Algorithm Highlights

- **Exploration Phase (MPA-based)**: Random walk behavior using Levy distribution for diverse search space sampling.
- **Exploitation Phase (GWO-based)**: Social hierarchy (Alpha, Beta, Delta) based convergence for refined search near optima.
- **Adaptive Switching**: The algorithm automatically transitions from exploration to exploitation based on the iteration count.

## 🧪 How to Run

1. Extract the contents of the ZIP file.
2. Open **MATLAB**.
3. Navigate to the extracted folder.
4. Run the main script:
```matlab
HGWMPA
```

## 🧮 Parameters

- `N`: Number of search agents (default: 100)
- `Max_iter`: Maximum number of iterations (default: 500)
- `F_name`: Name of the benchmark function (e.g., `'F1'`)

These can be modified in the `HGWMPA.m` script.

## 📊 Output

- **Convergence Curve**: Shows the decrease in fitness value over iterations.
- **Function Plot**: 3D visualization of the selected benchmark function.
- **Console Output**: Best solution vector and its corresponding objective function value.

## 🧠 Authors

- **Saptadeep Biswas** – [Email](mailto:saptadeepbiswas7@gmail.com)
- **Binanda Maiti** – [Email](mailto:matheaticsbinanda@gmail.com)

## 💻 System Specifications

- Tested on: **Intel Core i7-11700**, **16GB RAM**
- MATLAB Version: **2021a**
- OS: **Windows 11 (64-bit)**

## 📜 Citation

If you use this code in your research, please cite the authors appropriately. A paper detailing the method will be available upon publication.

---
