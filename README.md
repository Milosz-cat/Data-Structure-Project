# Data-Structure-Project
The aim of the project is to demonstrate the benefits of using formats designed to store large data sets.

The studied formats use different data structures, which affects various aspects, such as the time of writing and reading data.

## Our large dataset
https://www.kaggle.com/datasets/wabinab/g2net-as-image?select=test

## Wave file 
In this file, we do a study in which we load a certain number of images from the dataset and then measure the read/write time compared to a direct write to the disk, and pay attention to the amount of memory used by the format.

## Wave_2 file
In this file, we divide our dataset into the given number of smaller datasets in order to train the model more efficiently. On the disk, we need to put the right number of subfolders, but the HDF5 and TFrecord formats offer saving the entire dataset in one file and using slicing for partial use of data without loading the RAM memory with the entire dataset. We then time the data readings before training. We simulate the operation of the data generator through the for loop because we do care about the speed of data reading.

## Report
https://docs.google.com/document/d/1idYBmvavqTwhH0f8VU5Tc5dZ90aCG6fRxHzmVy9duGE/edit

## Parquet and Feather (tabular data)
https://www.youtube.com/watch?v=u4rsA5ZiTls

## Helpful links
https://realpython.com/storing-images-in-python/
https://medium.com/@mrgarg.rajat/training-on-large-datasets-that-dont-fit-in-memory-in-keras-60a974785d71
https://openml.github.io/blog/openml/data/2020/03/23/Finding-a-standard-dataset-format-for-machine-learning.html
