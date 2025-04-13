# Code Book

## Data Source

Original data was collected from the UCI Machine Learning Repository:
[Human Activity Recognition Using Smartphones Dataset](http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones)

## Variables in Tidy Data Set

The tidy data set includes the following variables:

- `subject`: ID of the subject (1-30)
- `activity`: Descriptive activity name (WALKING, WALKING_UPSTAIRS, etc.)
- All other columns are averages of the original mean and standard deviation measurements.

These features were selected from the original dataset because they contain either `mean()` or `std()` in their name.

## Transformations Performed

1. The raw data files were merged to create a unified dataset.
2. Only columns with measurements on the mean and standard deviation were extracted.
3. Activity codes were replaced with descriptive names.
4. Variable names were cleaned up:
   - `t` replaced with `Time`
   - `f` replaced with `Frequency`
   - `Acc` replaced with `Accelerometer`
   - `Gyro` replaced with `Gyroscope`
   - `Mag` replaced with `Magnitude`
   - `BodyBody` fixed to `Body`
5. A new dataset was created with the average of each variable for each subject and activity combination.
6. The final tidy dataset was written to `TidyData.txt`.

## Units

All measurement variables are normalized and dimensionless. They represent sensor signals.

