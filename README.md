Coffee Production Analysis
==========================

This project dives into an analysis of coffee production data, aiming to uncover
trends in total coffee production across various regions and time periods. I
used Python for data manipulation, exploration, and visualization to help shed
light on production patterns.

Files in this Repository
------------------------

-   `total-production.csv`: The main dataset, with details on coffee production
    by region, month, year, yield, and total production.

-   `Coffee_Analysis.ipynb`: A Jupyter Notebook with all the code used to
    analyze `total-production.csv`. This includes data cleaning, manipulation,
    and visualizations to bring the data to life.

Project Overview
----------------

In this analysis, I focused on:

1.  **Data Cleaning**: Preprocessing steps like handling missing values,
    adjusting data types, and removing unnecessary rows or columns.

2.  **Exploratory Data Analysis (EDA)**: Basic statistics and visualizations
    that reveal underlying patterns in coffee production.

3.  **Data Manipulation**: Transforming data to look at production totals by
    year, region, and month.

4.  **Visualization**: Creating charts and graphs to illustrate trends over time
    and across regions.

Requirements
------------

To run the notebook and reproduce my analysis, you’ll need the following Python
libraries:

-   **Pandas**: For data handling.

-   **Matplotlib**: For plotting.

-   **Seaborn**: (Optional) For more polished visualizations.

If you don’t have them installed, you can install them with:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
bashCopy codepip install pandas matplotlib seaborn
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

How to Use
----------

1.  **Clone the Repository**: Clone this repository to your local machine:

    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    bashCopy codegit clone https://github.com/your-username/coffee-production-analysis.git
    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

2.  **Open the Notebook**: Navigate to the project folder and open the Jupyter
    Notebook:

    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    bashCopy codejupyter notebook Coffee_Analysis.ipynb
    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

3.  **Run the Notebook**: Go through each cell to see the analysis steps and
    visualizations.

Example Code Snippets
---------------------

Some of the code used in the analysis:

-   Loading and displaying the dataset:

    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    pythonCopy codeimport pandas as pd
    coffee_production = pd.read_csv("total-production.csv")
    coffee_production.head()
    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

-   Setting the first row as column headers:

    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    pythonCopy codecoffee_production.columns = coffee_production.iloc[0]
    coffee_production = coffee_production.drop(0).reset_index(drop=True)
    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

-   Dropping unnecessary columns:

    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    pythonCopy codecoffee_production.drop('total_production', axis=1, inplace=True)
    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Results
-------

This analysis helps reveal patterns in coffee production by looking at changes
across different regions and years. The Jupyter Notebook contains all the
insights and visuals generated from this data.

License
-------

This project is open-source under the MIT License.
