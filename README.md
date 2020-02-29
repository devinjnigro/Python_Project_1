# Currency Exchange Dashboard for Travel Agency

## Team 2: members:
Devin Nigro\
Kebbin Eke\
Mohan Nilavar\
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


# Conclusions:
We utilized a currency API (Currency Layer) in order to pull exchange rate data in real time. Whenever a new currency is selected in one of the dropdown menus and the convert button is pressed, new data would be pulled from the API, unless the exchange rate for the selected currencies has already been pulled and cached within a specified time period (we chose 20 seconds). The map feature that we incorporated into the converter was created using choropleth, a function within Plotly that renders a world map with color-coded selected countries. Choropleth recognizes the borders of any selected country based on the currency the user selects from the dropdown menus. The dropdown menus, input and output text boxes, and 'Convert' and 'Switch' buttons were created using IPYwidgets, a library within Python that creates user-friendly widgets and allows them to be compiled into a single interface, in which they can interact with each other seamlessly. We used CSV files containing country names, ISO codes, currency symbols, and country codes in order to further enhance the user experience by making easier to identify currency names in the dropdown menus, which in turn served as key values in a dictionary, paired with ISO codes that then signal to the API which currencies we are selecting. The currency symbols displayed next to the text boxes were also drawn from a dictionary created pairing ISO codes with the symbols.

The API we used offered additional options, such as the ability to pull historical exchange rate data between two currencies over a specified time period. We used this data to observe the British Pound / US Dollar exchange rate over a period of time that included Brexit referendum, and we noticed a clear weakening of the pound over this period, which was in line with our prediction. The use of historical exchange rates from the API we used can be used to observe the effects of any number of global events in which one currency would be expected to be affected more than the other.
