# run_analysis.R description

The following package is used inside the script so it must be loaded:
- dpyr

The script starts reading the following tables:
- X_test.txt
- y_test.txt
- subject_test.txt
- X_train.txt
- y_train.txt
- subject_train.txt
- features.txt
- activity_labels.txt

The script carries on appending *test* and *train* values to create two new datasets:
- x_values -> result of append X_train values to X_test values.
- y_values -> result of append Y_train values to Y_test values.

Then the relevant means and standard deviations are identified and allocated on *measurements* dataset

*specific_dataset* represents the *x_values* showing only the measurements on the mean and standard deviation for each measurement.

Afterward descriptive activity names were used to name the activities in the data set.

Finally *specific_dataset* is arranged, grouped by both subject and activity and each column is summarized with mean() function to generate the tidy data 

