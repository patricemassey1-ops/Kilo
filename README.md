# Calculateur Fantrax 2025 (Streamlit)

Application Streamlit pour importer des exports Fantrax (skaters/goalies), calculer la masse salariale par propriétaire, et simuler des mouvements entre **Grand Club** et **Club École**.

## Prérequis

- Python 3.9+ (utilise [`zoneinfo.ZoneInfo()`](app.py:6))

## Installation

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Lancer

```bash
streamlit run app.py
```

## Fichiers attendus / générés

- `Hockey_Players.csv` : base joueurs (optionnelle). Chargée par [`charger_db_joueurs()`](app.py:44).
- `historique_fantrax_v2.csv` : historique des imports (généré/écrit automatiquement).
- `rachats_v2.csv` : rachats (généré/écrit automatiquement).
