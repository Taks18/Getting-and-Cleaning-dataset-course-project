## Introduction

### The script run_analysis.R performs below mentioned steps

* First the data is downloaded from the location given.
* Training and test data is merged using rbind() function.
* Only mean and standard deviation measurement is derived from the feature data file and relavent data subsetted.
* Activity data has values of 1:6, using activity names from activity.txt the activity dataset is updated.
* Subject dataset updated with "Subject" column name.
* All the measurement, activity, and subject dataset is combined using cbind() function.
* Finally average dataset is created for each suject by activity type and uploaded .txt in repository.

## Variables

* x_train, y_train,x_test,y_test,subject_train,and subject_test contain the data from the raw files.
* x_data,y_data, and subject_data is rbinded using above data.
* xdata is updaed with feature dataset where measurement is only mean and standard deviation.
* Simmillar approcah for activity and subject dataset.
* all_data merged x_data,y_data, and subject_data with necessary transaformation
* Finally, averages_data contains relavent averages which are stored is average_data.txt.ddply() from plyr library is used to create average at subject and activity level.
