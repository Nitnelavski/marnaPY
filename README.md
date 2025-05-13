# marnaPY
Analyse des marnages de réservoirs EPANET.

Basé sur du code Python propriétaire de SUEZ.
(Ganessa, MultiPI, etc.)

## Project structure
marnaPY/
├── src/           # Python source code
├── notebooks/     # Jupyter Notebooks
├── data/          # Raw data (not versioned!)
├── tests/         # Unit tests
├── .gitignore
├── README.md
├── requirements.txt
├── environment.yml (for conda)
├── setup.py / pyproject.toml (if packaging)

## Dépendances
* Ganessa
  * en2emu.py
* OWA:EPANET_2.2

Ce code ne fonctionnera pas de manière autonome, et nécessite la possession des utilitaires précédemment cités.
