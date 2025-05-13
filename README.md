# marnaPY

Analysis of EPANET reservoir level fluctuations.

Based on proprietary Python code from SUEZ (Ganessa, MultiPI, etc.).

## Project Structure

```
marnaPY/
├── src/           # Python source code
│   └── ...        # Python modules and packages
├── notebooks/     # Jupyter Notebooks
│   └── ...        # Example and analysis notebooks
├── data/          # Raw data (not versioned)
│   └── ...        # Input and output data files
├── tests/         # Unit tests
│   └── ...        # Test scripts
├── .gitignore
├── README.md
├── requirements.txt
├── environment.yml (for conda)
├── setup.py / pyproject.toml (for packaging)
```

## Dependencies

- Ganessa
  - en2emu.py
- OWA:EPANET_2.2

**Note:** This code will not work standalone and requires the above-mentioned utilities.
