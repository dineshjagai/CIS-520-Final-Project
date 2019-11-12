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
1. **Motivation** (adapted from [DengAI](https://www.drivendata.org/competitions/44/dengai-predicting-disease-spread/page/80/)) 
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
            -  PERSIANN [satellite precipitation measurements](https://www.ncdc.noaa.gov/cdr) (0.25x0.25 degree scale) <br> 
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

2. **Related Work**
     - 01) https://ieeexplore.ieee.org/abstract/document/7912315 (This papers discusses disease Prediction by Machine Learning Over Big Data From Healthcare Communities using a CNN-based multimodal disease risk prediction )   <br>
     - 02) https://bmcinfectdis.biomedcentral.com/articles/10.1186/s12879-019-3874-x (This paper discusses how to predict dengue outbreaks based on disease surveillance, meteorological and socio-economic data - it uses a Quasi-Poisson regression in which the variance of count data (dengue counts) is assumed to be a linear function of the mean for to predict the dengue cases)  <br>
     - 03) https://towardsdatascience.com/dengue-fever-and-how-to-predict-it-a32eab1dbb18 (An article highlighting how to predict dengue using different regression methods (fairly similar to what we're trying to do, but ours has more parameters and data. Also we plan to use deep learning in addition to regression)  <br>
     - 04) https://pdfs.semanticscholar.org/1c31/0e22fe1a0418aaa25fcc629736b5a46655f8.pdf (This paper looks at developing a Dengue Possibility Forecasting Model using Machine Learning Algorithms. Specifically, they use a Gradient Boosting Regression ensemble method to predict the possibility of a dengue outbreak taking place)  <br>
     - 05) https://journals.plos.org/plosntds/article?id=10.1371/journal.pntd.0005973 (This paper examines predicting the number of dengue cases in China using several ML techniques including the support vector regression (SVR) algorithm, step-down linear regression model, gradient boosted regression tree algorithm (GBM), negative binomial regression model (NBM), least absolute shrinkage and selection operator (LASSO) linear regression model and generalized additive model (GAM), were used as candidate models to predict dengue incidence) They found that the (support vector regression) SVR model achieved a superior performance in comparison with other forecasting techniques assessed in this study.  <br>
     - 06) http://www.imedpub.com/conference-abstracts-files/deep-learning-applications-for-predicting-dengue-fever.pdf (This paper looks at using deep learnging to predict the number of dengue cases in Taiwan.  <br>
     - 07) https://www.researchgate.net/profile/Yuhanis_Yusof/publication/272912479_Dengue_Outbreak_Prediction_A_Least_Squares_Support_Vector_Machines_Approach/links/5691be4f08ae0f920dcb9058/Dengue-Outbreak-Prediction-A-Least-Squares-Support-Vector-Machines-Approach.pdf (This paper develops a dengue prediction model using Long Short Term Memory neural networks)  <br>
     - 08) https://www.biorxiv.org/content/biorxiv/early/2019/09/06/760702.full.pdf (This paper uses Least Squares Support Vector Machines (LS-SVM) in predicting future dengue outbreaks in Malaysia) <br>
     
     

3. **Problem Formulation**
     - Predit the number of degue cases each week in San Juan and Iquitos over a five year period (2008 - 2013) using 
    given environmental variables describing changes in temperature, precipitation, vegetation, and more from 1990.<br>

4. **Methods**
     - Used an imputation method to clean the data  <br>
     - Use simple regression methods to pedict the number of cases based on our 22 features <br>
     - Use deep learning with neural networks for a more robust approach. <br>

5. **Evaluation**
  - Performance is evaluated according to the mean absolute error. <br>
    ![MAE](https://github.com/dineshjagai/CIS-520-Final-Project/blob/master/Tex2Img_1573418695.jpg)
  
6. **Project Plan**
   - **Week 1 11/4** <br>
          - Clean the data  <br>
          - Impute the missing data <br>
          - Visualize the data <br>    
   - **Week 2 11/11** <br>
          - Work on mimimizing the loss on the training set using different regression methods <br>
    
   - **Week 3 11/18** <br>
           - Work on minimizing the loss on the test set using different regression methods <br>
   - **Week 4 11/25** <br>
           - Use a Neural Network (deep learning) <br>
   - **Week 5 12/2** <br>
            - Work on Presentation <br>



