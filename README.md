# Accident Data Analysis

## 1.0 Introduction
This report analyzes detailed records of road traffic accidents from 2020, focusing on vehicle, casualty, and geographic details. The aim is to identify patterns and factors contributing to accidents to support the creation of targeted safety measures.

## 2.0 Data Cleaning and Preparation
The dataset for the year 2020 was retrieved from various tables and merged into a new dataframe with 86 columns and over 220,434 rows. After cleaning, 36 columns were selected based on their relevance to the study's goals, as detailed in Table 1.

### Table 1: Selected Columns for Analysis
| Category                      | Data Fields                                            | Justification                                     |
|-------------------------------|--------------------------------------------------------|---------------------------------------------------|
| Time Analysis                 | date, time, day_of_week                                | Patterns in accident occurrence                   |
| Spatial Analysis              | longitude, latitude, lsoa_of_accident_location         | Pinpointing accident hotspots                     |
| Severity Analysis             | accident_severity, weather_conditions                  | Influencing factors on accident severity          |
| Demographic Analysis          | sex_of_driver, age_of_driver                           | Demographic patterns related to accidents         |
| Traffic and Infrastructure    | number_of_vehicles, road_type                          | Understanding traffic flow and infrastructure     |
| Pedestrian Analysis           | pedestrian_movement                                    | Assessing pedestrian safety at accident sites     |
| Vehicle and Casualty Profile  | vehicle_type, engine_capacity_cc                       | Insights on vehicle types involved in accidents   |
| Urban vs Rural Analysis       | urban_or_rural_area                                    | Accident trends in different environments         |

Data preprocessing involved handling missing values, categorizing data, and addressing outliers with the Interquartile Range (IQR) method.

## 3.0 Accident Demography
Analysis included demographic review through visualizations, providing insights into driver and casualty ages, and the geographic spread of incidents. Key findings were the high involvement of middle-aged individuals in accidents and significant accident hotspots in urban areas like London, Manchester, and Birmingham.

## 4.0 Outlier Detection
Outliers were identified but retained in the dataset to preserve potentially significant patterns.

### Table 2: Outliers in Data
| Columns               | Outliers Identified | Upper Boundary |
|-----------------------|---------------------|----------------|
| number_of_vehicles    | 74,763              | 2.0            |
| number_of_casualties  | 17,685              | 3.5            |
| age_of_vehicle        | 2,617               | 20.0           |

## 5.0 Analysis
The study included various analyses such as the distribution of accidents by time, day, and under different environmental conditions. Peak accident times were identified during morning and late afternoon hours, with Fridays showing a higher incidence rate.

## 6.0 Predictive Modeling
Advanced predictive models were developed to forecast fatal accidents, enhancing the ability to implement preemptive road safety measures.

## 7.0 Conclusion
Insights from this analysis are intended to aid governmental and related agencies in crafting effective and timely road safety strategies.

## 8.0 References
- Hiary, H., et al. (2018). "Flower classification using deep convolutional neural networks." *IET Computer Vision*, 12(6), 855-862.
- Singh, A., & Singh, P. (2020). "Image Classification: A Survey." *Journal of Informatics Electrical and Electronics Engineering*, 1(2), 1-9.

## Figures
- Figure 1: Histogram showcasing the baseline model performance.
- Figure 2 to Figure 6: Various visualizations depicting accident trends and demographic distributions.

## Appendices
- Appendix A: Code snippets and methodologies used for data cleaning and analysis.
- Appendix B: Additional tables and figures supporting detailed analysis.
