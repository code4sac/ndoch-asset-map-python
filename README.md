## Code of America - NDoCH 2020

![03.06_sac_lihm_choropleth][99.06]

### Code for Sacramento: Equity Asset Map Project

*Change Log*
* 08-21-2020: Baseline Version v0.1

### Introduction
This project focuses on the asset map item for the Code for America (CFA) National Day of Civic Hacking (NDocH) [event][02.01]; it consists of this notebook to visualize various assets within the Sacramento area. The data is sourced from various open data portals and provides the deliverables listed below.

*Deliverables*
1. Asset Maps: Shared as HTML files in maps folder and within notebook
2. Notebook: Contains all code and documentation needed for visualization
3. Documentation: Notebook and README contains full write-up and results

> Note: Data processing and maps are created using Jupyter Notebook due to its ability to visualize results effectively and efficiently. Listed below are installation instructions and more about Jupyter and Python.

### CFA NDoCH
The event NDoCH instructions are shown below and specify that open data sources should be used to visualize resources available to the Sacramento community. This notebook is intended as starting point to visualize such data for further development.

> Asset mapping is an integral part of empowered community building that is based on understanding the strengths and needs of diverse communities. First, use publicly available information about your locale to give a sense of the landscape and demographics. Next, research the location and availability of government programs (e.g. county health and human services offices), community based organizations (like resource centers, food banks, and legal aid clinics) or other resources that are vital to your community. Visually documenting the landscape can help identify what might make your community more equitable and accessible to all who live there.

### Methodology
This notebook starts with a tutorial using Python mapping tools as a prototype, then develops asset maps for the Sacramento area. Open data sources are listed below and will be added to with additional development.

> One desired outcome for this project is to develop a better understanding of publicly available data, appropriate tools and spatial analysis technique in develop the asset maps. As a result, project methodology, assumptions and results are documented in this readme.

Key project assumptions are listed below and validated through analysis and visualization of publicly available datasets. They serve as an outline for guide development of the notebook, analysis and visualizations.

*Assumptions*
1. Publicly available data via open data portals are typically good quality and therefore suitable for use in generating equity/asset maps
2. Data science tools such as Jupyter, Python and the Folium plotting package are appropriate tools to analyze, communicate and share results
3. All selected tools are open-source software, and all analysis is repeatable, documented and reproducible to improve accessibility  

### Results
Asset maps are summarized below and organized into separate modules within the notebook. Each map is available as a separate HTML file in the maps folder.

*Data Processing Steps*
1. Import raw data, then process it with helper functions as needed
2. Lat/long coordinate CSV and GeoJSON formats used for analysis
3. GeoJSON data was converted to JSON for plotting within Folium
4. Geospatial data was plotted with helper functions
5. Complete map is output within notebook and as separate file

### Map 1: SFPD Crime Reports (2003-2018)

![03.01_sfpd_reports][99.01]

*Map Legend*
* SFPD Crime Reports, 2003-2018 (Red Point)

*Results*
1. Map served to validate Jupyter, Python and Folium for visualizations
2. Tools were appropriate, and functions developed for use in notebook
3. Cluster markers and map options implemented for additional use

*SF Open Data*
* [SFPD Crime Report Data (2003-18)][03.02]

*Tutorials*
1. [Folium Tutorial: SFPD Crime Data][03.01]
2. [Folium Example: Cluster Markers][03.03]
3. [Folium Tutorial: Cluster Markers (JPYTR)][03.04]
4. [Folium Tutorial: Shapefile Data (Medium)][03.05]

### Map 2: SACOG LIHM Communities and Sac Area Schools

![03.02_plot_sac_lihm_school][99.02]

*Map Legend*
1. SACOG LIHM Communities, 2016 (Blue Polygon)
2. CA Schools: Sac County, 2019-20 (Red Point)
3. CA Schools: Amador County, 2019-20 (Green Point)
4. CA Schools: Placer County, 2019-20 (Blue Point)
5. CA Schools: Yolo County, 2019-20 (Orange Point)
6. CA Schools: Yuba County, 2019-20 (Purple Point)

*Results*
1. Map starts with SACOG Low Income High Minority (LIHM) Communities
2. Sacramento area schools were filtered from CA data and added to map
3. Map shows good access to schools within LIHM communities
4. LIHM communities in the north and southeast may have less school access

> Note: Analysis only evaluates proximity and not school quality; also, additional CA Geoportal data are listed below for future analysis.

*SACOG Data*
* [Sac Region LIHM Communities (2016)][05.01]

*CA Geoportal Data*
1. [CA Geoportal: Open Datasets][04.01]
2. [CA School Locations (2019-20)][04.02]
3. [CA Healthcare Shortage (Primary Care)][04.03]
4. [CA Healthcare Shortage (Mental Health)][04.04]
5. [CA Healthcare Shortage (Dental Care)][04.05]

### Map 3: SACOG LIHM Communities and Sac Area Bike Facilities

![03.03_sac_lihm_bike][99.03]

*Map Legend*
1. SACOG LIHM Communities, 2016 (Orange Polygon)
2. City of Sacramento Bike Facilities, 2018 (Green Line)
3. City of Sacramento Bike Opportunity Areas, 2016 (Purple Polygon)

*Results*
1. Map starts with SACOG Low Income High Minority (LIHM) Communities
2. City of Sacramento bike facility data was added to map
3. Map shows good access in downtown and expanding in opportunity areas
4. LIHM communities outside of downtown may have less access to bike facilities

*SACOG Data*
* [Sac Region LIHM Communities (2016)][05.01]

*City of Sacramento Data*
1. [City of Sacramento Bike Facilities (2018)][06.01]
2. [City of Sacramento Bike Opportunity Areas (2016)][06.02]

### Map 4: SACOG LIHM Communities and Public Transit

![03.04_sac_lihm_transit][99.04]

*Map Legend*
1. SACOG LIHM Communities, 2016 (Orange Polygon)
2. Sac Region High Transit Frequency Areas, 2020 (Purple Polygon)
3. Sac Region High Quality Transit, 2017 (Green Line)

*Results*
1. Map starts with SACOG Low Income High Minority (LIHM) Communities
2. SACOG transportation quality data added to map
3. Map shows good access in downtown and along major corridors
4. LIHM communities outside of downtown may have less access to transit

*SACOG Data*
1. [Sac Region LIHM Communities (2016)][05.01]
2. [Sac Region High Transit Frequency Areas (2020)][05.02]
3. [Sac Region High Quality Transit (2017)][05.03]

### Map 5: SACOG LIHM Communities and Pollution Levels

![03.05_sac_lihm_pollution][99.05]

*Map Legend*
1. SACOG LIHM Communities, 2016 (Orange Polygon)
2. SACOG Air Pollution PM 2.5 Planning Areas, 2018 (Purple Polygon)
3. SACOG CalEnviroScreen 3.0, Top 25% Tracts (Green Line)

*Results*
1. Map starts with SACOG Low Income High Minority (LIHM) Communities
2. SACOG pollution level data was added to map
3. Some LIHM communities are within CalEnviroScreen areas
4. Most of Sacramento area is within the PM 2.5 pollution planning area
5. Additional analysis needed to evaluate CalEnviroScreen overlap

*SACOG Data*
1. [Sac Region LIHM Communities (2016)][05.01]
2. [SACOG Air Pollution PM 2.5 Planning Areas, 2018][07.02]
3. [SACOG CalEnviroScreen 3.0, Top 25% Tracts][07.01]

### Jupyter Installation
1. Download and install Jupyter Notebook from their [website][01.01]
2. Verify that Jupyter Notebook was installed and visible from Windows Start menu
3. Start Jupyter Notebook; it will start CMD shell and load in the web browser
4. Save this notebook and CSV data to your "Documents" folder and navigate to it from the Notebook start page
5. Open this notebook from the start page; file and cells should be viewable

### Jupyter Introduction
This notebook will require some basic understanding of the Python programming language, Jupyter platform and data analysis concepts. It is based on this [tutorial][01.02] and [Github Repo][01.03].

Jupyter is a powerful collaborative tool which is open-source and light-weight. It provides all the tools necessary to run data analysis, visualization, statistics and data science [out of the box][01.04]. In addition, it has gain acceptance from industry and academia for collaborating on projects and publishing work.

Jupyter is a combination of text and code with the programming run-time built into the platform so there is no need to install additional software. The text is in the markdown file format (similar to HTML), and code in several languages. It is organized by cells which can consist of either text or code; placed together, they can be sent as a single document to share/publish work.

### Jupyter Notebook
Notebooks are organized by cells, which mainly consist of text (in markdown) and code (Python). It operations like a hybrid between MS Word and Excel file; whereas the entire file is like a document, the cells operate like a spreadsheet. For getting started, feel free to scroll down each cell and navigate around the cells for a quick tour. Here is a breakdown of how to view/edit cells:

*Navigation*
1. Each cell may be edited by hitting ENTER; toggle between cells using the arrow keys or mouse/scroller
2. When editing a cell, be sure to select "markdown" for text or "code" before writing into it
3. Each cell can be run by hitting CTRL + ENTER or the "run" button form the menu bar
4. Output from each cell will appear below; if an error occurs, please read and try to debug it(!)
5. File can be saved by hitting CTRL + "s" or file/save from the pulldown menu above

### Quick Start

*Notes*
1. This notebook will require some Python programming
2. It is widely used and taught in [high school][01.05] and AP Computer Science [courses][01.06]
3. [Jupyter][01.07] supports many other languages, including R, Scala and Julia
4. Python is the most popular of them and can be used for other tasks, primarily data science and web applications

### Exercises

*Jupyter*
1. [Intro Guide (DataQuest)][01.08]
2. [Intro Guide (DataCamp)][01.09]
3. [Notebook Intro (Medium)][01.10]
4. [Data Science Tutorial (Jupyter)][01.11]

*Python*
1. [Quick Start][01.12]
2. [Intro Tutorials][01.13]
3. [Quick Start (FCC)][01.14]

*Markdown*
1. [Quick Start (Github)][01.15]
2. [Quick Start Guide (Markdown)][01.16]
3. [Quick Start Tutorial (Markdown)][01.17]

[01.01]: https://jupyter.org/install
[01.02]: https://medium.com/python-pandemonium/introduction-to-exploratory-data-analysis-in-python-8b6bcb55c190
[01.03]: https://github.com/kadnan/EDA_Python/
[01.04]: https://jupyter.org/jupyter-book/01/what-is-data-science.html
[01.05]: https://codehs.com/info/curriculum/intropython
[01.06]: https://code.org/educate/curriculum/high-school
[01.07]: https://jupyter.org/
[01.08]: https://www.dataquest.io/blog/jupyter-notebook-tutorial/
[01.09]: https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook
[01.10]: https://towardsdatascience.com/a-beginners-tutorial-to-jupyter-notebooks-1b2f8705888a
[01.11]: https://jupyter.org/jupyter-book/01/what-is-data-science.html
[01.12]: https://www.python.org/about/gettingstarted/
[01.13]: https://realpython.com/learning-paths/python3-introduction/
[01.14]: https://guide.freecodecamp.org/python/
[01.15]: https://guides.github.com/features/mastering-markdown/
[01.16]: https://www.markdownguide.org/getting-started/
[01.17]: https://www.markdowntutorial.com/

[02.01]: https://www.codeforamerica.org/events/national-day-of-civic-hacking-2020

[03.01]: https://blog.dominodatalab.com/creating-interactive-crime-maps-with-folium/
[03.02]: https://data.sfgov.org/Public-Safety/Police-Department-Incident-Reports-Historical-2003/tmnf-yvry
[03.03]: https://github.com/python-visualization/folium/blob/master/examples/MarkerCluster.ipynb
[03.04]: https://www.jpytr.com/post/analysinggeographicdatawithfolium/
[03.05]: https://medium.com/@rohanguptha.bompally/python-data-visualization-using-folium-and-geopandas-981857948f02

[04.01]: https://gis.data.ca.gov/
[04.02]: https://gis.data.ca.gov/datasets/CDEGIS::california-schools-2019-20?geometry=-152.476%2C31.022%2C-85.723%2C43.235
[04.03]: https://gis.data.ca.gov/datasets/CHHSAgency::health-professional-shortage-area-primary-care?geometry=-146.864%2C31.069%2C-91.141%2C43.275
[04.04]: https://gis.data.ca.gov/datasets/CHHSAgency::health-professional-shortage-area-mental-health?geometry=-146.864%2C31.049%2C-91.141%2C43.257
[04.05]: https://gis.data.ca.gov/datasets/CHHSAgency::health-professional-shortage-area-dental?geometry=-147.022%2C31.077%2C-91.300%2C43.281

[05.01]: https://data.sacog.org/datasets/d37cca2c798b48b9966b62e4bb1f380d_0
[05.02]: http://data.sacog.org/datasets/high-frequency-transit-area-mtp-scs-2020
[05.03]: http://data.sacog.org/datasets/high-quality-transit-2036?geometry=-123.179%2C38.303%2C-119.697%2C39.053

[06.01]: http://data.cityofsacramento.org/datasets/15f8e048d9ad4442a3e12b6182bcd4f2_1?geometry=-121.899%2C38.464%2C-121.028%2C38.652
[06.02]: http://data.cityofsacramento.org/datasets/8439c4e091a2434aafee1cf888b061f0_0?geometry=-122.330%2C38.373%2C-120.589%2C38.749

[07.01]: http://data.sacog.org/datasets/calenviroscreen-3-0-top-25-tracts?geometry=-123.212%2C38.343%2C-119.729%2C39.093
[07.02]: http://data.sacog.org/datasets/sacramento-pm-2-5-planning-area-

[99.01]: https://github.com/walteryu/code4sac/blob/master/ndoch_2020/images/03.01_sfpd_reports.png
[99.02]: https://github.com/walteryu/code4sac/blob/master/ndoch_2020/images/03.02_plot_sac_lihm_school.png
[99.03]: https://github.com/walteryu/code4sac/blob/master/ndoch_2020/images/03.03_sac_lihm_bike.png
[99.04]: https://github.com/walteryu/code4sac/blob/master/ndoch_2020/images/03.04_sac_lihm_transit.png
[99.05]: https://github.com/walteryu/code4sac/blob/master/ndoch_2020/images/03.05_sac_lihm_pollution.png
[99.06]: https://github.com/walteryu/code4sac/blob/master/ndoch_2020/images/03.06_sac_lihm_choropleth.png
