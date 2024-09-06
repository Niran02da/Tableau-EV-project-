# EV-Dashboard

### Dashboard Link : https://public.tableau.com/views/EVAnalysisProject/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

## Problem Statement
####  KPI’S Requirement

-  Total Vehicles:
Understand the overall landscape of electric vehicles, encompassing both BEVs and PHEVs, to assess the market's size and growth.
-  Average Electric Range:
Determine the average electric range of the electric vehicles in the dataset to gauge the technological advancements and efficiency of the EVs.
- Total BEV Vehicles and % of Total BEV Vehicles:
Identify and analyze the total number of Battery Electric Vehicles (BEVs) in the dataset.
Calculate the percentage of BEVs relative to the total number of electric vehicles, providing insights into the dominance of fully electric models.
- Total PHEV Vehicles and % of Total PHEV Vehicles:
Identify and analyze the total number of Plug-in Hybrid Electric Vehicles (PHEVs) in the dataset.
Calculate the percentage of PHEVs relative to the total number of electric vehicles, offering insights into the market share of plug-in hybrid models.

#### Charts Requirement
- Total Vehicles by Model Year (From 2010 Onwards):
Visualization: Line/ Area Chart
Description: This chart will illustrate the distribution of electric vehicles over the years, starting from 2010, providing insights into the growth pattern and adoption trends.
- Total Vehicles by State:
Visualization: Map Chart 
Description: This chart will showcase the geographical distribution of electric vehicles across different states, allowing for the identification of regions with higher adoption rates.
- Top 10 Total Vehicles by Make:
Visualization: Bar Chart 
Description: Highlight the top 10 electric vehicle manufacturers based on the total number of vehicles, providing insights into the market dominance of specific brands.
- Total Vehicles by CAFV Eligibility:
Visualization: Pie Chart or Donut Chart
Description: Illustrate the proportion of electric vehicles that are eligible for Clean Alternative Fuel Vehicle (CAFV) incentives, aiding in understanding the impact of incentives on vehicle adoption.
- Top 10 Total Vehicles by Model:
Visualization: Tree map
Description: Highlight the top 10 electric vehicle models based on the total number of vehicles, offering insights into consumer preferences and popular models in the market.




### Overview

The Electric Vehicle (EV) Data Analysis Project is a comprehensive dashboard providing detailed insights into the state of electric vehicle adoption. It examines various dimensions, including vehicle models, manufacturers, state-wise adoption, and the distribution between Battery Electric Vehicles (BEVs) and Plug-in Hybrid Electric Vehicles (PHEVs). This README serves as a guide to the key components of the dashboard, helping users navigate through the data and insights presented.

### Steps followed 
#### Header Section: Electric Vehicle Data Analysis
The header contains the title of the project:

Title: "Electric Vehicle Data Analysis" (Displayed at the top of the dashboard).
#### Key Summary Metrics
This section provides a quick reference to the core metrics of the data analyzed:

- Avg Electric Range: Displays the average electric range for vehicles in the dataset, marked as 67.83 miles. This gives a reference point for the typical driving range of EVs in the dataset.
- Total Vehicles: The total number of electric vehicles in the analysis, listed as 150,413 vehicles.
- Total BEV Vehicles: The number of Battery Electric Vehicles (BEVs) in the data, shown as 116,745 vehicles, representing 77.6% of the total.
- Total PHEV Vehicles: The number of Plug-in Hybrid Electric Vehicles (PHEVs), shown as 33,668 vehicles, representing 22.4% of the total.

Snap of Total vehicle,

![Screenshot_20240906_122124](https://github.com/user-attachments/assets/0cb24245-fd31-49b5-8355-91934eb56445)

Following calculation  was written for the Total vehicle ,
        
        
        COUNTD([DOL Vehicle ID])
)

Snap of Average Electric Range,

![Screenshot_20240906_122116](https://github.com/user-attachments/assets/424b60ca-3205-458f-a270-9cc17874addd)

Following calculation  was written for the Average Electric Range ,
        
        AVG([Electric Range])
        



Snap of Total BEV Vehicle,

![Screenshot_20240906_122136](https://github.com/user-attachments/assets/ad0e9ab7-9c44-4cd4-a220-e37e519ca25f)

Following calculation  was written for Total BEV Vehicle ,
        
        COUNTD ( IF [EV Type] = "Battery Electric Vehicle (BEV)" 
        THEN [DOL Vehicle ID]
        END
        
        


Snap of Total PHEV Vehicle,

![Screenshot_20240906_122206](https://github.com/user-attachments/assets/2bac799c-6caf-4bf6-acab-7055926da2db)

Following calculation  was written for Total PHEV Vehicle ,
        
        COUNTD(If [EV Type]= "Plug-in Hybrid Electric Vehicle(PHEV)" THEN[DOL Vehicle ID]END)





#### Total Vehicles by Model Year
- Purpose
This chart illustrates the growth trend of electric vehicles by model year (from 2011 to 2024).

Snap of Total vehicle by Model Year,

![Screenshot_20240906_122223](https://github.com/user-attachments/assets/33531a4a-01e4-453c-8cb2-d46cc29d97e2)


- Description
The area chart is colored in green and shows the number of electric vehicles registered per year.
Noteworthy peaks include:
2023: The highest registration year with 37.1K vehicles.
2018 and 2022: Significant jumps with 14.4K and 27.8K vehicles respectively.
A dotted line represents the average number of vehicles across all years, which is 10.7K.

#### Map: Total Vehicles by State
- Purpose :
This map provides a geographical breakdown of electric vehicle registrations across the United States.

Snap of Total vehicles by State,

![Screenshot_20240906_122236](https://github.com/user-attachments/assets/9429d8b1-9099-43b1-b71a-3fcbf65e9a0f)


- Description
The choropleth map uses shading to depict the number of vehicles registered in each state.
California leads significantly with 150,082 vehicles, while other states show smaller numbers.
Lighter colors indicate lower adoption, with some states registering fewer than 100 vehicles.
#### Bar Chart: Top 10 Total Vehicles by Make
- Purpose
This chart highlights the top 10 vehicle makes (brands) contributing to the total number of electric vehicles.

Snap of Top 10 Total vehiclesby Make,

![Screenshot_20240906_122246](https://github.com/user-attachments/assets/dff44e94-47b1-49ac-a562-ff0429342ebd)

- Description
TESLA is the dominant manufacturer, with 68,939 vehicles making up 52.70% of the total.
Other key brands include Nissan (10.32%), Chevrolet (9.19%), and Ford (5.81%).
#### Bar Chart: Total Vehicles by CAFV Eligibility
- Purpose
This chart categorizes vehicles based on their eligibility for Clean Alternative Fuel Vehicle (CAFV) programs.

Snap of Total vehicles by CAFV Eligibility,

![Screenshot_20240906_122259](https://github.com/user-attachments/assets/0afe0d40-2016-4bf5-869a-2b80edd59183)

- Description
The chart splits the vehicles into CAFV Eligible and CAFV Ineligible categories.
Tesla vehicles make up the largest portion of CAFV Eligible vehicles, indicating a trend toward cleaner vehicle models.
#### Table: Top 10 Total Vehicles by Model

- Purpose
This table displays the most popular vehicle models in the dataset.

Snap of Top 10 Total Vehicle by model,

![Screenshot_20240906_122315](https://github.com/user-attachments/assets/52a1dbe6-35f9-4005-b2ca-5348d7b2849f)

- Description
Tesla Model Y leads with 28,501 vehicles (18.95% of the total), followed by the Tesla Model 3 with 27,179 vehicles (18.07%).
Other popular models include the Nissan Leaf (13,187 vehicles) and Chevrolet Bolt EV (5,732 vehicles).
The table columns display the model, make, EV type (BEV or PHEV), total vehicle count, and the percentage of total vehicles.


        


        
## The report was then published to Tableau public.
 
 
![Screenshot_20240906_125556](https://github.com/user-attachments/assets/71958a96-2c3f-4b14-9c39-9c7ae2710465)

# Snapshot of Dashboard ( Tableau Desktop )

![Screenshot_20240906_125016](https://github.com/user-attachments/assets/85421f0e-f026-4bb5-992f-ae491eb7ca54)

 
# Report Snapshot (Power BI DESKTOP)

 
![Screenshot_20240905_070604](https://github.com/user-attachments/assets/276b4d52-72ae-4823-b438-e336c0cf22e7)

# Key Insights


- Tesla Dominance: Tesla is the clear leader in both the total number of vehicles and the most popular models.
- EV Growth: The total number of electric vehicles has grown steadily over the years, with significant peaks in recent times, particularly in 2022 and 2023.
- Geographic Distribution: EV adoption is heavily concentrated in California, with other states having far fewer registrations.
- CAFV Eligibility: A large portion of vehicles, particularly from Tesla, are eligible for CAFV programs, indicating a move toward cleaner and more eco-friendly vehicles.

### Next Steps for Further Analysis
Here are some recommendations for additional analysis to deepen the understanding of the data:

- State-Wise Growth Trends: Analyze the growth of electric vehicle adoption in each state over time.
- Battery Range Analysis: Study the evolution of battery range across different models and manufacturers.
- Manufacturer Growth Trends: Analyze which manufacturers are increasing or decreasing their market share over time.
- PHEV vs BEV Analysis: Compare the growth trends of Plug-in Hybrid Electric Vehicles (PHEVs) and Battery Electric Vehicles (BEVs).
- Model Year vs CAFV Eligibility: Investigate how Clean Alternative Fuel Vehicle (CAFV) eligibility varies by model year and manufacturer.


## Conclusion
The Electric Vehicle Data Analysis dashboard provides a comprehensive view of the current landscape of electric vehicles, with Tesla being the dominant player. The insights drawn from this data are useful for understanding trends in EV adoption, geographic distribution, and manufacturer market share. Further analysis can provide deeper insights into state-level growth, battery range improvements, and manufacturer-specific trends
