# Manas Subbaraman

## Description

I aim to develop an interactive geospatial visualization exploring natural disaster risk across the United States. Using FEMA's National Risk Index (NRI) and demographic data from the American Community Survey (ACS) 2024 5-Year Estimates, the visualization will examine how disaster risk varies geographically, which hazards contribute to that risk, and how risk intersects with socioeconomic vulnerability.

The visualization will be an interactive county-level map allowing users to explore the distribution of overall disaster risk and individual hazards across the country. Users will be able to switch between different hazard types and risk metrics, zoom into specific states and counties, and select individual counties to examine their hazard profiles, demographic characteristics, and community resilience. The project may either incorporate supplementary visualizations (ex: bar graphs) or additional filters to explore relationships between disaster risk and demographic characteristics such as poverty, income, age, and disability.

My goal is to make disaster-risk data more accessible and encourage users to explore how natural hazards and socioeconomic conditions interact across American communities.

## Technical Plan re: Option A/B/C/D

I plan to pursue Option C, as the project is primarily centered around an interactive map and geographic exploration.

The main visualization will be a county-level choropleth map of the United States, with interactive controls allowing users to switch between hazard types, risk metrics, and potentially socio-economic characteristics. User can explore different geographic regions, and select counties to retrieve additional information. Selecting a county will update a supplementary information panel containing its risk profile, demographic characteristics, and hazard-specific measures.

The project will incorporate at least one custom JavaScript visualization using D3.js. This will either be a county-level hazard profile or a comparison chart displaying the risk and demographic characteristics of selected counties.

### Libraries and technologies:

- MapLibre GL JS: Interactive county-level mapping, choropleth layers, zooming, geographic navigation, and map interactions.
- D3.js: Custom interactive charts, including hazard profiles and county comparisons.
- HTML and CSS: Page structure, layout, styling, and interactive controls.
- JavaScript: Managing user interactions, updating map layers and charts, and coordinating data between components.
- Python (Pandas and GeoPandas): Cleaning, aggregating, joining, and preparing the NRI and ACS datasets for web visualization.

### Inspiration
1) FEMA Resilience Analysis and Planning Tool: https://www.fema.gov/emergency-managers/practitioners/resilience-analysis-and-planning-tool 
2) David Steffen's Project from Autumn 2024: https://capp-projects.civic.garden/projects/steffen-health-interactive/
3) Gabriel Barrett's project from Autumn 2024: https://capp-projects.civic.garden/projects/pl280ods/ 
4) A dashboard that I created over the summer for the Inter-American Development Bank (attaching mock-up since dashboard is still under development): 
![Alt text](images/EAST_Wireframe_07.02.26.png)

## Mockup
The first image will be the landing page of the visualization. Clicking on a state or county on the national map will open a new page with the state-level county map with further breakdowns.

![Alt text](images/Mockup_Page_1.jpg)
![Alt text](images/Mockup_Page_2.jpg)

## Data Sources

### Data Source 1: FEMA National Risk Index Data

URL: (https://www.fema.gov/flood-maps/products-tools/national-risk-index)

Size: 3233 rows, 465 columns

The FEMA National Risk Index (NRI) combines expected annual economic loss, social vulnerability, and community resilience to show which communities are at risk to 18 natural hazards. 

I have already used this dataset in my static visualization project, so I am familiar with its structure and variables. For the interactive visualization, I plan to use county-level data to let users explore overall and individual disaster-risk (for all 18 disasters), expected annual loss, social vulnerability, and community resilience.


### Data Source 2: American Community Survey 2024 5-Year Estimates

URL: https://data.census.gov/ 

Size: 3224 rows, Number of Columns varies by ACS table used

The ACS 2024 5-Year Estimates supplements the NRI data by helping the audience understand who lives in the most vulnerable communities and whether there are common characteristics among populations living in high-risk areas.

I plan to incorporate county-level data on age and sex, zero-vehicle households, income and poverty status, and disability. Since I have already used these datasets in the static visualization, I am familiar with their characteristics. For the interactive visualization, I plan to allow users to filter and explore different socioeconomic characteristics, with the possibility of providing more detailed breakdowns within each category.

## Questions

{Numbered list of questions for course staff, if any.}

1.
2.
3.