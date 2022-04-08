# Kalman-filter

This repository hosts code available on Google Colab developed for **Copernicus Marine Services For Energy Optimized Cargo Ship Routing**.
Code works along the following steps:
* Loads csv file which contains AIS data for specific ship
* Preprocess csv file and prepare vectors with data for Kalman filter
* Run Kalman filter 
* Plot vessel's positions from raw data and
* Plot vessel's positions as calculated by Kalman filter
* Plot x and y axis differences between raw and Kalman filtered positions

It is important to note that Kalman filter can work as smoothener or predictor. In our case, we used it as predictor. Points are available for the whole vessel trajectory but input into Kalman filter is only first 20 points, after that Kalman filter makes predictions which then can be compared to the raw "real" positions. As visible on the image, 
