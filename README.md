# Data-Science-And-Algorithms
## Assignemnt 1: Building path
Study Area
min_lat = 39.84     
min_lon = 116.30     
max_lat = 39.97     
max_lon = 116.46     
Getting study area graph (with roads for cars)     
Two random points on the map which I will use to calculate route     
Calculating shortest path between two points with dijkstra algorithm      
Figure 1: Road network plot using OSMnx      
Figure 2: Scaled map of our route     
Figure 3: Histogram of edge lengths      
Figure 4: Bars of different types of roads      
Saving graph and shortest path for QGIS      


## Assignment 2: My Spatial Databases
Important Time
Submission: 23:59 Mar. 21, 2024 (UTC+8) ### Related Datasets Assignment2-
2012_BIT_POI.csv ### Task Description 1. Build an in-memory spatial database for Point
of Interest (POI) that can support the spatial range query and the nearest neighbor query. 2.
Demonstrate the efficiency of the spatial index. 3. Use your database to answer following questions. a) What’s the nearest ATM (type_code starting with “1603XX”) around Central Building of BIT (latitude:39.958, longitude:116.311)? b) How many restaurants (type_code starting
with “5XXXX”) within 500 meters of the south door of BIT (latitude:39.955, longitute:116.310)?
What You Need to Program 1. An index-building function (implemented by your own)
index = IndexBuilding(file_path) 2. A range query function based on the spatial index res =
RangeQuery(query_range, type_regex_str, index) “query_range” could either be - (upper-left,
bottom-right) rectangle - A central point + a radius square “regex_str” is the regular expression string to match the type_code 3. A nearest neighbor query function based on the spatial
index res = NNQuery(query_point, type_regex_str, index) 4. A brute-force range query function res=RangeScan(query_range, type_regex_str, file_path) 5. A brute-force nearest neighbor
query function res=NNScan(query_point, type_regex_str, file_path) 6. Compare the efficiency
of different queries with/without the spatial index 7. Answer above questions


## Assignment 3: Intelligent Cancer Diagnose
Important Time
Submission: 23:59 Apr. 11, 2024 (UTC+8)
Related Datasets
Assignment3-Breast-Cancer-Diagnose.csv
Task Description
According to features computed from a digitized image of a fine needle aspirate (FNA) of a
breast mass, choose appropriate classifier to diagnose whether breast tissues are malignant or
benign.
What You Need to Program
1. Split your datasets into train/val/test or train/test.
2. Implement at least 3 types of classifiers to make the binary classification.
3. Give the process about how you choose the hyperparameters for each classifier.
4. Compare the performance of difference classifiers.
Note
5. This work can be done using scikit-learn.
6. Using the provided ".csv" file. Do not directly load your data using the scikit-learn
API, i.e., "sklearn.datasets.load_breast_cancer ".
