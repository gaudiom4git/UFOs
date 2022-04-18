# Module 11 UFOs
## Overview of Project
The objective of this project was to display documented UFO sightings.  Each sighting has a sighting date, city, state and country.  
The general shape of the UFO and how long the UFO was visible.  Since the list of sightings is quite large, filter search fields are available
on the left by sighting date, city, state, country and shape.

This weeks lesson introduced us to Javascript by providing its similar concepts in Python.  Concepts covered were printing to a console, variable 
assignments, arraysm conditional logic, for loops, and functions.  Once students understood how to code in Javascript, the lesson taught students 
how HTML and Javascript interact by using event listeners to monitor for events triggered within the HTML page such as button clicks, input entry
changes using D3.

Use of the console log is very helpful in debugging issues when the code wasn't working as expected.

Use of arrow function used in the filterTable function as well as the D3 listener selectAll cut down alot of code.

## Results
The search was performed by monitoring for changes to the 5 input text boxes listed under the filter search list.   The D3 event listener (D3.selectALL) 
would listen for any and all changes made to any of the filter text boxes and call the updateFilter function to build a dictionary of the 
element that changed and the value entered by the user.  

It's important to note that the keys in the data.js file have the same name as the element id in index.html so that the filter would properly 
filter on the data in data.js.   I made this mistake where they didn't match and I couldn't understand why my filter wasn't working.

Arrow function was used to loop through the filterChgList dictionary and would apply the filter to the filteredTable until all key/value pairs 
in the filterChgList dictionary were applied.

[Data Must Match Element ID](https://github.com/gaudiom4git/UFOs/blob/main/resources/datamatchelement.png)

[Filters In Action](https://github.com/gaudiom4git/UFOs/blob/main/resources/FilterInAction.png)


## Summary

One drawback on this webpage is that the filter criteria is case sensitive.   So, the state values in the data.js file could be upper or lowercase.
Then, the filter would not work unless you converted the values so that the cases were the same.

Another recommendation would be to have a date range instead of an exact date.

