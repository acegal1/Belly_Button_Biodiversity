# Belly_Button_Biodiversity

Link for interactive dashboard: https://acegal1.github.io/Belly_Button_Biodiversity/ 

# Overview of Project

Project displays the relationship between data analytics and visualization. From Bacteria to Beef is what the company Imporable Beef hopes to accomplish. 
A biological researcher named Rosa needs to visualize and creates a Dashboard of the bacterial data collected from volunteers. Each volunteer should be able to identify the top 10 bacterial species in their belly buttons. That way, if Improbable Beef identifies a species as a candidate to manufacture synthetic beef, Roza's volunteers will be able to identify whether that species is found in their navel.

# Resources

VS Code, Plotly, Bootstrap, Javascript, Html, D3

# Results


1. Drop down and Demographics panel: The first step was to add all the IDs to the “Test Subject ID No” dropdown so that the user can select which ID they would like to look at and so we can use that ID to parse out the information that we need from our data json file. I then use the ID to filter out the metadata pertaining to the selected ID and stored it in an object. I then used d3 to select the panel-body class in my index.html where I used a forEach statement to iterate through the object and append the data to the demographics panel.

![dash](https://github.com/acegal1/Belly_Button_Biodiversity/blob/main/images/dash.png)


2. Horizontal bar chart and Bubble Chart: To create the horizontal chart, I first filtered the JSON data by the current ID that the user has selected. I then created a trace for the chart with the top 10 sample values as the x and the OTU IDs as the y. I then used Plotly to create the bar chart. I followed the same steps above to create the bubble chart.

![Bar graph](https://github.com/acegal1/Belly_Button_Biodiversity/blob/main/images/bargraph.png)
![bubble chart](https://github.com/acegal1/Belly_Button_Biodiversity/blob/main/images/bubblechart.png)

3. Gauge chart: To create the gauge chart, I first created my pie chart which would have the gradient colors and labels from lowest to highest frequency washings per week. I then proceeded to create my needle by created several SVG paths that would draw the needle and that correlate with the washing frequency of a subject. I then created a function that would use a switch statement to select the correct path drawing for the needle depending on the number of washing frequency. 

![guage chart](https://github.com/acegal1/Belly_Button_Biodiversity/blob/main/images/gauge.png)

4. Update all of the plots any time that a new sample is selected: Added an image to the jumbotron,background color , a variety of compatible colors to the webpage,
customized font with contrast for the colors,
Added more information about the project as a paragraph on the page.

Picture of final site:

![full website](https://github.com/acegal1/Belly_Button_Biodiversity/blob/main/images/website.png)

# Summary

The study reveals that a small handful of microbial species, operational taxonomic units, or OTUs, were present in more than 70% of people, while the rest were relatively rare.