# Major-Projects Linked from Google Drive (Python, R and HTML file types)
Tobago Weather Data (HTML): https://drive.google.com/file/d/17aMF8x_WWA-w6jTtqXt2q3aiZV3biOQf/view?usp=drive_link

Tobago Weather Data (Python): https://drive.google.com/file/d/1msDizEbuRmQmgs8dcAjzW5GDzk-hbtQC/view?usp=drive_link

NYC Harbour Water Quality Analysis (HTML): https://docs.google.com/document/d/1K9HOp7DsfeKgfGq1i8CXbouI9fAyM7H0AXWpA6qPoNI/edit?usp=drive_link

NYC Harbour Water Quality Analysis (Python): https://drive.google.com/file/d/1VI-hy4fveINL6o9p-xKilBmj56kPSi5p/view?usp=drive_link

# Hi, I'm Le' Sean Roberts | Data Wrangling & Statistical Programming Specialist

I specialize in building transparent data models and optimizing data extraction processes. 
My work focuses on bridging the gap between raw system data and actionable agency insights.

### 🔍 Technical Focus
* **Data Integrity:** Designing reliability checks and anomaly detection protocols. PyOD use. 
* **Data Wrangling:** From Data Asimilation (APIs, Databases, etc.) to data cleaning to feature engineering. Tidyverse and Pandas. DBI + dbplyr. Sparklyr. SQLAlchemy, PySpark. 
* **Statistical Programming:** Exploratory data analysis, unsupervised learing, feature importance/selection, supervised learning, ensemble learning and time series (analysis, modelling, forecasting)
* **Visualization:** ggplot2, Matplotlib, Seaborn, Folium, GeoPandas. Self sufficient and high level exhibitions. Tableau basics. 
* **Documentation:** Crafting technical requirements and data definitions for scalable systems.

### 🛠️ Tool Stack
* **Languages:** Python and R. Subjugating SQL environments with Python or R.
* **API/Integration:** RESTful APIs, JSON, Caching strategies
* **DevOps/Tools:** GitHub Actions


## ⚠️ Caveat 1

For the files `Traffic Reasearch.html` and `Traffic Research.ipynb` currently contain an issue that needs to be amended.  
Specifically: Concerning the attempted 'causal' scheme between vehicle collisions-crashed and anomalies detected from traffic data, I possibly should have further constructed/incorporated an additional condition...being, used the crashed coordinates and set condition for locations close and "infront" or "behind" facility 30. Hence, share percentage is likely lower. Also keep in mind that this type of vehicular collision (crashes) isn't encompassing of all types of crashes. As well, other possibilities for anomalies still reside.  This will be corrected in a future update (if attempted).


## ⚠️ Caveat 2

For the files `OEWS.html` and `OEWS.qmd`, in the **General Attributes Analysis** section there **may** be a typo concerning interpretation of the following:

results <- compare_binary_nonparam(data = OEWS_for_modelling, group = "area_type", var_names = num_vars)

print(results)

**Details:** *specifically "Group 2 has significantly higher employment (Median approximately 11,880) compared to Group 1 (Median approximately 404)*". My eyes seemingly were elsewhere while typing. Personally interpret and draw your own conclusions. 


## ⚠️ Caveat 3

For the TREK WITH METEOROLOGICAL AND CLIMATE DATA Projects....

Zero-Inflated Data: For variables like rain_sum or snowfall_sum, the 95th percentile can sometimes be $0$ if the region is very arid or in a non-snowy month. This would result in every day being flagged as "extreme." You may want to filter for days where value > 0 before calculating the quantile.

Inclusive Boundaries: Using >= and <= is standard, but in very small datasets, high quantiles might flag a large number of ties.

AS WELL, for places with temperature climate, choose those places that are consistent with snowfall to avoid sustainability issues with HMMs. 
