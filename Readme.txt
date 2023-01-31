CHICAGO CRIME DATA ANALYSIS

INTRODUCTION:

A police officer may know where the risky locations are, but he may not be able to predict what kind of crime may occur. Our objective is to help police officers by providing useful information which is hard to get so that they can take appropriate measures. We have used Random Forest, Logistic regression, and Decision tree Algorithms to develop this project.
This notebook is a Spark and Python learner to perform data analysis on the Chicago crime dataset.
In this project, I mostly use Spark, Pandas, Matplotlib, Seaborn, and Plotly to build a meaningful pipeline for better results. The point is to:
•	Perform data reading and transforming using Apache Spark and MongoDB
•	Data Cleaning and Handling missing values is done by reducing the number of output classes and removing records with null values.
•	Extract data from the crime date by converting the date column into date time format and extracting new columns such as Day, Month, Weekday, and Hour.
•	Visualize the target feature with others using existing Python libraries such as Matplotlib, Seaborn, and plotly.
•	Prepare data for modeling using in-built methods such as StringIndexer, VectorAssembler, and OneHotEncoder and other feature engineering techniques.
•	Implement different machine learning models and analyze the predictions to choose the best one.

--> How to run this and what to run it on?
•	Coding is done in a step-by-step manner to maintain the sequence of the pipeline and the entire code is present in a single 'Chicago crimes project.ipynb' file.
•	I wrote this on Apache Spark 3.3.0. The entire pipeline was executed on a single Jupyter notebook using Python with version 3.9.7.
•	Spark can be downloaded from https://spark.apache.org/downloads.html 
•	To run this notebook, one certainly needs all the mentioned libraries such as:
•	Pandas
•	Numpy
•	pyspark
•	pyspark.sql
•	matplotlib
•	Seaborn
•	Plotly. express
•	DateTime
•	pyspark.ml.classification

For me, all that was sorted out using Anaconda: https://www.anaconda.com/download/

Material:
The dataset selected for this research comprises crime reports from 2001 to present data for the city of Chicago. The dataset has sufficient details about the crime's date, type, description, location, etc. for our study. It is a huge dataset. Processing this much data quickly and effectively is necessary. Due to its capacity to process data in memory, the Spark framework(doubt) is what we selected to handle this volume of data.
We have implemented some algorithms such as Random Forest, Logistic regression, Decision tree, and feature selection for building the pipeline.

The pipeline of our project is as follows:
1. Data preprocessing :
•	Dropped missing/null values.
•	Filtered out irrelevant features from the dataset.
•	Optimizing target column by reducing the number of classes.
2. EDA ( Explorater data analysis):
•	To identify and prevent crime, we deduced helpful information and examined significant trends. The evaluation will aid in locating beneficial characteristics for developing predictive models.
•	Methods: Bar graph, line graph, pie-chart, heatmaps.
•	We used Seaborn, Matplotlib and Plotly for this specific task.
3. Analysis:
•	Performed Feature engineering and selection using spark-specific functionalities such as StringIndexer, VectorAssembler and OneHotEncoder.
•	The following hypotheses were tested using logistic regression, random forest, and decision tree, and the outcomes were compared. The procedures are listed below:

Steps to be performed in Windows Machine:
1)	Install MongoDB Community Server along with MongoDB Compass
2)	Open MongoDB and Create DB " 603_project" and Collection "Chicago_crimes_data”.
3)	Download “Spark 3.3.0” from the official website: 
https://spark.apache.org/downloads.html
You can download the live dataset till the present date from  https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-present/ijzp-q8t2

4)	Load the dataset into the database created above in Mongo DB and copy the “URL”.
5)	When you open the notebook, make sure you install all the required libraries in the imports section before further steps.
6)	Before running the notebook, Change the dataset URL for spark to read and load it correctly into a spark data frame.
7)	Open the Jupyter Notebook and execute the cells and you can get the expected results.

