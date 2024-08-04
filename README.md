# belly-button-challenge
https://robdunnlab.com/projects/belly-button-biodiversity/
Module 14

References for the WH
Bootstrap Official Website: https://getbootstrap.com/
Bootswatch Themes: https://bootswatch.com/
D3.js Official Website: https://d3js.org/
Plotly Official Website: https://plotly.com/
Bootcamp: DATA-PT-EAST-APRIL-041524-MTTH-CONS Xpert Learning Assistant 

This code is a JavaScript script that uses the D3.js library to create an interactive dashboard. The dashboard displays charts and metadata from a JSON file. Here's a simpler explanation of the main functions in the script:

buildMetadata(sample):
Purpose: To display metadata (extra information) about a specific sample.
Process:
Loads data from samples.json using D3.
Filters the metadata for the chosen sample ID.
Selects the HTML element with the ID #sample-metadata and clears any existing content.
Adds the filtered metadata as <h6> elements inside the #sample-metadata panel.
buildCharts(sample):
Purpose: To create visual charts for a specific sample.
Process:
Loads data from samples.json using D3.
Filters the sample data for the chosen sample ID.
Extracts data needed for the charts: otu_ids, otu_labels, and sample_values.
Creates a bubble chart and a bar chart using Plotly.
The bubble chart shows bacteria cultures per sample.
The bar chart shows the top 10 bacteria cultures found.
init():
Purpose: To set up the dashboard when the page loads.
Process:
Loads data from samples.json using D3.
Initializes a dropdown menu with sample names from the data.
Selects the first sample in the dropdown.
Calls buildCharts(firstSample) and buildMetadata(firstSample) to display the charts and metadata for the first sample.
optionChanged(newSample):
Purpose: To update the dashboard when a new sample is selected from the dropdown menu.
Process:
Rebuilds the charts and metadata for the newly selected sample using buildCharts(newSample) and buildMetadata(newSample).
Initialize the dashboard:
Start: The script begins by calling init() to set up the initial dashboard with the data from the first sample.
Summary
Overall, this script updates the charts and metadata dynamically based on the selected sample from the dropdown menu, creating an interactive dashboard for exploring the data.

