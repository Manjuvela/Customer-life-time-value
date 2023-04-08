
# Project Title

Lifetimes Package was developed by Cameron Davidson who is a Data Scientist at Shopify.
Frequency, Recency, and T, you are going to use the “summary-data-from-transaction-data” function.
Inside this function, you have to specify the Dataset and also Specify the Columns “CustomerID”, and “InvoiceDate” which are necessary for this Analysis. You are specifying the “Sales” column as the monetary_value_column and Observation_period_end Checking the Head of the Dataset: -
- The minimum value for Frequency is 0, the Average is around 2.86, whereas the Maximum Value is 131.
- The minimum value for Recency is 0, the Average is around 130, whereas the Maximum Value is 373. - The minimum value for T is 0, the Average is around 222, whereas the Maximum Value is 373.
- The minimum value for Monetary Value is 0, the Average is around 307, whereas the Maximum Value is 1.6 Million. The minimum value for Recency, Frequency, and Monetary value are all 0. 
- Checking the Percentage of Zeros in each of these columns. Frequency, Recency, and Monetary value, around 36% of all the values are Zeros.
## Installation


Python Libraries: -
- Numpy
- Pandas
- Seaborn
- Matplotlib

To Install the Lifetimes Package: -
Lifetimes. plotting and lifetimes. utils are Packages to import all the Classes.

Importing the Gamma-Gamma Model: -
Fit the Model with the Frequency and Monetary Value. 

And also check the Model Parameters. Use the onditional_expected_average_profit function available in the lifetime package.

## Contributing-

Distribution plot from the seaborn library: -
The distribution for Monetary Value and Frequency is Highly Skewed.

Recency and Duration - the Distribution is slightly skewed.

Important to check the Frequency-Recency Matrix.
The customer has made a purchase every day for four weeks straight, and then haven’t heard from him in months.

For frequency and Recency Analysis, you have to use the BG-NBD Model also known as Beta-Geometric or Negative Binomial Distribution Model.

Generally, the BG/NBD model is used to predict aggregate future transactions, and you are going to Visualize the Frequency-Recency Matrix.

Import the BG-NBD Model from the Lifetimes Package as “BetaGeoFitter”.
## Documentation



Importing the Dataset: -
Converting the Invoice Date column into a Date-time Object.

Remove all the Records from the Dataset. The notNull function allows you to get the missing values for CustomerID.

Remove all the Records where the Value is zero or less than zero.

Preparing the Dataset: -
Select only the CustomerID, the InvoiceDate, and the Sales Column to prepare our Dataset.

For Calculating the Lifetime Value of Customers. Statistical functions: -
- Minimum sales
- Average Sales
- Maximum Sales

Analyze Frequency and Recency Analysis to extract more Insights from the Generated Data. Using the BG-NBD Model you can also predict which customers are alive. 

Fit the BG-NBD model into the probability-alive matrix function provided by the lifetimes. 

plotting package. After fitting and executing the Model, you can see the Probability-Alive Matrix using this to Predict Whether the Customer is Alive or not.

Analyzing this Matrix: - 
- Upper-right of the Matrix - This Model exposes a method that will help you to predict a customer’s expected purchases using their history. 

You just need to use the Predefined function named - 

conditional-expected-number-of-purchases-upto-timefunction. Inside this function, you have to specify Frequency, Recency, and T.

The BG/NBD model believes that making more purchases within the near future is our best customer.
## Insights

If the Model’s Performance is Good by certain Metrics you can Trust the Output or Predictions made by the Model.
Plotting the Period Transactions, you can Import the plot_period_transactions function and fit the BG-NBD Model.

The Actual and Predicted Values in each of the Period Transactions mean our Model is Performing Well and Proceed Further.
Partitioning our dataset into a calibration period and a holdout dataset. After the Calibration Period and the Holdout Dataset are prepared. 

Separate the data into both an in-sample (calibration) and validation (holdout) period. The green and blue line presents the model prediction and actual result of the y-axis respectively. In the Next Video, you will Estimate the Total Lifetime Value of a Customer.
