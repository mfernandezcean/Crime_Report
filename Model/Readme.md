## Model:

![image](https://github.com/mfernandezcean/Crime_Report/assets/105746149/076238df-6831-46b7-9a02-1a929b710766)

Simple Two Table with a Many-To-One Relationship, Between Data Table and Crime Types Table. With flow of Data going from Crime Types to Data. Joined by the 'Crime Type ID' Column.

## Date Table:

Go to 'New Table':

![image](https://github.com/mfernandezcean/Crime_Report/assets/105746149/daded494-645b-4867-b26a-aa6ac92aceef)

Use DAX to 'Addcolumns' to the new table. Using CALENDARAUTO() the function will read the data we've got and automatically assigned, in this case, a 'Year'. 
```
DateTable = 
ADDCOLUMNS(
    CALENDARAUTO(),
    "Year", YEAR([Date])
)
```

![image](https://github.com/mfernandezcean/Crime_Report/assets/105746149/e26c78b5-ed6f-4a7f-8c75-91659b302bd6)
