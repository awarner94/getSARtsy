# getSARtsy
NASA Space Apps 2023 Challenge
-
Author: Ashley Nicole Warner

# Motivation

Santa Catalina Island is a small island located about 25 miles off the coast from mainland Southern California. It is home to about 4,000 across its two towns, Avalon and Two Harbors (data from 2010 census), although easily 200 times that amount visit the quaint towns yearly via cruise ships or weekend get aways. The majority of the land on Catalina Island is protected by the Catalina Island Conservancy, uniquely locking the towns' borders to a fixed size. Isolated, the island has to ship in all of it's resources from the mainland. Because of it's unique geographical and geopolitical situation, the island's fresh water only has one source: rain.

The historic droughts of Southern California wreaked havoc on the islanders (my then 90-year-old grandmother was taking sponge baths in the kitchen sink). Residents got strict monthly allowances of daily water usage, likely to offset the lack of conservation efforts of ever increasing tourism. As climate change worsens weather patterns, the residents of Catalina Island live in the constant fear of an imminent water shortage, and with the geographic isolation, this will have dire consequences on not only the residents and their livelyhood, but also on conservation efforts of the island's delicate (and untraditional) ecosystem.

# Goal/Future Goal

For this contribution to NASA's Space Apps Challenge 2023, the goal was to use SAR data to explore vegetation change on the island from 2009 vs 2022. Future goals include plotting the amount of rainfall over a large sum of months/years and project future rainfall trends.

The following are the sources for the data used/planned to be used:

SAR Data: 
1. JPL UAVSAR (https://uavsar.jpl.nasa.gov/cgi-bin/product.pl?jobName=ChanIs_30102_09071_001_090916_L090_CX_01#data, https://uavsar.jpl.nasa.gov/cgi-bin/product.pl?jobName=ChanIs_30104_22054_013_221130_L090_CX_01#data)
Downloaded both geoTIF files and used those in QGIS.

Weather Data: 
1. Socioeconomic Data and Aplications Center (SEDAC) (https://sedac.ciesin.columbia.edu/data/set/sdei-high-res-extreme-heat-estimates-1983-2016)
Tuholske, C., K. Caylor, C. Funk, A. Verdin, S. Sweeney, K. Grace, P. Peterson, and T. Evans. 2021. Global urban population exposure to extreme heat. Proceedings of the National Academy of Sciences, 118(41), e2024792118. https://doi.org/10.1073/pnas.2024792118.

2. Los Angelos Almanac (https://www.laalmanac.com/weather/we133a.php)

# Files

1. Jupyter Notebooks - these are mostly what I used to explore initial data from SEDAC. I had the hopes of plotting temperatures of Avalon, CA but the data from SEDAC only listed information of areas that the humidity index combined with temperature exceeded safe values.
2. Catalina.gqz - QGIS file that uses TIF files from JPL UAVSAR, as well as a rasterized log difference.
4. CatalinaSAR.png - Plain ol' SAR image of Catalina Island circa 2022 😊
5. band1_22to09.png - logarithmic difference of 2022 / 2009 SAR data, band 1 (red band).
6. SAR log2022:2009 Red Band.png - annotated version of "band1_22to09.png"
7. rateOfDays.png - using data from SEDAC, world map showing the average amount of additional days per year an area had a humidity and heat index reach a combined hazardous level, calculating from 1983 to 2016.
8. detailedDescription - detailed thought process behind the project and what happened at each step.
9. Get SARtsy - Catalina Island.pdf - power point of entire project

