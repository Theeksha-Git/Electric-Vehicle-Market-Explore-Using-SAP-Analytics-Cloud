
# Electric Vehicle Market Analysis Dashboard

## SAP Analytics Cloud

### Problem Statement
This dashboard provides a clear view of the electric vehicle market, helping to understand its size, growth, and adoption trends. It highlights technological advancements through average electric range and shows the market share of BEVs and PHEVs.  

By analyzing popular brands, models, and the impact of incentives, it offers insights into consumer preferences and factors driving EV adoption. This helps stakeholders identify opportunities for improvement and strategies to boost growth in the EV market.

### Steps Followed

#### Step 1: Import the Dataset

Start by importing the dataset in the form of a .csv file into SAP Analytics Cloud (SAC).
In this case, the dataset was imported as an Embedded Dataset.
Embedded Dataset: Data that is imported and transformed directly within a Story, making it available only for that specific Story.
Public Dataset: Data that is available for use across multiple Stories in SAC.

#### Step 2:  Prepare the CSV File

Before importing, ensure your .csv file is formatted correctly:
Data types: Clearly define the data types for each column.
Proper formatting ensures the data is imported correctly and tables function as intended.

#### Step 3: Add Geo-Location for the Dataset

Include geo-location information (such as country, state, or city) in your dataset if it’s relevant for visualizations like maps.
This geo-location data will be helpful when creating a Geo Map in the Story, allowing you to visualize the geographical distribution of the electric vehicles across different regions.


![Dataset](https://github.com/user-attachments/assets/d7110729-faf2-42aa-a8ad-f20c2aa21cb2)


#### Step 4: SAC Dashboard Creation
KPI Requirements and Calculations

Define and add the following KPIs to the dashboard:

##### Total Vehicles

Purpose: Understand the size and growth of the electric vehicle market (BEVs and PHEVs).
Calculation: Count(DOL Vehicle ID).

##### Average Electric Range

Purpose: Gauge the technological advancements and efficiency of electric vehicles.
Calculation: Avg(DOL Vehicle ID).

##### Total BEV Vehicles and % of Total BEV Vehicles

Purpose: Analyze the dominance of Battery Electric Vehicles (BEVs).
Calculation: Create a Restricted Account for BEVs and calculate the percentage relative to total vehicles.

##### Total PHEV Vehicles and % of Total PHEV Vehicles

Purpose: Understand the market share of Plug-in Hybrid Electric Vehicles (PHEVs).
Calculation: Create a Restricted Account for PHEVs and calculate the percentage relative to total vehicles.

![Restricted Cal](https://github.com/user-attachments/assets/52496abb-663d-4ac9-bde9-7ecc4eeefe83)

#### Chart Requirements and Interactions

Add the following visualizations to represent data effectively:

##### Total Vehicles by Model Year (From 2010 Onwards):

Visualization: Line/Area Chart.
Insight: Growth pattern and adoption trends of electric vehicles over the years.

##### Total Vehicles by State:
Visualization: Map Chart.
Insight: Geographical distribution of electric vehicles, identifying regions with higher adoption.

##### Top Total Vehicles by Make:
Visualization: Bar Chart.
Insight: Top manufacturers and their market dominance.

##### Total Vehicles by CAFV Eligibility:
Visualization: Pie/Donut Chart.
Insight: Impact of Clean Alternative Fuel Vehicle (CAFV) incentives on adoption.

##### Total Vehicles by Model:
Visualization: Grid View.
Insight: Consumer preferences and popular electric vehicle models.

#### Additional Features

##### Widget Filters: Filter vehicles registered from 2010 onwards.

![Widget Filter](https://github.com/user-attachments/assets/e9f88e92-36c7-407b-b3a9-8cc226a0b88d)
##### Sorting: Display manufacturers with the highest number of vehicles at the top.
##### Input Controls: Add dynamic filters for CAFV eligibility, EV type, model, and state. Set these to interact with all widgets.
##### Linked Analysis: Enable dynamic interactions between the widgets (e.g., Bar Chart and Donut Chart) based on user selections.
##### Styling: Apply appropriate formatting and styling for a visually appealing and professional dashboard.

![Dashboard](https://github.com/user-attachments/assets/b692ea88-c9c0-4314-815e-9fa558f5ed99)
