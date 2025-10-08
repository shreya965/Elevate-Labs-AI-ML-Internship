## Data Preprocessing steps.

Used the Titanic dataset from Kaggle.

Loaded the data into datframe.

Checked the missing values in the data.

Checked the distribution of data with KDE plot.

The distribution was slightly skewed, close to normal so we used median for filling up the na values in the Age column.

Then cabin had many missing values ,almost 77% of the data in the column hence we could not remove the rows so we filled na values with Unknown.

Similarly embarked column had 2 missing values so we used mode to fill the na values here.

Then we performed one hot encoding ,droping the first column for 'sex' column and not dropping it for 'embarked' and 'deck' columns.

After this we scaled the numerical continuous data using standardscaler.

After that we plotted the box plot to find the outliers. There were alot of outliers for 'fare' and 'age' column and hence it did not make sense to remove those rows. 

For 'sib' and 'par' columns ,I printed the outliers and their values seem plausible in some cases, hence these outliers can be meaningful for analysis.
