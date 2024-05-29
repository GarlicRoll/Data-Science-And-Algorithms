# Data-Science-And-Algorithms
## Assignment 1: My Road Network
Important Time
Submission: 23:59 Mar. 14, 2024 (UTC+8)
Study Area
minimum latitude: 39.84
minimum longitude: 116.30
maximum latitude: 39.97
maximum longitude: 116.46
Task Description
l Construct a routable road network based on NetworkX
n Each edge should at least contain "type"/"highway" and "length"
i. Method 1: OSMnx
ii. Method 2: From scratch (w/o using OSMnx): An optional choice, you would be
awarded with bonus score if you choose such a method.
n Test whether the shortest path query can work correctly given arbitrarily two vertices in the
road network (show the testing process in your report).
 - It should be already functional if you use Method 1 to construct the road network.
Otherwise, you should pay additional attention to it.
 - The shortest path query is NOT required to be implemented by your own. You can use the
interface of NetworkX, e.g., nx.shortest_path, nx.astar_path
l Visualize your network data with at least 3 figures using arbitrary visualization tools.
n (Optional): At least one figure is draw by KQGIS Desktop.
For example, you can plot the road network in QGIS, draw the distribution of the road type/highway,
the distribution of the road length, ...
       
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
