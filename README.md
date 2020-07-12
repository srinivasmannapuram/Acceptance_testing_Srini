Application displays the 5 day weather forecast for a given location for every 3 hours.

/* Features of the application as mentioned in the scenario*/

1. Search weather forecast for 5 days with data every 3 hours by city name
2. Search weather forecast by selecting the day and retrieve 3 hourly forecast
3. Search weather forecast by selecting the day again, hide 3 hourly forecast
4. Search weather forecast by Daily will summarise the 3 hour data for the following parameters:
    i. Most dominant (or current) condition
    ii. Most dominant (or current) wind speed and direction
   iii. Aggregate rainfall
     iv. Minimum and maximum temperatures
5. All decimal values should be rounded down


/* Automatable Scenarios */:

1. Verify application displays weather forecast for 5 days with data every 3 hours by city name..
2. Verify application displays weather forecast by selecting the day and retrieve 3 hourly forecast.
3. Verify the application hides 3 hourly forecast on selecting the same day again.
4. Verify the application is showing the 3 hour data for daily forecast of current condition, wind speed, direction, aggregate rainfall and temperatures.
5. Verify all the values displayed on the application are rounded off to the nearest value.

/*Negative Scenarios */
1. Verify error is displayed if city is not selected for the Test data or lft blank.
2. Verify city entered is not case sensitive.
3. Verify if weather forecast is displayed from the current day.


/* Run the feature */ 

    $ ./node_modules/.bin/cucumber-js or npm run acctest

/* To Generate report of the execution run the Gulp file in the repository */

    $ gulp cucumberReports  

/*What was used to save time for this solution*/

1. Came up with a node.js kind of implementation and used all the existing libraries I used for different solutions to save time
2. gulp cucumberReports  command can be used to generate the report.
3. As the time was limited only few scenarios could be covered and automated
4. HTML, Javascript ans core Java were used in the repo.


/* if given more time , following can be acheived to my knowledge */

1. We can implement a framework compatible with different browsers like safari, IOS etc..
2. We can implement Page object model or simple POM.xml type of solution that can help in covering wider scenarios and entire features of the application. 
3. TestNg kind of reporting can be implemented in the framwork itself.


