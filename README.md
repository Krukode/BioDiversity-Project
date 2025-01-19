​Biodiversity Analysis Project
Overview
This project involves analyzing biodiversity data from the National Parks Service to uncover insights about various species and their conservation status. The data is inspired by real biodiversity data but is fictionalized for analysis. This project uses Python libraries like Pandas, NumPy, Matplotlib, and Seaborn for data cleaning, analysis, and visualization.
Key Questions
What is the distribution of conservation status for species?
Are certain types of species more likely to be endangered?
Which animal is most prevalent, and what is their distribution among parks?

Dataset Description
species_info.csv
Contains information about various species observed in national parks:
category: Taxonomy category of each species (e.g., Mammal, Bird).
scientific_name: Scientific name of the species.
common_names: Common names of the species.
conservation_status: Status indicating if the species is endangered or of concern.
observations.csv
Contains observations of species in national parks:
scientific_name: Scientific name of the observed species.
park_name: National park where the species was observed.
observations: Number of observations recorded in the past 7 days.

Methodology
Data Cleaning
Replaced missing values in the conservation_status column with "No Intervention."
Dropped duplicate records in the observations dataset.
Verified data integrity, including unique categories, species, and park names.
Analysis and Visualizations
1. Distribution of Conservation Status for Species
Excluded species with "No Intervention" status.
Visualized the distribution of conservation status using a stacked bar plot.
2. Endangered Species Analysis
Created a new column, is_endangered, to identify endangered species.
Calculated the proportion of endangered species in each category.
Visualized the results using a bar plot.
3. Most Prevalent Animal and Its Distribution Among Parks
Identified the most prevalent species based on total observations.
Analyzed and visualized the distribution of the most prevalent species across parks.

Key Findings
Conservation Status Distribution:
"Species of Concern" is the largest category, followed by "Endangered," "Threatened," and "In Recovery."
Endangered Species:
Mammals and Fish have the highest proportion of endangered species, indicating they need the most conservation efforts.
Most Prevalent Animal:
The most prevalent species is Castor canadensis (beaver), and its observations vary significantly across parks due to differences in habitat and park size.

Visualizations
Species Count per Category: A bar plot showing the number of species in each taxonomy category.
Conservation Status Distribution: A stacked bar plot visualizing the count of species under different conservation statuses.
Proportion of Endangered Species by Category: A bar plot showing which categories have the highest proportion of endangered species.
Observations by Park: Bar plots and a pie chart visualizing the total observations and park sizes.
Distribution of Most Prevalent Species Across Parks: A bar plot showing how Castor canadensis is distributed across various national parks.

Tools and Technologies
Programming Language: Python
Libraries: Pandas, NumPy, Matplotlib, Seaborn
Visualization Tools: Matplotlib and Seaborn for creating detailed plots and charts

Conclusion
National Parks host a diverse range of species, with a significant number falling under "Species of Concern."
Mammals and Fish require targeted conservation efforts due to their high proportion of endangered species.
Park size and habitat diversity influence the prevalence and distribution of species like Castor canadensis.

Future Enhancements
Integrate additional datasets, such as climate or habitat conditions, for deeper insights.
Use advanced modeling techniques to predict conservation trends.
Create interactive dashboards using tools like Tableau or Power BI for dynamic exploration of the data.

How to Run the Project
Clone the repository and navigate to the project directory.
Ensure the required libraries (Pandas, NumPy, Matplotlib, Seaborn) are installed.
Run the Jupyter Notebook or Python script to execute the analysis and generate visualizations.
View the generated plots and findings in the output folder.

Acknowledgments
The datasets used in this project are inspired by the National Parks Service and adapted for educational purposes. Special thanks to the open-source Python community for providing robust libraries for data analysis and visualization.
