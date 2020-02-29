### Python_Project_1
### Team 2


# Currency Exchange Dashboard for Travel Agency

## Team members:
Devin Nigro
Kebbin Eke
Mohan Nilavar
Song Zhao


## Background:
We have been tasked with building a currency exchange rate dashboard for a travel agency/online travel platform, in which a user would select currencies from dropdown menus and the rate of exchange would be displayed as an output. As an extension, we will also include a text box feature that will allow the user to type in an amount of the first currency, and the conversion rate will be multiplied by the input amount to display a converted amount of the second currency. The dashboard will also include an interactive map, in which the user could select two countries as an alternative way to display exchange rates.


## Project:
### Data:
Currency rates will be imported using the Forex_Python library.
For the map feature, we will need a data frame that matches countries with their currencies. We can probably access this data using the World Bank or CIA Factbook.

### Methodology:
The dropdown menus will be created using Panel’s interact feature.
The map will be created using the Mapbox API.
A dashboard will be created using Panel’s columns/rows and tabs features.

### Results:
The currency converter will display conversion rates between any two currencies.
A text box will allow the user to input an amount of the starting currency, and the rate calculated from the dropdown menus will be multiplied by the input to display an equivalent amount of the second currency.
The interactive map will allow users to select two countries and the conversion rate between the countries’ respective currencies will be displayed.

### Visualization:
The final visualization will include a convenient dashboard, with at least two tabs, one for the dropdown currency converter and amount converter, and one for the map.
