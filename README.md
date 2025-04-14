# WHO-Covid19-Data-Preprocessing

## Project Overview
This project involves cleaning and preprocessing a real-world COVID-19 dataset to handle missing values, remove duplicates, and ensure consistency. After cleaning the dataset, several visualizations were created to gain insights into global COVID-19 trends.

## Dataset
The dataset used in this project is taken from WHO's COVID-19 Dashboard, which can be found at https://data.who.int/dashboards/covid19/data?n=c

## Key Insights

### Data Cleaning & Preprocessing
1. **Handle Missing Values**: 
   - Filled missing values in columns like `New_cases` and `New_deaths` with `0`, as missing values could indicate no new cases or deaths reported on that day.
   - For columns like `Country_code` and `WHO_region`, kept the null values as they are, as filling them could introduce inaccuracies.

2. **Consistency Checks**:
   - Ensured that `Date_reported` was correctly formatted as a datetime column.

3. **Data Aggregation**:
   - Aggregated data to ensure that `Cumulative_cases` and `Cumulative_deaths` were the maximum values for each country and date.

### Visualizations Created

1. **Overall Cumulative COVID-19 Cases & Deaths Over Time**: 
   - A time series plot displaying the global cumulative cases and deaths over time.

2. **Top Cumulative Cases by WHO Region**:
   - A bar plot showing the regions with the highest cumulative COVID-19 cases.

3. **Top Cumulative Deaths by Country**:
   - A bar plot highlighting the countries with the highest cumulative COVID-19 deaths.

### Tools and Libraries Used
- **Pandas**
- **Matplotlib**
- **Seaborn**
- **Google Colab**
