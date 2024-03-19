# Lead-Score-Case-Study
A detailed analysis using Logistic Regression is done for an education company X Education that sells online courses to industry professionals. The raw data from the past of 9000 data points was provided, from which Hot Leads i.e. leads likely to convert into paying customers are identified and assigned lead score based on the most significant model. 
Steps followed are:
	Cleaning Data:
The data was first cleaned by:
	Replacing “Select” by NaN values
	Converting all the values in the dataset into lowercase
	Removing variables with more than 35% missing values
	Replacing import columns NaN values with ‘Not Provided’
	Identifying the country India with maximum customer views. 

	Exploratory Data Analysis (EDA):
To check the distribution of our dataset and correlation among the variables we performed EDA. It was found that many categorical variables were highly correlated hence dropped before building the model, and there were no visible outliers in the data set.


	Data Preparation:
	Dummy Variable: Dummy variables for 8 category variables were created and later dummies with not provided dummies and the first dummy of each variables were removed from the data.
	The numeric values are appropriate and scaled using MinMax Scaler,
	Train and Test split of data set.

	Model Building: 
On the train data we use RFE method and  identify 15 the most relevant features from the data set. After dropping the high VIF and insignificant variables or features from the data set we finally get a 12 feature model all significant at 5% level with VIF less than 5 for all.
