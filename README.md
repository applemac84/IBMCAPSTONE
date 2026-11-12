# IBMCAPSTONE

IBM Data Science Professional Certificate capstone: predicting whether the SpaceX Falcon 9 first stage will land successfully.

## Notebooks and files

| Step | File |
| --- | --- |
| EDA with SQL | [jupyter-labs-eda-sql-coursera_sqllite.ipynb](jupyter-labs-eda-sql-coursera_sqllite.ipynb) (data: `Spacex.csv`) |
| EDA with data visualization | [edadataviz.ipynb](edadataviz.ipynb) (data: `dataset_part_2.csv`, `dataset_part_3.csv`) |
| Interactive map with Folium | [lab_jupyter_launch_site_location.ipynb](lab_jupyter_launch_site_location.ipynb) (data: `spacex_launch_geo.csv`; the maps are also saved as HTML in [maps/](maps/) because GitHub does not render Folium output) |
| Plotly Dash dashboard | [spacex_dash_app.py](spacex_dash_app.py) (data: `spacex_launch_dash.csv`; run with `python spacex_dash_app.py`, then open http://127.0.0.1:8050) |
| Classification (LogReg, SVM, Tree, KNN) | [SpaceX_Machine Learning Prediction_Part_5.ipynb](SpaceX_Machine%20Learning%20Prediction_Part_5.ipynb) |

Screenshots of the Folium maps and the Dash dashboard are in [screenshots/](screenshots/).

## Dashboard findings (from `spacex_launch_dash.csv`, 56 launches)

1. Largest number of successful launches: KSC LC-39A (10).
2. Highest launch success rate: KSC LC-39A (10 of 13, 76.9%).
3. Highest success rate by payload range (1000 kg slider steps): 3000-4000 kg (8 of 11, 72.7%).
4. Lowest success rate by payload range: 6000-7000 kg (0 of 4); the 0-1000 kg range is next lowest (2 of 10, 20%).
5. Booster version with the highest success rate: B5 (1 of 1, a single launch), then FT (16 of 24, 66.7%), the best result with a meaningful number of launches.
