# Analysis of Twitter Hashtag Surrounding the January 6th Capitol Insurrection and the Black Lives Matter Movement

## Summary
There is no denying that 2020 was an eventful year. From the COVID-19 pandemic, to the revival of the Black Lives Matter (BLM) movement and the Presidential election between Joe Biden and Donald Trump, the people of the United States were consistently on edge. While the whole world was stuck at home, mis-information ran wild across the internet and conspiracy theories made their way into the mainstream. The violent rhetoric coming from the White House empowered far right individuals and groups to comit arguably the worst act of domestic terrorism since the country's inception in what we now know as the January 6th Capitol Insurrection. Academics and journalists alike have studied and reported on the significant role that social media played in this context. However, little attention has been put toward the spatial dimension of the use of social media surrounding it. This project aims to close that gap by exploring the spatial distribution of hashtag use in Tweets made across the United States during the peak of the BLM movement in the summer of 2020 and the lead up to January 6th after the November Presidential election. This project has two main objectives.
* Map the spatial distribution of tweets in the United States using four of the most common hashtags related to the Black Lives Matter movement (#blacklivesmatter, #blm, #icantbreathe, #georgefloyd) in key dates of the summer of 2020 (May 26th - 31st) and spring of 2021 (March 8th and 28th).
* Map the spatial distribution of tweets in the United States using three of the most common hashtags related to the January 6th Capitol Insurrection (#stopthesteal, #voterfraud, #electionfraud) in key dates after the 2020 Presidential Election (November 3rd, 7th, 11th, 24th and 30th, December 14th, and January 6th). 

## Approach and Method

#### Data: 
We will be creating our own dataset by scraping tweets using snscrape. Snrcrape is an open source social media scraper that will allow us to extract all tweets using the hashtags we identified as most relevant to the Black Lives Matter movement and the January 6th Capitol Insurrection. This scraper also allows us to set specific date ranges and exclude all tweets in foreign languages. Due to the limited availability of tweets that include information about the location where they were tweeted, we will use the user???s self identified location as a proxy. This metric will give us a better understanding of people???s attitudes toward the Black Lives Matter movement and the January 6th Capitol Insurrection across the country more concretely than taking the locations where they were when they tweeted. We are in the process of cleaning up the available data from non-existent locations and locations outside of the United States.

#### Code:
* Use Snscrape to scrape all tweets that used common hashtags related to the Black Lives Matter movement (#blacklivesmatter, #blm, #icantbreathe, #georgefloyd) in key dates of the summer of 2020 (May 26th - 31st) and spring of 2021 (March 8th and 28th) and those that used the most common hashtags related to the January 6th Capitol Insurrection (#stopthesteal, #voterfraud, #electionfraud) in key dates after the 2020 Presidential Election (November 3rd, 7th, 11th, 24th and 30th, December 14th, and January 6th). 
* Use ggplot2 to make timelines of the dates we are including in our analysis along with the relevant event that prompted us to include it. 
* Since Snscrape is Python based, we will build a script that allows us to clean the data to keep only relevant locations and export it as a csv file automatically. The next stage in the data cleaning process will be manual to make sure we keep as many tweets as possible for increased accuracy.
* Make a Choropleth Map at the state level depicting the spatial distribution of the use of the identified hashtags related to the Black Lives Matter movement for each date.
* Make a Kernel Density Map depicting the spatial distribution of the use of the identified hashtags related to the Black Lives Matter movement for each date. We will use the coordinates of the cities the Users identified as their locations. Not all tweets include mention of the city so the sample size will be smaller than the one used for the Choropleth Map. 
* Make a Choropleth Map at the state level depicting the spatial distribution of the use of the identified hashtags related to the January 6th Capitol Insurrection for each date.
* Make a Kernel Density Map depicting the spatial distribution of the use of the identified hashtags related to the January 6th Capitol Insurrection for each date. We will use the coordinates of the cities the Users identified as their locations. Not all tweets include mention of the city so the sample size will be smaller than the one used for the Choropleth Map. 
* Make an animated gif showing the change in the use of each of the hashtags over time. 

#### Timeline:
* Nov 18th: Select Dates for BLM and Insurrection (Valeria) 
* Nov 22nd: Build Scrapper for BLM and Insurrection (Sadie and Valeria) 
* Nov 23rd: Scrape Tweets for BLM and Insurrection (Sadie and Valeria)
* Nov 26th: Complete Round 1 Data Cleaning (Sadie and Valeria) 
* Nov 28th: Complete Round 2 Data Cleaning (Sadie and Valeria) 
* Nov 30th: Complete Round 3 Data Cleaning (Sadie and Valeria) 
* Dec 3rd: Complete Data Cleaning for BLM and Insurrection (Sadie and Valeria) 
* Dec 6th: Complete Kernel Density Maps for BLM and Insurrection Data (Sadie and Valeria)
* Dec 7th: Complete Chloropleth Maps BLM and Insurrection Data (Sadie and Valeria)
* Dec 9th: Complete Miscellaneous Visualizations (Timeline, Animated Gif, etc) (Sadie and Valeria)
* Dec 12th: Finish Assembling Vignette (Sadie and Valeria) 
Note about the splitting of tasks: Valeria will be making the visualizations for the Capitol Insurection data while Sadie will be making the equivelent visualizations for the Black Lives Matter dataset. 

#### Anticipated outcomes: 
* Greater understanding of the spatial distribution/concentration of digital activity around Black Lives Matter and the Capitol Insurection during key dates of 2020
* A comparison between states and between twitter activity across states for two different political groups (BLM versus Capitol Insurection geospatial patterns)
* Increased knowledge of how twitter activity around BLM and the Capitol Insurrection changed over time
