# Quant-Project

# Market Analysis

## Variance & Measures of Dispersion

Dispersion measures describe how spread out a dataset is, providing insights into its variability. Two key measures of dispersion are variance and standard deviation:

Variance: The average of the squared differences between each data point and the mean. It provides a sense of how much the data points deviate from the average.

Standard Deviation: The square root of the variance, representing the average distance of each data point from the mean. It is easier to interpret as it is expressed in the same units as the data.

However, both variance and standard deviation treat upward and downward deviations equally, meaning they do not account for directional trends. Additional tools, such as skewness and kurtosis, can provide more nuanced insights into data distribution.


![image](https://github.com/user-attachments/assets/3b862607-1fd0-4ad1-83f7-24cdabfb9cde)
![image](https://github.com/user-attachments/assets/6a9ae408-97e6-4416-8968-1b40bad2f6e5)
![image](https://github.com/user-attachments/assets/eb3fbcf9-a3ef-4aee-a371-1bd92bc23695)


## Simple Displays

Graphical representations of data can help us intuitively understand patterns, trends, and potential flaws in datasets. Plots are powerful tools for:

Identifying potential structure or anomalies in the data.

Formulating hypotheses by visualizing data behavior.

However, it is essential to remember that plots are exploratory tools, not confirmatory. They should not be used for hypothesis testing as they lack statistical rigor.

Common types of simple displays include:

Histograms: To visualize the frequency distribution of a variable.

Scatterplots: To examine relationships between two variables.

Box plots: To highlight the spread and identify outliers.

![image](https://github.com/user-attachments/assets/061e4d8d-7362-4b2f-b4f9-4c42a255775c)
![image](https://github.com/user-attachments/assets/53fb488b-bf11-45c5-b18f-71adf37a5cad)
![image](https://github.com/user-attachments/assets/29c00d43-7634-482c-a509-9c8ae4184c35)
![image](https://github.com/user-attachments/assets/e9289063-8fb2-4398-8aed-cee980a8fe4b)
![image](https://github.com/user-attachments/assets/4d3799c1-8e35-491d-b346-ac8602e167a2)



## Statistical Moments

Statistical moments extend beyond mean and variance to provide a more comprehensive understanding of a dataset:

Mean (First Moment): The central tendency of the data.

Variance (Second Moment): The spread or dispersion of the data.

Skewness (Third Moment): Measures the asymmetry of the data distribution.

Kurtosis (Fourth Moment): Indicates the "tailedness" or extremity of the data distribution.

To assess normality in data, the Jarque-Bera Test can be used. This test combines skewness and kurtosis to determine whether a dataset follows a normal distribution. Financial returns, for example, often exhibit fat tails and skewness, deviating from normality.

![image](https://github.com/user-attachments/assets/43b83594-c724-4bfd-910a-baee576c5094)
![image](https://github.com/user-attachments/assets/47de3433-45af-48f7-a750-e1d720472591)
![image](https://github.com/user-attachments/assets/d13d6918-27e7-4bc5-b975-3140be2f1c36)


## Linear Correlation Analysis

The correlation coefficient quantifies the strength and direction of a linear relationship between two variables:

Values range from -1 to 1:

1: Perfect positive correlation.

0: No linear correlation.

-1: Perfect negative correlation.

It measures the degree to which changes in one variable predict changes in another.

While correlation is a valuable tool, it has limitations. It only captures linear relationships and may overlook more complex, non-linear interactions.

Instability of Parameter Estimates

When analyzing data over time, parameter estimates can fluctuate, revealing their instability:

Moving Window Analysis: Dividing the dataset into subsets (time windows) to observe how parameter estimates change.

Quantifying Instability: By measuring the variability of these moving estimates, we can assess the uncertainty in the parameters.

Understanding instability helps determine whether model estimates are robust or overly sensitive to specific data subsets.

![image](https://github.com/user-attachments/assets/dd623508-5111-4af7-8893-dfe5a94aa833)
![image](https://github.com/user-attachments/assets/5549f3d0-b0c3-417b-8019-54dd22795416)
![image](https://github.com/user-attachments/assets/5d2707a7-2be4-4a74-a0f3-eefa95a652b7)




## Introduction to Linear Regression

Linear regression is a foundational statistical method for understanding relationships between variables. Given an independent variable (X) and a dependent outcome variable (Y), linear regression finds the best-fit line, modeled as:



Where:
- Intercept (value of Y when X = 0).
- Slope (rate of change in Y for a unit change in X).

This technique is widely used in predictive modeling and provides insights into the strength and nature of relationships between variables.
![image](https://github.com/user-attachments/assets/59d623eb-3a79-4d76-9191-740aecc6198b)


## Regression Model Instability

Regression analysis involves estimating coefficients that relate multiple datasets. However, these coefficients can vary depending on:

The choice of dataset.

The time period considered.

The inclusion or exclusion of specific data points.

Moving Window Regression is a method to test the stability of these coefficients by repeatedly recalculating them for different time frames. Significant fluctuations in coefficients may indicate that the model is not robust or that the relationships it captures are not consistent over time.
![image](https://github.com/user-attachments/assets/ab26f006-d275-4169-9cc3-76bd150765c2)
![image](https://github.com/user-attachments/assets/0c41acc5-20ce-423f-834e-9104290551fb)
![image](https://github.com/user-attachments/assets/2d96ec6d-cf63-48f3-be77-5308addf52e7)
![image](https://github.com/user-attachments/assets/a42a465d-66d3-476d-a377-8406cbd340bf)




## Multiple Linear Regression

Multiple linear regression extends the simple linear regression model to include multiple independent variables:

Where:
- Independent variables.
- Coefficients representing the effect of each variable on Y.

This method allows for:

Predicting outcomes based on multiple factors.

Understanding the relative importance of each independent variable.

In quantitative finance, this is a crucial tool for building models that analyze and forecast market trends.

![image](https://github.com/user-attachments/assets/063b5edd-bc05-4d92-b899-64fa505b1a77)
![image](https://github.com/user-attachments/assets/0e528d6f-e343-43e1-9707-d0047d983e7c)
![image](https://github.com/user-attachments/assets/d4e31b73-6cff-4c20-9fce-e12e3f4beec7)
![image](https://github.com/user-attachments/assets/a7ce1efd-96a6-441c-95be-3fec1a42f336)
![image](https://github.com/user-attachments/assets/edb42f99-424c-4684-9aad-2d942e5f5f29)


## Violations of Regression Models

Regression analysis relies on key assumptions, such as:

Linearity: The relationship between independent and dependent variables is linear.

Homoscedasticity: Variance of the residuals is constant.

No Autocorrelation: Residuals are independent of each other.

Normality: Residuals follow a normal distribution.

Violations of these assumptions can lead to:

Biased estimates: The coefficients no longer accurately represent relationships.

Inefficient estimates: Increased variability in parameter estimates.

Invalid inferences: P-values and confidence intervals become unreliable.

To address these violations, techniques such as data transformations, robust standard errors, and model re-specifications can be employed to ensure valid results.

![image](https://github.com/user-attachments/assets/97be4a6f-6c02-4766-a2a1-29079c08bf9e)
![image](https://github.com/user-attachments/assets/f11df2d3-e51f-46c6-8f55-4612c5ea6f62)
![image](https://github.com/user-attachments/assets/b457bcaa-cb5d-4bd7-8aac-9ebb9fb29e90)
![image](https://github.com/user-attachments/assets/c1095b8a-4a79-43c7-8ef0-b6f8f5606c86)
![image](https://github.com/user-attachments/assets/0a0c2b24-0c8f-4a39-9bc7-ce9aac41dcb6)


