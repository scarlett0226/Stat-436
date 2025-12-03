Stat 436 HW2


Dataset description
The dataset I used this time is the US Wildfire Dataset (2014-2025) - 9.5 Million Spatiotemporal Wildfire Forecasting Data (GRIDMET+IRWIN), from Kaggle by Shaurya Mathu, Shreyas Bellary Manjunath, and Alina Vereshchaka. The dataset contains wildfire events across the continental U.S.


Data cleaning
Since I wanted to study real-world wildfire events, I filtered and retained 502,000 real-world events. After verifying that the entire dataset contained no missing values, I calculated year, month, and season values ​​based on the time variable. I then grouped these events into specific states based on latitude and longitude, creating new columns. This completed my data preparation. Each row represents a real-world wildfire event between 2014 and 2025, including key information such as season, location, and average solar radiation. The variables I primarily used were season, year, state, location (latitude/longitude), and solar radiation(W/m2).

Main question
This visualization is meant to explore the relationship between wildfire distribution, solar radiation, and seasons across different regions of the United States.
The target audience includes climatologists, environmental policy researchers, conservationists, and the general public interested in wildfire trends.

Intervative elements
I designed two pages, one is Overview and the other is State Explorer.
Both pages allow filtering by season and solar radiation through a dropdown and a slider. The US map on the right shows how these two factors influence the distribution of wildfires. Furthermore, I've added an additional Brushing interaction to the year histogram. The x-axis of this graph plots the years 2014-2025, while the y-axis shows the number of wildfires each year. Users can intuitively see the number of wildfires each year through the histogram itself, or add the additional year factor to observe changes in the number and distribution of wildfires.
On the State Explorer page, users can see detailed information about each state. They can select a state of interest, and a map of that state will appear on the right, along with filtered wildfire locations. Similarly, users can filter by solar radiation or seasonality to see wildfire distribution during different periods and conditions.
I chose year, season, state, and solar radiation because year can help users visualize wildfire trends over the past 10 years, and combined with a map, it can also help users understand regional trends. I chose the season because this dataset contains a lot of detailed weather information, such as temperature, humidity, and other climate information during wildfires. However, too many variables would make the interactive map too complex and difficult for users to identify trends. Therefore, I used season, a more general variable, to try to summarize information from a specific time period with similar climate characteristics. The United States is very large, and climate conditions vary significantly between states. To help users better understand the states they are interested in, or those who want to track specific locations where wildfires have occurred, I created the State Explorer page. I believe that solar radiation, a variable with a strong periodic pattern that combines location and time, combined with this filter, can better help users understand wildfire trends.

Style & layout

I used a relatively simple style, with a white background and black/green text guides. In order to highlight the two separable pages, I used green, while keeping other colors simple. Sliders and histograms use a uniform blue tone, with brief interaction notes below the title. In the main view, whether it is the US map in the Overview or the state map in the State Exporter, a light gray background is used, and each event point is gradiently colored from low to high by Solar Radiation. The color of the point is also yellow/red, corresponding to the Wildfire theme, which facilitates hierarchical search while maintaining visual neatness.

Unexpecting finding

Except for incomplete 2025 data, wildfire counts have steadily increased year by year.
In addition to California, Florida also has a high number of wildfires, especially in winter when there are fewer wildfires in the north. Florida is the only state with a winter fire and a solar radiation of 250 (W/m2) or more.
Wildfire can still occur even when the Solar Radiation is less than 5.
I focused on the situation in Wisconsin and found that the peak season for wildfires in Wisconsin is spring, followed by winter, rather than summer, when the solar radiation is the highest. This shows that, in addition to solar radiation, humidity may also be an important factor in inducing wildfires.












