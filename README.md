## Project Title: Evaluation of Organizational Accessibility and Characteristics
## Project Overview:
- To analyze the distribution of hospitals by geographycal regions such as city, county and post code
- To Use Latitude and Longitude to map the organizations and identify spatial patterns or clusters.
- To identify regional concentration and coverage by different Organisation Types and Sectors.
- To Visualize and analyze the network of organizations and their parent-child connections.
- We also need to analyze the variation within Organisation Types and Sub Types to identify prevalent categories.
- To Evaluate the proportion and characteristics of organizations managed by PIMS (IsPimsManaged).
- To identify the current operational status (OrganisationStatus) of organizations to identify active versus inactive entities.

## Data Sources:
The data used in this project comes from a CSV file containing detailed information about various organizations. The key variables in the dataset include:

OrganisationID
OrganisationCode
OrganisationType
SubType
Sector
OrganisationStatus
IsPimsManaged
OrganisationName
Address1, Address2, Address3, City, County, Postcode
Latitude, Longitude
ParentODSCode, ParentName
Phone, Email, Website, Fax
Tools Used:
Python: The primary programming language used for data analysis and visualization.
Pandas: For data manipulation and analysis.
Seaborn: For data visualization.
Matplotlib: For creating plots and charts.
Pyvis: For network visualization.

## Data Cleaning:
The data cleaning process involved the following steps:

- Loading the Data: The dataset was loaded into a pandas DataFrame with UTF-8 encoding to handle special characters.
- Handling Missing Values: Rows with missing values in critical columns (e.g., ParentName) were dropped.
- Data Type Conversion: Ensured that relevant columns were treated as strings to avoid issues during analysis.
- Completeness Check: Added a new column to evaluate the completeness of contact information (Phone, Email, Website, Fax).

## Exploratory Data Analysis:
- Distribution of Organisation Types and Sub Types: Analyzed the variation within Organisation Type and Sub Type to identify prevalent categories.
- Operational Status: Evaluated the current operational status (OrganisationStatus) of organizations to identify active versus inactive entities.
- PIMS Management: identify the proportion and characteristics of organizations managed by PIMS (IsPimsManaged).
- Contact Information Completeness: Evaluated the accessibility of organizations based on the completeness of their contact information.

## Results and Findings:
### Organisation Types and Sub Types:

The analysis revealed that certain Organisation Types and Sub Types were more prevalent.
Visualizations showed the distribution of these categories, highlighting the dominant types and subtypes.

### Operational Status:

The majority of organizations were found to be active, with a smaller proportion being inactive.
Bar plots and pie charts provided a clear picture of the operational status distribution.

### PIMS Management:

The analysis showed the proportion of organizations managed by PIMS and highlighted the characteristics of these organizations.
Visualizations illustrated the distribution of Organisation Type, Sector, and Organisation Status among PIMS-managed and non-PIMS-managed organizations.

## Recommendations:

### Active Status Maintenance:

Regular updates and audits should be conducted to maintain the accuracy of the operational status of organizations.

### Enhanced Data Collection:

Future data collection efforts should focus on capturing more detailed and consistent information across all relevant fields.

## Limitations:
- Data Completeness: The dataset had some missing values which may affect the accuracy of the analysis.
- Data Recency: The dataset's recency is unknown, and the status of some organizations may have changed since the data was collected.
- Limited Variables: The analysis was limited to the variables provided in the dataset. Additional variables could provide more insights.

References:

Pandas Documentation: https://pandas.pydata.org/pandas-docs/stable/

Seaborn Documentation: https://seaborn.pydata.org/

Matplotlib Documentation: https://matplotlib.org/stable/contents.html

Pyvis Documentation: https://pyvis.readthedocs.io/en/latest/

This documentation provides an overview of the project, detailing the steps taken from data loading and cleaning to analysis and visualization, along with the key findings and recommendations based on the analysis.
