# Dubai_UG_3
F21DL Coursework AY 2024-25

## Group Name:
 Undergraduate  Group 13
## Project Title: 

 Predicting and Analyzing damage from hurricanes and typoons

## Group Members 
•	Joseph Abdo

•	Joe Ettumanookaran

•	Lubna Gulnar

•	Thomson Thomas 

•	Irin Varughese



## Project Milestones and the Timeline

### Weeks 1–2: Research and Project Selection
•	Explore various applications for the project before deciding on a suitable application that met all assessment criteria.

•	The topic chosen was Predicting and analyzing damage from hurricanes and typoons.

•	Finalized two datasets from Kaggle: a numerical dataset for hurricane parameters and an image dataset with satellite visuals of hurricane damage.

•	Defined the project goals and scope.

### Weeks 3–4: Understanding the dataset, Preprocessing, and Initial Analysis

#### Numerical DataSet:

•	Explore the structure of the dataset and identify relevant features.

•	Performed preprocessing steps like handling missing values and normalizing data.

•	Conducted exploratory data analysis (EDA) using scatter plots and histograms

####	Image Dataset:
•	Resize images and adjust color channels to highlight features relevant to storm damage.

•	Utilize MATLAB colormaps to enhance image visualization.

####	Deliverable 1:

•	Created and presented the Project Pitch which outlined the goals, datasets, and initial insights.

### Weeks 5–10: Model Development and Evaluation
#### 	Model Training:
Trained multiple machine learning models on the preprocessed numerical dataset, including:

•	Naïve Bayes

•	Clustering algorithms

•	Decision Trees

•	Linear and Logistic Regression

•	K-Nearest Neighbors (KNN)

and trained CNN on the preprocessed image dataset

#### 	Evaluation:
Assessed model performance using metrics like Accuracy, Precision, Recall, F1-Score, and RMSE.

### Week 11: Documentation and Repository Finalization
•	Compiled the Project Report, summarizing all findings, methodologies, results and visualization 

•	Organized the GitHub repository for submission, ensuring all files, scripts, and documentation were clearly structured and accessible.

### Week 12: Preparation for Final Deliverable 
•	Prepare the final presentation, highlighting the key results, methodologies, and learnings from the project.

•	Deliver the final presentation to showcase the outcomes and potential applications of the project



## Source of the datasets

#### numerical dataset
The numerical dataset is sourced from the HURDAT (HURricane DATabase), published by the National Hurricane Center (NHC). It includes detailed information on various hurricanes across the Atlantic and Pacific basins, such as location, date, time, maximum wind speeds, minimum pressure, and more.

The license of the numerical dataset is: https://creativecommons.org/publicdomain/zero/1.0/

#### image dataset

The image dataset consists of satellite images depicting areas in Texas affected by Hurricane Harvey. It is categorized into two groups: images of areas with damage and those with no damage. The Data is originally sourced from:  
https://ieee-dataport.org/open-access/detecting-damaged-buildings-post-hurricane-satellite-imagery-based-customized

The license of the numerical dataset: https://creativecommons.org/licenses/by/4.0/

### examples from numerical dataset
#### Example 1
•	Feature: Maximum Wind 

•	Value: 110 knots

•	Description: This represents the peak wind speed recorded in the Atlantic basin during Hurricane JOAQUIN. The high wind speed indicates extreme storm intensity.

#### Example 2
•	Feature: Minimum Pressure

•	Value: 995 hPa

•	Description: This corresponds to the central pressure recorded during Hurricane Beatriz  in the pacific basin. Pressure is used as a key factor in assessing storm strength.


### examples from image dataset
#### Example 1
Image Description: A satellite image showing the damage to infrastructure caused during Hurricane Harvey.
#### Example 2
Image Description: A satellite image taken in the after math of Hurricane Harvey showing infrastructure with no viable damage 
## The steps included in data preparation

#### 1) Setting up the environment
#### 2) Loading the Data:
 CSVs for numerical datasets, image files for visual data
#### 3) Cleaning the Data
Handling missing values, removing duplicate records, standardizing data formats etc
#### 4) Preprocessing the data
For numerical data: Scaling or normalizing values

For image data: Resizing images to a uniform size, Using colormaps

#### 5) Exploratory Data Analysis (EDA)
Visualizing the data to understand patterns, correlations, and distributions.

For numerical datasets: creating scatter plots, histograms etc.

For image datasets: visualizing sample images to verify preprocessing.

#### 6) Saving the Processed Data

### To excecute the data preparation pipeline:
1) Clone the repository

2) Install dependencies 

3) Run the pipeline: Navigate to the root directory of the repository and run the pipeline using the command: python run_pipeline.py



