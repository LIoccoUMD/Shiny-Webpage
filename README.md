# Project 2: Hurricane Data Analysis

## Overview
This project explores the dynamics of hurricane impacts over time, leveraging the `hurricNamed.csv` dataset to analyze patterns in hurricane frequency, severity, and consequences. The analysis focuses on:

- **Economic Impact:** Assessing damage in 2014 USD and identifying influencing factors.
- **Mortality Patterns:** Correlating hurricane intensity (wind speed, pressure) with death tolls.
- **Geographical Trends:** Mapping hurricane activity across U.S. states.
- **Gender of Hurricane Names:** Investigating if naming conventions affect perceived or actual severity.

## Key Components

### Data
- **Dataset:** `hurricNamed.csv`
- **Variables:** 
  - **LF.WindsMPH** (Maximum Wind Speed at Landfall in MPH)
  - **LF.PressureMB** (Lowest Pressure at Landfall in MB)
  - **deaths** (Number of deaths caused by the hurricane)
  - **BaseDam2014** (Economic damage adjusted to 2014 USD)
  - **Year** (Year of hurricane occurrence)
  - **AffectedStates** (States affected by the hurricane)
  - **mf** (Gender of the hurricane name)

### Analysis Tools
- **R** with libraries:
  - `shiny` for interactive web applications
  - `ggplot2` for static and dynamic plotting
  - `dplyr`, `tidyr` for data manipulation
  - `plotly` for interactive plots
  - `maps` for geospatial visualizations

### Project Structure

#### Shiny Application
- **UI:** 
  - Overview filters for variable selection.
  - Tabs for different analysis types:
    - **Scatter Plot** for examining relationships between hurricane metrics.
    - **Trends Over Time** to visualize changes in hurricane characteristics.
    - **Insights** for deep dives into economic impacts.
    - **Correlation Heatmap** to identify variable interrelations.
    - **Geospatial Map** showcasing hurricane distribution by state.

- **Server:** 
  - Reactive computations for dynamic data visualization.
  - Custom functions for data processing and visualization.

#### Static Visualizations
- **Wind Speed vs. Deaths:** Scatter plot to visualize the impact of wind speed on mortality.
- **Pressure vs. Deaths:** Similar analysis but with pressure as the variable.
- **Hurricane Frequency by State:** Bar chart showing hurricane counts over years for top states.
- **Economic Damage Distribution:** Frequency polygon to understand damage spread across states.
- **Trends Over Time:** Faceted plot showing multiple hurricane metrics' evolution.
- **Impact of Hurricane Name Gender:** Violin and Box plots to assess if hurricane name gender correlates with damage.

## How to Use

### Running the Shiny App
- Ensure you have R and RStudio installed.
- Install required packages with:
  ```r
  install.packages(c("shiny", "ggplot2", "dplyr", "tidyr", "plotly", "maps"))

### Viewing Static Visualizations
- Open the Rmd file in RStudio and knit it to generate an HTML document with all visualizations.
