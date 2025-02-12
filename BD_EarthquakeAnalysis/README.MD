# Overview

Exploratory Data Analysis (EDA) on earthquake data from Bangladesh (1970-2021). The dataset was collected from IRIS IEB website and contained information on earthquake magnitude, depth, location (longitude & latitude), and time of occurrence.

## Execution Details

### 1. Data Collection & Preprocessing

- Dataset: The dataset was saved and loaded in a CSV file format

- Tools Used:

    - Python for analysis.

    - Pandas & NumPy for data preprocessing and statistical analysis.

    - Seaborn & Matplotlib for data visualization.

- Preprocessing Steps:

    - Checked dataset structure using

    - Filtered relevant data for earthquakes occurring in:

        - BANGLADESH

        - INDIA-BANGLADESH BORDER REGION

        - BAY OF BENGAL

        - MYANMAR-BANGLADESH BORDER REGION

    - Converted timestamps into readable date formats.

    - Focused on earthquakes with magnitude ≥ 3.5 for significant event analysis.

### 2. Data Exploration & Key Visualizations**

**A. Earthquake Magnitude Distribution***

- Graph Used: Histogram of Magnitude (Seaborn displot)

**Findings:**

    - Most earthquakes had a magnitude below 4.0, indicating low to moderate seismic activity.

    - A smaller number of earthquakes had a magnitude above 5.0, which could cause structural damage.

**B. Depth Distribution of Earthquakes**

- Graph Used: Histogram of Depth (Seaborn displot)
**Findings:**

    - Most earthquakes occurred at shallow depths (0-50 km).

    - Deeper earthquakes (more than 100 km) were less frequent.

**C. Geographical Distribution of Earthquakes**

- Graph Used: Scatter Plot of Latitude vs. Longitude with Magnitude (sns.scatterplot)

**Findings:**

    - Earthquakes were concentrated near border regions and coastal areas (Bay of Bengal).

    - Higher magnitude earthquakes (≥4.0) were scattered across multiple regions.

**D. Relationship Between Magnitude and Depth**

- Graph Used: Hexbin Plot (sns.jointplot(kind='hex'))

**Findings:**

    - No strong correlation between magnitude and depth.

    - Some high-magnitude earthquakes occurred at shallow depths, increasing their potential impact.

**E. Monthly & Seasonal Trends of Earthquakes**

- Graphs Used:

    - Bar Plot of Earthquake Count by Month (sns.countplot)

    -  Bar Plot of Magnitude by Month (sns.barplot)

**Findings:**

    - Earthquakes were evenly distributed throughout the year with no significant seasonal trend.

    - Higher magnitude earthquakes (≥4.0) were more frequent in March, May, and October.

**F. Daily Trends of Earthquakes**

- Graphs Used:

    - Bar Plot of Magnitude by Day of the Month

    - Count Plot of Earthquake Frequency by Day

**Findings:**

    - Earthquakes did not show a clear pattern based on days of the month.

    - Some peaks were observed on specific days, but they might be random variations.

**G. Decadal Analysis of Earthquake Trends**

- Graph Used: Count Plot of Earthquake Occurrences by Decade

**Findings:**

    - Increase in recorded earthquakes over time.

    - The 2000-2009 decade had the highest number of earthquakes.

    - This could be due to better monitoring technology rather than an actual increase in earthquakes.

### Key Takeaways

**1. Earthquake Activity in Bangladesh is Moderate:** Most earthquakes have a magnitude below 4.0.

**2. Shallow Earthquakes are More Common:** Most earthquakes occur at depths of 0-50 km, which can have surface-level impacts.

**3. Geographical Risk Areas Identified:** The Bay of Bengal and border regions experience frequent earthquakes. 

**4. Increasing Trend Over Decades:** More earthquakes have been recorded over time, possibly due to better monitoring systems.

