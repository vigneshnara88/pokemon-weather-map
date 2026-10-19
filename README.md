# Pokémon in the real world

A group data-science project mapping Pokémon to real-world weather and geographic conditions. The project focuses on fire, ice and water types, combining Pokémon attributes with rankings of hot, cold and wet locations to build a playful geographic mapping.

**Team Error_105:** Adrian, Hailey, Jonathan and Vignesh. This repository presents the work as a group project.

## Workflow

| Component | Contents |
| --- | --- |
| `code/data_collection/01_collection.ipynb` | Pokémon and species data collection, with JSON outputs. |
| `code/data_collection/process_biomes.py` | Ecoregion-centroid extraction through Google Earth Engine. |
| `code/data_processing/02_processing.ipynb` | Type filtering, rankings and SQLite table construction. |
| `code/weather/04_weather.ipynb` | Weather collection, location ranking, geographic joins, SQLite export and Folium maps. |
| `code/data_visualisation/03_visualisation.ipynb` | Exploratory plots and geographic visualisation. |

Pokémon attributes and place conditions are linked using explicit ranking rules. This is a creative data project; the mapping is a heuristic rather than a scientific model of where fictional species would live.

## Working with the code

Use a Python environment with the dependencies in `requirements.txt` and a Jupyter frontend. Open each notebook from its own directory so its `../../data/` and `../../outputs/` paths resolve to the repository root.

The sequence is collection, weather preparation, processing and visualisation. Individual notebooks contain exploratory cells and may require outputs from an earlier stage. Review their input paths before use. Supply geographic and weather inputs locally; source datasets, SQLite databases, downloaded media and generated maps are excluded from this repository.

The biome utility expects `GEE_SERVICE_ACCOUNT` and `GEE_PRIVATE_KEY_PATH` in the local environment, together with authorised access to Earth Engine. Credential files and `.env` files stay outside version control. The collection notebooks access external services when run; no service calls are required simply to read the project.

## Data and outputs

The code documents data collection and processing. Notebook outputs and embedded media have been cleared. Pokémon names and other franchise material belong to their respective rights holders; no official affiliation is implied. Any downloaded datasets or media remain subject to their source terms.
