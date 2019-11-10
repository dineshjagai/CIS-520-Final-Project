# CIS520 FINAL PROJECT! 
![Dengue Vector](https://github.com/dineshjagai/CIS-520-Final-Project/blob/master/0f3a28954438c90e1935d61f3f2c23e906feb39a.jpg)

# Team-members 
  - Dinesh Jagai <dinesh97@seas.upenn.edu>
  - Pranav Panganamamula <ppranav@seas.upenn.edu>
  - Julian P. Schnitzler <schnitzl@seas.upenn.edu>

# Project Title
> Predicting the spread of dengue virus in San Juan and Iquitos over a five year period 



# Goal
> To predict the number of dengue cases each week (in each location) based on environmental variables describing changes in temperature, precipitation, vegetation, and more.

[PROJECT DESCRIPTION](https://www.drivendata.org/competitions/44/dengai-predicting-disease-spread/page/82/)

# Objectives
1. Motivation (adapted from [DengAI](https://www.drivendata.org/competitions/44/dengai-predicting-disease-spread/page/80/)) 
- Dengue fever is a mosquito-borne disease that occurs in tropical and sub-tropical parts of the world. In mild cases, symptoms are similar to the flu: fever, rash, and muscle and joint pain. In severe cases, dengue fever can cause severe bleeding, low blood pressure, and even death. 
 - Because it is carried by mosquitoes, the transmission dynamics of dengue are related to climate variables such as temperature and precipitation. Although the relationship to climate is complex, a growing number of scientists argue that climate change is likely to produce distributional shifts that will have significant public health implications worldwide.
 - In recent years dengue fever has been spreading. Historically, the disease has been most prevalent in Southeast Asia and the Pacific islands. These days many of the nearly half billion cases per year are occurring in Latin America. 
 - Our goal is to predict the number of dengue cases each week (in each location) based on environmental variables describing changes in temperature, precipitation, vegetation, and more.
 - **DATASET** 
      - **Sets of features(N = 1456, p = 22)** <br> 
            - City and date indicators <br> 
            _city_ – City abbreviations: sj for San Juan and iq for Iquitos <br> 
             _week_start_date_ – Date given in yyyy-mm-dd format <br> 
            - NOAA's [GHCN daily climate data weather station measurements](https://www.ncdc.noaa.gov/oa/climate/ghcn-daily.html) <br>
                _station_max_temp_c_ – Maximum temperature <br> 
                _station_min_temp_c_ – Minimum temperature <br> 
                _station_avg_temp_c_ – Average temperature <br> 
                _station_precip_mm_ – Total precipitation <br> 
                _station_diur_temp_rng_c_ – Diurnal temperature range <br> 
            -  PERSIANN [satellite precipitation measurements]https://www.ncdc.noaa.gov/cdr) (0.25x0.25 degree scale) <br> 
             _precipitation_amt_mm_ – Total precipitation <br> 
             - NOAA's [NCEP Climate Forecast System Reanalysis measurement](https://rda.ucar.edu/datasets/ds093.0/#metadata/detailed.html?_do=y)  (0.5x0.5 degree scale)  <br> 
                _reanalysis_sat_precip_amt_mm_ – Total precipitation <br> 
                _reanalysis_dew_point_temp_k_ – Mean dew point temperature <br> 
                _reanalysis_air_temp_k_ – Mean air temperature <br> 
                _reanalysis_relative_humidity_percent_ – Mean relative humidity <br> 
                _reanalysis_specific_humidity_g_per_kg_ – Mean specific humidity <br> 
                _reanalysis_precip_amt_kg_per_m2_ – Total precipitation <br> 
                _reanalysis_max_air_temp_k_ – Maximum air temperature <br> 
                _reanalysis_min_air_temp_k_ – Minimum air temperature <br> 
                _reanalysis_avg_temp_k_ – Average air temperature <br> 
                _reanalysis_tdtr_k_ – Diurnal temperature range <br> 
            - Satellite vegetation - Normalized difference vegetation index (NDVI) - NOAA's [CDR Normalized Difference Vegetation Index](https://www.ncdc.noaa.gov/cdr) (0.5x0.5 degree scale) measurements <br>
                _ndvi_se_ – Pixel southeast of city centroid <br> 
                _ndvi_sw_ – Pixel southwest of city centroid <br> 
                _ndvi_ne_ – Pixel northeast of city centroid <br> 
                _ndvi_nw_ – Pixel northwest of city centroid <br>

2. Related Work

3. Problem Formulation
     - Predit the number of degue cases each week in San Juan and Iquitos over a five year period (2008 - 2013) using 
    given environmental variables describing changes in temperature, precipitation, vegetation, and more from 1990.<br>

4. Methods 
     - Used an imputation method to clean the data  <br>
     - Use simple regression methods to pedict the number of cases based on our 22 features <br>
     - Use deep learning with neural networks for a more robust approach. <br>

5. Evaluation
  - Performance is evaluated according to the mean absolute error. <br>
    ![MAE](https://github.com/dineshjagai/CIS-520-Final-Project/blob/master/Tex2Img_1573418695.jpg)
  
6. Project Plan
   - **Week 1**
          - Clean the data  <br>
          - Impute the missing data <br>
          - Visualize the data <br>    
   - **Week 2**
          - Work on mimimizing the loss on the training set using different regression methods <br>
    
   - **Week 3**
           - Work on minimizing the loss on the test set using differnt regression methods <br>
   - **Week 4**
           - Use a Neural Network (deep learning) <br>
   - **Week 5**
            - Work on Presentation <br>



