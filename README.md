# Housing Trends Across Five most populated towns in Connecticut

This project will show trends associatied with the housing market in Connecticut from 2006 to 2022. We will focus on the five most populated towns, the assessed property values vs. the sales amount, the sales amount and number and types of properties sold. We will utilize visualization tools to prove our finds.

## Instructions 

1. Retrieve data from DATA.Gov https://catalog.data.gov/dataset/real-estate-sales and save as Real_Estate_data.csv

2.  Load the [Real_Estate_data.csv]("Resources/Real_Estate_data.csv") file into Pandas DataFrame. 
    * view the headers 
    * filter data to have the five most populated towns in Connecticut.
        *`Bridgeport`, `Stamford`, `New Haven`, `Hartford`, `Waterbury`
    * narrow the `List Year` to exluded 2001-2005 as no property info was recorded.
    * filter for empty rows `Residential Type` and drop
    * create df_filtered to obtain .value_counts()
    
3.  Create a bar chart that visualizes the Resdential Sale Type
    
    * Title: Residential Sale Type
    * x-axis label: Residential Type
    * x-tick labels: Single Family, Cond, Two Family, Three Family, Four Family
    * y-axis label: Sale Amount

4.  * drop the `NaN` values [`longitude`, `latitude`, `sale amount`, `town`]
    * ensure `longitude` `latitude` and `sale amount` are numeric
    * push changes to a new dataframe

5. Create a bar chart for House Sale Amount in CT 2006 to 2022

    *  create a list indicating x labels, and set figure size to adjust for space  
    * Title: House Sale Amount in CT 2006 to 2022
    * x-axis label: List Year
    * x-tick labels: Year
    * y-axis label: Sale Amount

6.  Create a bart chart with a secondary line graph to show Total Sales Amount and Property Sales Count
    * Bar chart 
    * Title: Total Sale Amount and Property Sales Count by Town
    * x-axis label: Town
    * x-tick labels: `Bridgeport` `Hartford` `New Haven` `Stamford` `Waterbury`
    * y1-axis label: Total Sale Amount
    * y2-axis label: Property Sales Count

7.  Create data sets for the statistical analysis for assessed value and sales amount

8. Merge the two data frames on the `town` index

9. Plot the grouped bar chart
    * create a list indicating x labels, and set figure size 
    * Title: Comparison of Mean Assessed Value and Mean Sale Value by Town
    * x-axis label: `town`
    * x-axis ticks: `Bridgeport` `Hartford` `New Haven` `Stamford` `Waterbury`
    * y-axis label: `value`
    * ax. legend

10. Create a geographical scatter plot showing the locations `Bridgeport` `Hartford` `New Haven` `Stamford` `Waterbury`
    * create the dataframe
    * create geo scatter plot
    * customixe the layout 
    * show the plot 

11. Create a Linear regression 
    * create the variables to be listed
    * calculate slope (m) and y-intercept (b)
    * plot the results
    * set y- axis: (0,700000)
    * set x-axis: (years)
