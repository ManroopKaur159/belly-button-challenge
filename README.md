Belly Button Biodiversity Dashboard
This assignment is an interactive dashboard that visualizes data from the Belly Button Biodiversity study dataset. 
It allows users to catalogs the microbes that colonize human navels.
The assignment was built using D3.js and Plotly.js to create dynamic, interactive visualizations.

# Steps followed for this assignment-
1. Load Data Using D3- We used the D3 library to read in the data from a provided JSON file, which contains information required in this assignment.
- The data was fetched from the URL:https://static.bc-edx.com/data/dl-1-2/m14/lms/starter/samples.json

2. Create a Horizontal Bar Chart- A horizontal bar chart was created to display the Top 10 OTUs (Operational Taxonomic Units) found in a selected individual.
In this bar chart the following specifications were made-
- `sample_values` was used as the values for the bar chart (x-axis).
- `otu_ids` was used as the labels for the bar chart (y-axis).
- `otu_labels` was used as the hover text for the bar chart.

A dropdown menu was implemented, allowing the user to select a test subject ID.

3. Create a Bubble Chart- A bubble chart was created to display each sample's OTUs.
This chart provides a visual representation of all OTUs found in the selected individual.

In this bubble chart the following specifications were made-
- `otu_ids` were used for the x-axis values.
- `sample_values` were used for the y-axis values and the marker size.
- `otu_ids` were used to determine the marker colors.
- `otu_labels` were used for the hover text.

4. Display Demographic Information
The selected test subject's metadata (demographic information) was displayed dynamically.
This included details such as age, gender, ethnicity, and location.

- The data was fetched from the `metadata` field in the JSON.
- We looped through each key-value pair from the metadata and created text strings to display in the demographic info panel.

5. Dynamic Updates on Sample Change-All the charts (bar chart, bubble chart) and demographic information were dynamically updated whenever the user selected a new test subject from the dropdown menu.
The `optionChanged()` function was implemented to trigger updates to all charts and panels whenever a new sample was selected.

6. Deployment- The app was deployed using GitHub Pages for easy accessibility:
GitHub Pages- Deployment URL: https://manroopkaur159.github.io/belly-button-challenge/
Visit the link to see the live version of the dashboard.

7. Open the index.html file in your browser- open index.html
   
### Technologies Used

- D3.js: To fetch and manipulate the data.
- Plotly.js: To create the interactive bar and bubble charts.
- HTML: To structure and style the dashboard.
- GitHub Pages: For deployment of the static site.




