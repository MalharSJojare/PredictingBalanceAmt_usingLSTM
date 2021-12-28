# PredictingBalanceAmt_usingLSTM
-------------------------------------------
## Contents
* Libraries required
* Getting the dataset
* Subsettings
* Training and Validating
-------------------------
# Note- For analyzing purposes I have use the Jupyter Notebook, but the code works with any of the computing platform.
### Libraries Required
  Most of them are default libraries are used, but additionally for dataset files ,subsettings, training purpose we are going to use these
1. pandas 
2. numpy
3. keras
4. tensorflow
5. JSON
#### You can use the command-> pip install libraryname in Jupyter's terminal to install the library, if not installed earlier.
-------------------------
### Getting the dataset
Here I have used the banking dataset which contains multiple columns and numerous rows. There are empty values in dataset, i.e. why I use the fixed number of records from the dataset. Here, I have used csv file for dataset but a JSON, pdf or xlsx file can be used. I already put the JSON file conversion to csv. The dataset can be changed according to your need, just changed the file path in code and start working with subsettings.


------------------------------------------------
### Subsettings
Check the required columns and starts working on them, the important thing is you are predicting the data with respect to what i.e. date any specific index value.
1. Drop the columns which are not needed
2. Replace the special characters such as $, %, & etc. with blank space
3. Check the datatypes if you are using date as index check the datatype of date if its an object then change it datetime (refer online for help regarding how change the object to date)
4. Sort the index
5. Plot the simple graph between index and training data and understand the trends(upward, downward, exponential etc.)
---------------------------------------
### Training and Validating 
For training purpose the one should have at least 200 records and for validating 50 records.

The total records should be greater than or equal to 250 minimum.

Transform the data using MinMaxScalar into the range of 0 to 1.

Select the number of records you are going to use for training purpose and for validating as well.

I have used LSTM model for prediction purpose because it works great with Time-Series datasets.

Train the data using model functions, predict the values and lastly plot a graph.
