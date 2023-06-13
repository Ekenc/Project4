# Predicting Changes in Glaciers Mass And Sea Level

## Project Description

Train supervised machine learning models to read historical data of glacier size, sea levels, global temperature, and greenhouse gases, including carbon dioxide, methane, and nitrous oxide concentration levels, to predict the possible future of glaciers and sea levels.

**Research Question:**

How is the change in global average temperature affecting average glacier mass and sea level change? What changes can be predicted for the near future based on historical data?

Does change of greenhouse gas emissions in the Earth’s atmosphere affect average glacier mass and sea level change? 


## Getting Started
### Prerequisites

*Before you begin, please ensure you have the following requirements:*
1. Internet connection
2. Compatible web browser such as Google Chrome, Microsoft Edge, Mozilla Firefox, or Safari

**The platforms used (Google Colab and Tableau Public) are web-based, therefore this project does not require cloning of the git repository.**

### Instructions

**Google Colab Notebooks**
1. Open Google Colab in your preferred browser by following this link: [Google Colab](https://colab.research.google.com/)
2. Click on "GitHub" on the top menu
3. Enter the following onto the search line: Ekenc/Project4
4. From the "Repository" dropdown menu choose Ekenc/Project4
5. You can now choose which notebook to view
- Simply click on the name of the notebook OR to open more than one see the next step
- Click on the icon to the far right of the file to "Open notebook in new tab". This will allow you to return to the list of files so   that you may open several files at once in separate tabs.  
6. To run the notebook click on "Runtime" from the top menu bar, then "Run all"
 
**Tableau Public Dashboard**
1. The pdf version of the dashboard is located in the "TableauDashboard" folder as "dash.pdf" or can be accessed by following this link: [Dashboard pdf](https://github.com/Ekenc/Project4/assets/119901186/2d3cbeb3-6482-4691-a312-5e32dc30c79f)
2. The interactive dashboard can be viewed by following this link: [Dashboard](https://public.tableau.com/app/profile/ellie.culverhouse/viz/PredictingChangesinGlacierMassandSeaLevel/Dashboard1)
3. The map can be viewed by following this link: [World Glaciers & Ice Caps Map](https://public.tableau.com/app/profile/ellie.culverhouse/viz/worldglaciersmap/Dashboard1)

## Project Overview

### 1. Data
Our data was collected from the US Environmental Protection Agency’s Climate Change Indicators.
We selected data that was prima facie related to glacier melt and sea level change
- The atmospheric concentration of the three major greenhouse gases (carbon dioxide, methane, nitrous oxide)
- The annual precipitation anomaly, based on the 1901-2000 average
- The temperature anomalies of the Earth’s surface and the sea surface, based on the 1901-2000 and the 1971-2000 averages, respectively

**Data and Notebook Guide** [Data Guide](https://github.com/Ekenc/Project4/blob/main/Data_Guide_For_Notebooks_CSVs.pdf)


### 2. ML Model
We ran two types of models for this project, a random forest regression and a linear regression model. While both have their own pros and cons for this data we thought the linear regression model was able to perform better for our datasets.

Linear Regression Model:
This model projected well continuing a Strong Linear Relationship all the way through 2050 showing Glaciers lose over 10 more cumulative mass balance & Sea Level rising almost 3 more inches in that span.

**Model notebooks are located in the "Modeling" folder**

We Used Pandas to create visualizations that showed comparisons between the linear regression model and the random forest regression model.

Linear Regression Model:

![Glacier_Linear](https://github.com/Ekenc/Project4/assets/119901186/ebbca2c5-2a24-4be8-a0b8-135df75768ad)
![Sea_Level_ LinearPNG](https://github.com/Ekenc/Project4/assets/119901186/81170b32-eb7f-4274-bbd3-f89e070f5193)

Random Forest Regression Model:

![Glacier_RFR](https://github.com/Ekenc/Project4/assets/119901186/0c591e92-4f48-45c8-8f75-4dc2114d0bc8)
![Sea_Level_RFR](https://github.com/Ekenc/Project4/assets/119901186/504bcc74-4597-4c79-a0a9-e0e675759df9)

### 3. Visualizations
We used Tableau Public to generate a dashbaord to organize our data outcomes in a more visually pleasing way for our audience. While the Tableau Public workbooks are in this repository to view them more easily, links to the publihsed dashboards will be provided by the corresponding visualization.

The Dahsboard:

![dashboard](https://github.com/Ekenc/Project4/assets/119901186/2d3cbeb3-6482-4691-a312-5e32dc30c79f)

https://public.tableau.com/app/profile/ellie.culverhouse/viz/PredictingChangesinGlacierMassandSeaLevel/Dashboard1

World Glaciers & Ice Caps Map:

<img width="955" alt="worldglaciers" src="https://github.com/Ekenc/Project4/assets/119901186/8958f8e5-4327-4d7a-8cd1-0e1457ff2a1e">


Due to the large size of the file it made more sense to run the map on a seperate Tableau workbook then import it onto the main dashboard as a pdf file. Another complication of the file size was being unable to push a file of it's size to GitHub. The data for the shapefiles was pulled from the National Snow and Ice Data Center and directly sourced in our credits below.
https://public.tableau.com/app/profile/ellie.culverhouse/viz/worldglaciersmap/Dashboard1

### 4. Conclusion
We were successful in creating a model with a high accuracy in the prediction of future data

From results from our model & statistical analysis:
- Greenhouse gasses concentration increase does have correlation in the decrease in average glacier mass and increase in sea level
- Global average temperature change does have correlation in the decrease in average glacier mass and increase in sea level



## Sources and Credits
GLIMS Consortium, 2005. GLIMS Glacier Database, Version 1. Boulder Colorado, USA.  NASA National Snow and Ice Data Center Distributed Active Archive Center.  DOI: https://doi.org/10.7265/N5V98602  [6/23].
Environmental Protection Agency. (n.d.). EPA. https://www.epa.gov/ 
USGS.gov | Science for a changing world. (2023, June 11). https://www.usgs.gov/
https://nsidc.org/data/nsidc-0272/versions/1 : map files source since too large to commit
