# Getting-and-Cleaning-Data
The mean and SD data of accelerometer is extracted from train/X_train.txt and test/X_test.txt and saved in trainData and testData dataframes respectively. Note that the dataframe's columns have been named while extracting the data.
The data for test/train activity and test/train subjects is extracted in a same manner.
The train and test dataframes are merged using rbind. The merged dataframes are combined together using cbind to form a new dataframe.
The final table is converted to tbl format and saved in newTable object for further operations.
All objects expect newTable are removed from workspace.
Data in Activity column is replaced with appropriate string values using mutate function and ifelse function.
A new independent tbl object is created from newTable called summaryTable which contains the mean of all the data grouped by values in activity column.
The summaryTable object is writen in Output.txt with row names removed.
The summaryTable and newTable objects are removed from workspace.
The dplyr library is detached from the workspace.
