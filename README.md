# python-api-challenge
This is my submission for the python api challenge homework number 6

For this submission I use the starter code presented in the starter_code folder and all work is done in Jupyter Notebook, not Jupyter lab.

## WeatherPy ##

The weatherpy starter code has us starting out by gathering a random set of latitudes and longitudes within a set range

From there, I call the randomly generated latitudes and longitudes in a for loop to call the open weather API and store the data into various lists that I created. Then I store those lists in a dataframe

to get the summary statistics I use the .describe() method.

None of the cities I called had humidity over 100%, but I rote a short filter that only kept the data with humidity of 100 or less.

Using Matplotlib and my cleaned DF I create multiple scatter plots.

Then I create two new dataframes that filter for northern hemisphere latitudes and southern hemisphere latitudes and create scatter plots and perform a linear regression on each.

lastly, I write my pandas dataframe out into a csv to use in VacationPy

## VacationPy ##

I start by importing my csv dataframe then using that information to create a heatmap using humidity as the weight.

Then I filter down my dataframe to just the cities within my vacation paramaters (I used the default, recommended paramaters in the instructions readme)

From there I create a new Dataframe called hotel_df and use another for loop to call the Google Places API and store the relevant data into lists which I add to my dataframe.

Then I use that information to create markers to put on my map.