# UFOs
Creating a webpage with a dynamic table and filter for UFO sightings using Javascript and D3.

## Overview
In this project javascript was used to create a filter function that allowed users to filter for multiple criteria at the same time. The webpage only had a filter for date, so more filter inputs were added via HTML. After assigning unique ID's to each of the input elements the code was able to be refactored to store our inputs into a variable and and filter our data by the selected filters.

![filter_search](/Resources/filter_search.PNG)


## Results
The webpage now successfully filters data based on user input. A variable was created to store the users filters and a function was created to grab the user input and store it in the filter varaible.

![updateFilters](/Resources/updateFilters.PNG)

After the filters have been added to the filters variable, another function looped over the filters and created a filtered data set. That new dataset would be used with the function that builds the table and displays it in the webpage.

![filterTable](/Resources/filterTable.PNG).

Now our webpage can search our data with multiple filters using user input. After entering the filters the user just has to press the enter key and the table will update. To clear the filters the user can just select the UFO sightings link in the top right corner, or clear out the filters and press enter.

![filtered_table](/Resources/filtered_table.PNG)