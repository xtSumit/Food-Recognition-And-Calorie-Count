# Food-Recognition-And-Calorie-Count

## Sections 
+ [Problem Statement](https://github.com/vipul-khatana/Food-Recognition-And-Calorie-Count#problemstatement)
+ [Objective](https://github.com/vipul-khatana/Food-Recognition#objective)
+ [Technique Employed](https://github.com/vipul-khatana/Food-Recognition#techniques-employed)

## Problem Statement
To create a food recognition system which helps to keep track of everyday calorie intake based on food recognition and classification to maintain a healthy lifestyle.

## Objective
In this project we tackle the problem of recognizing a food item from an image and subsequently measuring the calorie intake from the image of the dishes being consumed. The Dataset is gathered from the local restraunts and cafeteria around my college campus wich are easily available to the students. The food items chosen to create the dataset are as follows idli, dosa, apple, banana, paneer tikka and palak paneer, all of which are Indian cuisine. This project finds application in the area of health analytics, where dieticians can recommend their patients the calorie intake, and the patients by using an app that can take the photo of the meal they consume and keep track of their calorie in take. Further the data of calorie intake can also be used to find the co-relation between the calorie consumption and the various health problems.  

## Proposed System
The following is a simple process chart of how the task is achieved 

<img src="flow_chart.png" alt="Drawing" width="500" height="300"/>

In this project we focus on step 3,4 and 5 which have been explained in brief below 

+ **Segementation** - Mean shift algorithm is applied for the process of segmentation. It consisted of five steps : [CIELAB conversion](https://en.wikipedia.org/wiki/Lab_color_space), [Pyramidal mean-shift filtering](https://en.wikipedia.org/wiki/Mean_shift), [Region growing](https://en.wikipedia.org/wiki/Region_growing), [Region merging](https://en.wikipedia.org/wiki/Statistical_region_merging), [Plate Detection/Background deletion](https://en.wikipedia.org/wiki/Background_subtraction) 

+ **Feature Extraction** - Color feature extraction was done using [k-means algorithm](https://en.wikipedia.org/wiki/K-means_clustering). While the [Local Binary Pattern](https://en.wikipedia.org/wiki/Local_binary_patterns) operator was used for texture extraction. 

+ **Classification** - Support Vector Machine(SVM) with an RBF Kernel is used for the process of classification. 

