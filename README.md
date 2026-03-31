# Project-3

---
## This includes files for Project no. 2:
- [Gantt Chart](https://github.com/Aperrotto/Project-3/blob/main/CIVE%20202%20Project%203%20Final%20Gantt%20Chart.pdf)
- [Timesheet](https://github.com/Aperrotto/Project-3/blob/main/CIVE%20202%20Project%203%20Final%20Timesheet.pdf)
- [Scope of Work]()
- [Annotated Code Document](https://github.com/Aperrotto/Project-3/blob/main/Project%20%233%20ACD.pdf)
- [Written Report](https://github.com/Aperrotto/Project-3/blob/main/CIVE%20202%20Project%203%20Report.pdf)

---
## Overview
- We analysed data from NHTS and NGSIM for the Federal Highway Administration. The goal of this project is to organize the data, create clear graphs using python, and complete a driving simulation using IDM. We tracked the time we spent on each task so our company can compare Python's effiecency with Excel. 

## Project Tasks: 

### 1. Create visualizations of features and trends in the data
- Bar chart
- histogram
- boxplot
- 2 time series plots showing driving behavior

### 2.  Provide Simulation study using IDM
- select specific trajectory  and simulate the follower
- simulate acceleration of folllower and plot it

### 3. Document time spent on project
- create and fill out timesheet

 
## Methods
### Variables Selected and Data Retrieval 
- aquired data on vehicle characteristics by the use of variables using the NHTS database
- Use different variables: vehicle type, household income, number of vehicle in household
- retrieve data from the NGSIM database for variables: speed, acceleration, time, position
- analyse traffic flow and vehicle behavior

### Processing Data
- data from both NHTS and NGSIM were processed in python using the pandas package
- we reduced the data to only complete trajectory histories
- we plotted the data in speed vs time and position vs time charts
- we used rolling averages to reduce datat noise and indentify the trends
- We customized the graphs to make them easier to read and understand

### Intelligent Driver Model
- we preformed the simulations and observed the data
- we assessed the simulated and observed measurements against the performance measuure statistics

## Results and Analysis
### NHTS Analysis
- we found that SUVs and Pickup Trucks were the predominant vehicles using the bar graph
- the histogram shows that the majority of the dataset exist in the middle-income range
- the boxplot shows that median values are relatively uniform amon regions but factors sucha as proximity to other forms of transportation can affect the level of vehicle ownership
  
### NGSIM Analysis
- we found a higher correlation for the speed of the lead vehicle with the following vehicle
- both vehicles demonstrate continuous fluctuation showing dynamic traffic conditions
- the trajectory shows the average gap between 2 vehicles is approximately 23.6 meters

### IDM Sim results
- the simulated follower speed and position values were nearly identical to observed follower data
- the correlation between the simulated and observed follower speed was approximately .95
- Overall speed RMSE values were approximately 1.22 for speed and 9.82 for position
- The IDM's car acceleration correlation was only .22, so it doesn't accurately depict short term changes in acceleration.

  
## Using The Code: 
