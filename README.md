# Matplotlib Homework - The Power of Plots

![Laboratory](Images/Laboratory.jpg)

You've joined Pymaceuticals Inc., a burgeoning pharmaceutical company based out of San Diego. Pymaceuticals specializes in anti-cancer pharmaceuticals. In its most recent efforts, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

As a senior data analyst at the company, you've been given access to the complete data from their most recent animal study. In this study, 249 mice identified with SCC tumor growth were treated through a variety of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals' drug of interest, Capomulin, versus the other treatment regimens. You have been tasked by the executive team to generate all of the tables and figures needed for the technical report of the study. The executive team also has asked for a top-level summary of the study results.

## Observations
  - Strong positive correlation between Average Tumor Volume vs. Mouse Weight for Capomulin regimen: 0.84

  - Minimum Tumor Volume 22.050126 and max Tumor Volume 78.567014 across 
    regimens Capomulin, Ramicane, Infubinol, and Ceftamin are within IQR upper and lower bounds

  - Potential outliers for Infubinol, Values below 36.83290494999999
    Potential outlier for Infubinol: 36.321345799999996 (denoted above with red square in box and whister plot)

  - Line graph indicates that the majority of mice observed had an overall decrease in Tumor Volume (mm3) over timepoints. 
    Exception: Tumor Volume (mm3) increased for Mouse ID i557.

## Objectives

Objectives in this project are as follows:  

* Before beginning the analysis, check the data for any mouse ID with duplicate time points and remove any data associated with that mouse ID.

* Use the cleaned data for the remaining steps.

* Generate a summary statistics table consisting of the mean, median, variance, standard deviation, and SEM of the tumor volume for each drug regimen.

* Generate a bar plot using both Pandas's `DataFrame.plot()` and Matplotlib's `pyplot` that shows the total number of measurements taken for each treatment regimen throughout the course of the study.

  * **NOTE:** These plots look identical (plots generated using pandas `DataFrame.plot()` vs Matplotlib's `pyplot`).

* Generate a pie plot using both Pandas's `DataFrame.plot()` and Matplotlib's `pyplot` that shows the distribution of female or male mice in the study.

  * **NOTE:** These plots look identical (plots generated using pandas `DataFrame.plot()` vs Matplotlib's `pyplot`).

* Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Calculate the quartiles and IQR and quantitatively determine if there are any potential outliers across all four treatment regimens.

* Using Matplotlib, generate a box and whisker plot of the final tumor volume for all four treatment regimens and highlight any potential outliers in the plot by changing their color and style.

  - All four box plots display be within the same figure. Use this [Matplotlib documentation page](https://matplotlib.org/gallery/pyplots/boxplot_demo_pyplot.html#sphx-glr-gallery-pyplots-boxplot-demo-pyplot-py) was used as reference for changing the style of the outliers.

* Random number generator was used to select a mouse that was treated with Capomulin and generate a line plot of tumor volume vs. time point for that mouse.

  - Re-run this section to select a new random mouse treated with Capomulin and generate a new line plot for tumor volume vs. time point for that mouse.  

* Generate a scatter plot of mouse weight versus average tumor volume for the Capomulin treatment regimen.

* Calculate the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment. Plot the linear regression model on top of the previous scatter plot.

* Properties included on plots/figures: plot titles, axis labels, _x_-axis and _y_-axis, etc.