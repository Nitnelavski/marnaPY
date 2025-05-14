# marnaPY

**marnaPY** is a Python package and Jupyter notebook toolkit for analyzing reservoir level fluctuations (marnages) in EPANET water distribution network models.

This project is based on proprietary Python code from SUEZ (notably Ganessa and MultiPI) and leverages the OWA-EPANET 2.2 engine for hydraulic simulations.

---

## Features

- Interactive Jupyter notebook for analyzing minimum and maximum reservoir levels over a simulation period.
- Integration with EPANET input files (`.inp`) for hydraulic modeling.
- Extraction and reporting of tank pressure statistics.
- Modular code structure for extension and testing.

---

## Project Structure

```
marnaPY/
├── src/                # Python source code (modules, package __init__)
│   └── __init__.py
├── notebooks/          # Jupyter Notebooks for analysis
│   └── analyse_marnage.ipynb
├── data/               # Raw data (not versioned by git)
│   ├── modele.inp      # Example EPANET input file
│   └── analysis.txt    # Output statistics
├── tests/              # Unit tests
│   └── test_analyses_marnages_v3.py
├── utils/              # Hidden utility scripts
├── .gitignore
├── README.md
├── requirements.txt
├── environment.yml     # Conda environment definition
├── pyproject.toml      # Project metadata and build config
```

---

## Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/ValentinMounier/marnaPY.git
   cd marnaPY
   ```

2. **Set up the environment:**
   - Using conda:
     ```sh
     conda env create -f environment.yml
     conda activate marnaPY-env
     ```
   - Or using pip:
     ```sh
     pip install -r requirements.txt
     ```

3. **Install OWA-EPANET and Ganessa dependencies as required.**

---

## Usage

- Open the Jupyter notebook:
  ```sh
  jupyter notebook notebooks/analyse_marnage.ipynb
  ```
- Follow the notebook instructions to select your EPANET `.inp` file and simulation parameters.
- The notebook will run the simulation, extract tank pressures, and save the results to `data/analysis.txt`.

---

## Dependencies

- Python >= 3.8
- numpy
- pandas
- jupyter
- [Ganessa](https://github.com/SUEZ-Global/ganessa) (including `en2emu.py`)
- [OWA-EPANET 2.2](https://github.com/OpenWaterAnalytics/EPANET)

See `requirements.txt` and `environment.yml` for details.

---

## Notes

- The code relies on proprietary and external utilities (Ganessa, MultiPI, OWA-EPANET). It will not work standalone without these.
- The `data/` directory is not versioned and should be used for your input/output files.
- The `utils/` directory contains additional scripts for advanced analysis.

---

## License

Proprietary. See `pyproject.toml` for details.

---

## Author

Valentin Mounier  
[GitHub](https://github.com/valmoun)

---

## Issues

For bug reports or feature requests, please use the [GitHub Issues page](https://github.com/ValentinMounier/marnaPY/issues).
