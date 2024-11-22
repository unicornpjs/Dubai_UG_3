# Dubai_UG_3
F21DL Coursework AY 2024-25

## Group Name:
 Undergraduate  Group 03
## Project Title: 

 Predicting and Analyzing damage from hurricanes and typoons

## Group Members 
•	Joseph Abdo

•	Joepaul Ettumanookaran

•	Lubna Gulnaar

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




## Data Analysis and Exploration

The numerical dataset was loaded as a .CSV file and analyzed using methods like .info(), .describe(), and .shape() to understand its structure, data types, and statistics, including value ranges and missing data. Rows with missing values were removed to ensure data completeness. A scatter plot of "Maximum Wind vs. Minimum Pressure" was created to understand how the two parameters affect each other. The image dataset, consisting of .jpeg files, was preprocessed for machine learning by normalizing and reshaping the images to maintain consistent sizes. 

Data Analysis and Exploration can be found at: https://github.com/unicornpjs/Dubai_UG_3/blob/396568d47bd44f4e158443a822d19324b07d8ee3/Notebooks/Data%20PreProcessing%20and%20Analysis/Preprocessing1.ipynb

## The K-means clustering 

The K-means clustering algorithm was applied to hurricane data, using features like wind speed and pressure, to identify patterns for categorizing hurricanes into categories like tropical storm and no hurricane. The Atlantic and Pacific datasets were merged, with non-numeric columns and missing values removed to ensure data integrity. Features were standardized using "StandardScaler" before applying K-means with three clusters (k=3). Additionally, K-means was used on the image dataset with two clusters (k=2) for segmentation, helping group regions of the images to enhance image analysis.

The K-means clustering can be found at: https://github.com/unicornpjs/Dubai_UG_3/blob/396568d47bd44f4e158443a822d19324b07d8ee3/Notebooks/Clustering/UG3_kmeans_clustering.ipynb

## Baseline Training and Evaluation Experiments

A Decision Tree Classifier was used to classify hurricanes as either Atlantic or Pacific, and predict the hurricane type and location based on wind and pressure. 

The Gaussian Naive Bayes (GNB) algorithm was also applied to classify the data into Atlantic and Pacific categories, evaluating its accuracy and ability to identify mislabeled points under different data split ratios.

 The K-Nearest Neighbors (KNN) algorithm was used for the same classification task.

 the Baseline Training and Evaluation Experiments can be found at: https://github.com/unicornpjs/Dubai_UG_3/blob/main/Notebooks/Baseline%20Training%20and%20Evaluation%20Experiments/PredictiveModels_BY_DC_KNN.ipynb

Linear logistic regression was implemented to analyze the relationship between Minimum Pressure and Maximum Wind and predict hurricanes.
 
The files where linear and logistic regression are explored can be found under this folder: https://github.com/unicornpjs/Dubai_UG_3/tree/d4b84f6e7296c88e7461bf405853ca193d390a4b/Notebooks/Baseline%20Training%20and%20Evaluation%20Experiments


## Neural Networks
### CNN
CNN was utilized in image processing, with the model being selected for its architectural advantages in recognizing patterns in image data. The dataset was split as done previously, with the CNN classifier being trained based on the segmented images. The images were passed through the algorithm layer by layer, first with the input layer before the algorithm extracted main features, creating links and flatting the features to fully connect the layers. This process was repeated multiple times to improve the performance of the program.

the file for CNN can be found at: https://github.com/unicornpjs/Dubai_UG_3/blob/d4b84f6e7296c88e7461bf405853ca193d390a4b/Notebooks/Image%20Processing/%20UG3_TechnoDragons_ImageProcessing.ipynb


##  Results

| Algorithm           | Accuracy | Precision | F1 Score | Recall |
|---------------------|----------|-----------|----------|--------|
| Naive Bayes         | 0.62     | 0.68      | 0.73     | 0.79   |
| KNN                 | 0.66     | 0.71      | 0.75     | 0.81   |
| Decision Trees      | 0.66     | 0.68      | 0.77     | 0.90   |
| Logistic Regression | 0.65     | 0.65      | 0.79     | 1.00   |
| CNN                 | 0.86     |     -     |     -    |    -   |



## Files/folders in the Git Reprository

### Datasets
Contains the the two Datasets used.
#### Hurricane Data Numerical:
contains atlantic.csv and pacific.csv files
#### Image Dataset:
contains damage and no damage files

### Documentation
Within documentation, we have two files that tracks weeky updates and intitial idea exploration.

### Notebooks: 
#### Baseline Training and Evaluation Experiments:
contains files for linear and logistic regression, KNN, decision tress and Naive bayes

#### clustering:
contains the kmeans clustering file
#### Data PreProcessing and Analysis:
contains the numerical data preprocessing files
#### Image Processing:
contains the data preprocessing files for the images Dataset

### Project Pitch: 
contains the presentation for the project pitch.







