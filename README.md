# Data Visualization - Titanic - Relationship Explorer (D3.js)
Part of the mandatory Data Analyst Nanodegree curriculum. A data visualization project on D3.js using the Titanic Data Set

# Directory Structure
-  /Readme.md - this file
-  /index_1.html - first version (sketch)
-  /index.html - final version

# Summary

The data set has been extensively used by data analysts to build predictive models on the survivability of passengers. The visualization intends to help the reader analyze the distribution of passengers across key variables like gender, age, and passenger class. The interactivity feature around double clicking on passengers travelling together (having the same ticket number) helps the reader identify the relations between the co-travelers (parent-child, spouse, siblings, matrons, etc.) and make assumptions on why some people survived and others didn't. The visualization can be viewed [here](http://bl.ocks.org/aragorn87/raw/03e01fd46d488015ba072fda0476690b/)

# Key Themes

The visual aids the reader to quickly identify the key criterion which had an implied relation with the chances of survival. Gender and Passenger Class have been clearly demarcated to show that 'females' and first class passengers had higher rates of survival. Also, using the interactivity of the visual, one can build a hypotheses on the chances of survival of passengers if they were traveling in a group. (DISCLAIMER: the data is a subset of the total list of passengers and might not be able to capture the trend appropriately for all passengers. However, this is a prototype to help data modelers build hypotheses basis this important variable.)

# Design

The intention of the visual is not to help the reader calculate percentages. Segmentation into genders and passenger classes should help one to get a sense of what the key metrics were. Size of the pixels further gives the information around the age of passengers.

One of the key criteria that might have governed the survivability of passengers is whether the passenger was travelling alone or with co-travellers. Also, who were the co-travellers? Were they friends or family? Parents or siblings? The key premise of this logic is to check if there were any emotional strings present between a group of passengers that might have led to some sort of cohesion (which might have led to the group surviving as a whole or choosing to stay together till the end of their lives)

Some of the key visual encodings:
-  Pixel representation of passengers
-  Age denoted by pixel size
-  Color denotes whether a passenger survived or not
-  Grouping genders together
-  Grouping passengers travelling in the same class together
-  Interactivity - hover over a passenger to check if s/he was travelling solo or with a group (based on ticket number)
-  Interactivity - click on a passenger to check who were the co-travellers (based on name, gender, and age one can deduce almost accurate relationship with the selected passenger)

Some of the feedback receieved from reviewers:
-  Percentages are hard to calculate: The intent was never to help a reader calculate percentages. Therefore added a text above the visual to define the intended use of the visual
-  Difficult to revisit the passenger: Earlier versions did not have the functionality where the clicked on boxes would remain highlighted. Added the functionality to address the issue in a limited capacity
-  What is the purpose of the textbox: Added an explainer text to justify the use of a textbox

# Feedback

Feedback#1:
>  -  I would recommend using the legend to filter under 18s rather than changing square size as a visual encoding. While it's not confusing it does distort the other feature dimension (percentage of deaths versus survivors for each gender/class subset).
>  -  The "clicking on square to reveal more passengers" is not very effective because you can't easily 'return' to a particular data point easily without relying on some guessing. You're almost better off just having a list of the passengers on the screen and colour coding the text to show gender, age and survival status.

Feedback#2:
>  -  What do you notice in the visualization? 
>    This is a visualization on who survived on the Titanic, in a block form, with some organization of the blocks based on sex and class of travel. There is also a typo: Sauce

>  -  What questions do you have about the data? 
>    How was the data obtained? Do you have any links to the source data? Why is the passenger list only partial?

>  -  What relationships do you notice? 
>    I notice that that the passengers are grouped by class of travel and sex. Age is also represented by a smaller box. Colors are used to indicate if they survived. Also, related tickets are highlighted by hovering over them.

Feedback#3:
>  -  What do you think is the main takeaway from this visualization? 
>    The main takeaway is that more females than males survived in each class. For females, livability is directly dependent on class of travel. But, second class males seem to be an exception, i.e. they survived less than males in 3rd class. As a general rule, higher class females have a better chance at survival.

> -  Is there something you don’t understand in the graphic? 
>   The text box that displays details of selected passenger needs to be scrolled down to. Also, how is the name and details of passenger relevant to what you are trying to display? The related tickets also is some information that isn't being used aptly here, in the sense it's not properly represented or easy to access. It's not clear what role relationships play here in who survived(which is the theme of visualization) %age is not represented anywhere/ I can see the role  sex and class of travel on the outcome, but other factors, if important have not been represented.

# Resources
-  The visualization is inspired by Sarah Spijkers' photoshop rendered [visualization](http://sarahspijkers.com/DataVis.jpg) using the same data set

-  Source and description of data: [Kaggle](https://www.kaggle.com/c/titanic/data)

