# UFOs
Creating a webpage with a dynamic table and filter for UFO sightings using Javascript and D3.

## Overview
In this project Javascript was used to create a filter function that allowed users to filter for multiple criteria at the same time. The webpage only had a filter for date, so more filter inputs were added via HTML. After assigning unique ID's to each of the input elements, the code was able to be refactored to store our inputs into a variable and and filter our data by the selected filters.

![filter_search](/Resources/filter_search.PNG)


## Results
The webpage now successfully filters data based on user input. An empty object was created to store the users input, and a function was created to grab the user input and store it in the filter object.

![updateFilters](/Resources/updateFilters.PNG)

After the filters have been added to the filters object, another function looped over the filters and created a filtered dataset. That new dataset would be used with the function that builds the table and displays it in the webpage.

![filterTable](/Resources/filterTable.PNG).

Now our webpage can search our data with multiple filters with user input. After entering the filters the user just has to press the enter key or click on another part of the webpage and the table will update. To clear the filters the user can just select the UFO sightings link in the top right corner, or clear out the filters and press enter.

![filtered_table](/Resources/filtered_table.PNG)

## Summary

In summary this filtering system does do what is intended, but there are some drawbacks. The user input must be an exact match of the data they are trying to filter by. It's case-sensitive and some of the filterable parameters might not be known to users without inspecting the whole table. (ex: "shape: changing").

### Recommendations 

1. Since all of the data we are filtering from is in lowercase, I think the Javascript ```toLowerCase()``` method should be applied to the users inputted filters to help with user experience. A user won't know the filters are case sensitive without prior knowledge.

2. I think displaying what parameter the user could filter by would help with the user experience. A drop down list on the input fields that would list all values able to be filtered would make the webpage more intuitive.