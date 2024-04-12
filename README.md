# road-accident-analytics

## Introduction

The Excel project aims to analyze and visualize casualty data to enhance understanding and decision-making in road safety management. Leveraging Microsoft Excel's powerful features, the project encompasses a comprehensive approach to exploring and interpreting casualty data.

## Requirement

The client aims to create a Road Accident Dashboard for the years 2021 and 2022 to gain insights into the following requirements:

### Primary KPI
- Total casualties occurring after accidents.

### Primary KPIs
- Total casualties and percentage of total with respect to accident severity.
- Maximum casualties by type of vehicle.

### Secondary KPIs
- Total casualties with respect to vehicle type.
- Monthly trend comparison of casualties for the current year and previous year.
- Maximum casualties by road type.
- Distribution of total casualties by road surface.
- Relation between casualties by area/location by day/night.

## Stakeholders
- Ministry of Transport
- Road Accident Department
- Police Force
- Emergency Services Department
- Road Safety Corps
- Transport Operators
- Traffic Management Agencies
- Public
- Media

## Column details

- Accident_Index: Unique identifier for each accident.
- Accident Date: Date of the accident.
- Day_of_Week: Day of the week when the accident occurred.
- Junction_Control: Type of junction control at the accident location.
- Junction_Detail: Detailed description of the junction where the accident occurred.
- Accident_Severity: Severity level of the accident.
- Latitude: Latitude coordinate of the accident location.
- Light_Conditions: Lighting conditions at the time of the accident.
- Local_Authority_(District): Local authority district where the accident occurred.
- Carriageway_Hazards: Hazards present on the carriageway at the time of the accident.
- Longitude: Longitude coordinate of the accident location.
- Number_of_Casualties: Number of casualties involved in the accident.
- Number_of_Vehicles: Number of vehicles involved in the accident.
- Police_Force: Police force attending the accident.
- Road_Surface_Conditions: Surface conditions of the road at the time of the accident.
- Road_Type: Type of road where the accident occurred.
- Speed_limit: Speed limit on the road where the accident occurred.
- Time: Time of the accident.
- Urban_or_Rural_Area: Classification of the accident location as urban or rural.
- Weather_Conditions: Weather conditions at the time of the accident.
- Vehicle_Type: Type of vehicle involved in the accident.

## Data Cleaning

- Check all columns for appropriate size and space.
- Verify values in each column.
- Remove blanks, duplicates, and typo errors.

## Data Processing

To facilitate data analysis, several steps were taken:

- **Month Extraction**: A new column was added to extract the month from the accident date. This was achieved by right-clicking on the "Day_of_Week" column, selecting "Insert," and then dragging the formula down to cover all rows. The formula used was `=TEXT(B2, "mmm")`, where B2 represents the Accident_Date value.

- **Year Extraction**: Similar to the month extraction process, another column was added to extract the year from the accident date using the formula `=TEXT(B2, "YYYY")`, where B2 represents the Accident_Date value.

## Data Analysis and Visualization

To analyze and visualize the data effectively, the following steps were taken:

- **Pivot Table Creation**: Pivot tables were utilized to analyze the data. By inserting a pivot table and selecting the number of casualties, the total number of casualties was generated.

- **Visual Representation**: Visuals such as pie charts, donut charts, bar charts, and line charts were created to represent the analyzed data. These visuals were copied and pasted onto the same sheet for convenience.

- **Customization**: Various customization options were applied to enhance the clarity and aesthetics of the visuals. This included formatting shapes, changing chart styles, adding background colors, and adjusting chart properties.

- **Timeline Visualization**: An "Accident_Data" timeline was added to visualize the changing accident dates over time. This involved selecting a shell in the pivot table, going to "Analyze Pivot Table," and selecting "Accident Date."

- **Vehicle Type Analysis**: A pivot table was generated to visualize vehicle type-wise casualties. Calculated items were used to create categories such as cars, vans, bikes, buses, etc., and corresponding visuals were created.

- **Yearly Comparison**: Pivot tables were created for each year separately (2021 and 2022), and a comparison of casualties was visualized using line charts.

- **Road Type Analysis**: Another pivot table was generated to analyze casualties by road type. This data was visualized using bar charts, with customization applied for better visual representation.

- **Road Condition Analysis**: A pivot table was created to analyze casualties by road surface conditions. This data was visualized using a TreeMap, with appropriate customization.

- **Light Condition Analysis**: Casualties were analyzed based on light conditions using calculated items to group them into light and dark conditions. This data was visualized using donut charts, with data label values formatted for clarity.

- **Rural vs Urban Analysis**: A slicer was generated to include rural and urban categories. Another visual was created to include accident date using a timeline. Custom styles were applied to both visuals for better aesthetics.

- **Yearly Comparison**: Pivot tables were created for each year, months and quarters, and a comparison of casualties was visualized using line charts.

- **Connection with Other Pivot Tables**: All other pivot tables were connected by right-clicking on the visuals and selecting the appropriate options.

## Conclusion

Overall, the process facilitated a thorough exploration of casualty data, enabling stakeholders to gain valuable insights into factors influencing road accidents and casualties. The combination of slicers, pivot tables, and visualizations provided a comprehensive analysis framework, enhancing decision-making and strategy formulation in road safety management.

