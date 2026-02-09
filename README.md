# assignment_vanshika_102303735_11feb


Data Generation using Simulation for Machine Learning

Overview

This project focuses on generating synthetic data using modelling and simulation and applying machine learning techniques on the generated data. A discrete event simulation is developed using Python to model a single-server queue system. The generated data is then used to train and compare multiple machine learning models. The entire implementation is done using Google Colab.


Simulation Tool

SimPy was used as the simulation tool. It is a Python-based discrete event simulation framework that allows modelling of systems involving queues, resources, and events. It was chosen because it is lightweight, easy to use, and suitable for modelling real-world queueing systems.


Problem Description

A single-server queue system is simulated where customers arrive randomly and wait to be served by a single server. The aim is to study how different system parameters affect the average waiting time and to predict this waiting time using machine learning models.


Simulation Parameters

The following parameters were randomly generated within defined bounds:

Parameter	Description	Range
Arrival Rate	Rate of customer arrival	0.5 – 5
Service Rate	Speed of service	1 – 6
Simulation Time	Total simulation duration	50 – 200

Data Generation

For each simulation run, random values of arrival rate, service rate, and simulation time were generated. The simulation was executed and the average waiting time was recorded. This process was repeated 1000 times to generate a dataset for machine learning.


Machine Learning Models

The generated dataset was used to train and evaluate the following regression models:

Linear Regression
Ridge Regression
Decision Tree Regressor
Random Forest Regressor
Gradient Boosting Regressor

Evaluation Metrics

Model performance was evaluated using:
Mean Absolute Error (MAE)
Root Mean Squared Error (RMSE)
R² Score
The models were compared using a results table and a bar graph.


Results

Tree-based models performed better than linear models, as they were able to capture non-linear relationships between the input parameters and the average waiting time. The best model was selected based on the lowest RMSE and highest R² score.


Conclusion

This assignment demonstrates that simulation can be effectively used to generate data when real-world data is unavailable. The generated data was successfully used to train multiple machine learning models, and meaningful performance comparisons were obtained.



Tools Used

Python
SimPy
NumPy
Pandas
Scikit-learn
Matplotlib
Google Colab














