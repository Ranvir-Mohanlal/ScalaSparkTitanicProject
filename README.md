## Overview
This project serves as an example of a scala-spark project using the Kaggle Titanic dataset

## Usage
1. clone repository to local directory
2. cd into directory
3. compile the project with sbt using:
```
sbt package
```
4. Train model pipeline using:
 ```
 spark-submit --class ModelTrain --master local[*] --driver-memory 4G target/scala-2.11/scalasparktitanicproject_2.11-1.0.jar
 ```
4. Train model pipeline using:
 ```
 spark-submit --class ModelPredict--master local[*] --driver-memory 4G target/scala-2.11/scalasparktitanicproject_2.11-1.0.jar
 ```

## Notes
Predictions data will be saved as a csv file in the predictions directory found in project root dir