### Project 3 University of Minnesota Data Visualization and Analytics Boot Camp
# World CO<sub>2</sub> Emissions Dashboard:

Project Team Members: Ben Johnson, Joey Eikens, Yameena Khan, Zach Wood & Oscar Iwu
____________
## About 
This repo contain code and instructions to reproduce the CO<sub>2</sub> Emission Dashboard our groups has created. Our dashboard displays global emissions data from 1972 - 2020. The centerpiece of the dashboard, an interactive map, drives the user experience. Navigate through the emissions data by clicking a country on the map and selecting a year with the dropdown menu. The following emissions data is shown:
- Population, country's GDP, CO<sub>2</sub> per capita and country's global CO<sub>2</sub> contribution
- Top 10 contributors in global emissions in a given year
- The selected countries % contribution to the world's CO<sub>2</sub> in a particular year
- Total CO<sub>2</sub> per year
- Breakdown of %CO<sub>2</sub> contributions by different sources (coal, oil, gas, cement)

<p align="center">
  <img src="Images/dashboard.png" />
</p>


____________
## Technologies and Tools Used:

- PostgreSQL
- Jupyter Notebook/Pandas
- Flask 
- Bootstrap
- Charts.js
- Leaflet.js
- Plotly.js

_____________
## Contents of the Repo:

- app.py
- co2_ETL.ipynb
- world-co2-omissions.sql
- templates
  - index.html
- static
  - css
    - style.css
  - data
    - countries1.geojson
  - js
    - logic.js
    - scatter_plot.js
    - year_dropdown.js


_____________
## Instructions on how to use our Dashboard:

1. Clone the repo to your machine
1. Open the pgAdmin app on your machine
1. Create a new database called ``world_carbon_emissions_db`` 
1. Open the query tool within the ``world_carbon_emissions_db`` 
1. Open the ``world-co2-omissions.sql`` file stored in the repo cloned within PostgreSQL
1. Highlight the code to create tables for the ``world_co2``
1. Once the table is created right click on the local repo and then launch a Git Bash (Windows) or Terminal (Mac)
1. Type ``source activate PythonData38`` and then click ``enter`` to activate PythonData38 environment 
1. Launch Jupyter Notebooks in Google Chrome, by typing the command ``jupyter notebook`` on your Gitbash/Terminal window and then click ``enter``
1. Open the ``co2_ETL.ipynb``
1. Run all the cells peforming the ETL process
1. After that close the Jupyter Notebooks and exit the Gitbash/Terminal window
1. Navigate back to the local repo folder, right click on the local repo folder and open a new a Git Bash/Terminal window
1. Type ``source activate PythonData38`` and then click ``enter`` to activate PythonData38 environment 
1. Type ``python app.py`` and then hit ``enter``
1. Observe that the Flask server starts and tells you which port it's running on. Don't close this window.
1. With the Flask server running, enter this address in your Chrome browser: http://127.0.0.1:5000/. You will see that it loads the index page which is our World CO<sub>2</sub> Emissions Dashboard.
1. The data used in the dashboard can be found by following the /data route.
