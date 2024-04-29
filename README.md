# Problem Statement: 

NO2 Emission Factor Estimation from Global Power Plant.

**Abstract:**
1. This study utilizes advanced machine learning techniques to estimate nitrogen dioxide (NO2) emission factors from global power plants, aiding efforts to combat air pollution.
2. It explores the relationship between power plant characteristics and NO2 emissions, highlighting the efficacy of ensemble methods like Random Forest Regression and Gradient Boosting Regression for accurate predictions.
3. The findings provide valuable insights for developing targeted strategies to improve global air quality.

**Methodology:**
1.  Data Acquisition and Preprocessing:
  a) Data Collection: Obtain a global power plant database containing information such as location, capacity, and estimated generation.
  b) Data Cleaning: Handle missing values using mean imputation for relevant columns like capacity and estimated generation.
  c) Exploratory Data Analysis (EDA): Visualize the distribution of power plants across countries using bar plots and geographical maps to understand geographical patterns.

2. Emission Factor Estimation:
  a) Overall Estimated Generation Calculation: Sum the estimated generation for each power plant from 2013 to 2017 to calculate the overall estimated generation.
  b) Regression Modelling:
    i. Linear Regression
   ii. Random Forest Regression
  iii. Gradient Boosting Regression
   iv. Decision Tree Regression
   
3. Emission Factor Calculation:
  a) Emission Factor Derivation: Calculate the emission factor by dividing the total overall estimated generation by the total capacity of power plants.
  b) Cluster Analysis:
    i. Feature Selection
   ii. KMeans Clustering
  iii. Emission Factor Calculation per Cluster

4. Evaluation and Comparison:
  a) Model Evaluation: Assess the performance of regression models using metrics like mean squared error, mean absolute error, and R-squared score.
  b) Emission Factor Comparison: Compare emission factor values obtained from different regression algorithms and clustering, plotting them on a horizontal bar plot for better visualization.

5. Filtering Power Plants by Country:
  For India and the United Kingdom (UK):
  a) Filter power plants located in India and the UK from the dataset.
  b) Visualizing Power Plants on Maps:
     i. Create a map centered around India and the UK using Folium.
    ii. Add markers for each power plant in India and the UK on the map.
  c) Calculating Emission Factors:
    i. Calculate the overall estimated generation for each country's power plants by summing the estimated generation for each year.
   ii. Calculate the total emissions and total capacity of power plants.
  iii. Calculate the emission factor for power plants by dividing total emissions by total capacity.

**Result Analysis:**
1. Global NO2 Emission Factors Analysis:
  a) Our study aimed to estimate NO2 emission factors for global power plants using data from 2013 to 2017, employing regression models and KMeans clustering.

2. India vs. UK Disparities:
   a) Significant differences were found between India and the UK.
   b) Indian power plants showed lower emission factors (8.88 GWh/MW) compared to the UK (20.78 GWh/MW), indicating potential variations in emission control measures and operational practices.

3. Methodological Impact:
  a) Methodology greatly influenced NO2 emission factor estimations. While baseline calculations yielded 10.22 GWh/MW, machine learning techniques generated diverse results.
  b) Linear regression produced exceptionally high estimates (1672.75 GWh/MW), while random forest regression offered lower values (2.08 GWh/MW).
  c) Decision tree regression fell within the high estimate range (1727.26 GWh/MW), emphasizing method sensitivity.

4. KMeans Clustering Impact:
KMeans clustering identified two clusters, with slight variations in emission factors (Cluster 1: 10.51 GWh/MW, Cluster 2: 9.00 GWh/MW). An anomaly was noted where a duplicate cluster displayed a significantly higher emission factor (21.22 GWh/MW), highlighting the need for rigorous validation.

5. Implications:
  a) These findings underline the variability in NO2 emission factor estimations and stress the importance of methodological rigor in such analyses.
  b) Policymakers must consider these insights to address air pollution effectively and promote sustainable energy practices globally.

**Conclusion:**
1. The utilization of various machine learning algorithms offers a comprehensive approach to estimating NO2 emission factors from power plants.
2. While linear regression provides simplicity, ensemble methods like Random Forest Regression and Gradient Boosting Regression excel in capturing complex interactions, improving global air quality efforts.
3. Addressing regional disparities in emissions underscores the need for tailored solutions, including stringent standards, cleaner energy promotion, and international collaboration to safeguard environmental integrity and public health.

**References:**
[1] Concept of small satellite UV/visible imaging spectrometer optimized for tropospheric NO2 measurements in air quality monitoring: A Study by Tamaki Fujinawa,  Katsuyuki Noguchi, Akihiko Kuze, Andreas Richter, John P. Burrows, Andreas C. Meier, Tomohiro O. Sato, Takeshi Kuroda, Naohiro Yoshida, and Yasko Kasai, 15 May 2019. 

[2] Tracking NO2 Emission from Thermal Power Plants in North India Using TROPOMI Data: A Study by Gautam Kumar Saw, Sagnik Dey, Hemant Kaushal, and Kanhaiya Lal, 4 May 2021. 

[3] First Concurrent Observations of NO2 and CO2 From Power Plant Plumes by Airborne Remote Sensing: A Study by Tamaki Fujinawa, Akihiko Kuze, Hiroshi Suto, Kei Shiomi, Yugo Kanaya, Takahiro Kawashima, Fumie Kataoka, Shigetaka Mori, Henk Eskes, and Hiroshi Tanimoto, 20 July 2021. 

[4] Quantifying CO2 Emissions of Power Plants With CO2 and NO2 Imaging Satellites: A Study Published in Frontiers in Remote Sensing, Section: Satellite Missions, Volume 2 - 2021. Authors: Gerrit Kuhlmann, Stephen Henne, Yashika Meijer, and Dominik Brunner, July 2021. 

[5] Evaluating Machine Learning and Remote Sensing Techniques for Monitoring NO2 Emissions from Power Plants: A Study Published in MDPI 'Remote Sensing' Journal, February 2022, Volume 14, Issue 3, Page 729. DOI: 10.3390/rs14030729. Authors: Ahmed Alnaim, Ziheng Sun, Daniel Tong. Licensed under CC BY 4.0, February 2022. 

[6] https://www.kaggle.com/code/meenakshiramaswamy/ds4g-eie-no2emission-calcef-buildmodel/notebook 

[7] https://www.kaggle.com/code/maxlenormand/simplified-emission-for-each-plant-update-1?scriptVersionId=29240464 

[8] https://naei.beis.gov.uk/resources/3_9_324_136262_primary_no2_emission_factors_for_aviation_and_other_transport_sources_2010naei_v1.pdf 

[9] https://egusphere.copernicus.org/preprints/2023/egusphere-2023-1024/egusphere-2023-1024-manuscript-version2.pdf 

[10] https://naei.beis.gov.uk/resources/Primary_NO2_Emission_Factors_for_Road_Vehicles_NAEI_Base%202022_v1.pdf 
