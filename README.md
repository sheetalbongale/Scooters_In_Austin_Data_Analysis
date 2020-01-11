##  Scooters in Austin Data Analysis | JSON-and-team 
### Team Members: Erin Bentley, Jason Jones, Sana Khan, Sheetal Bongale
#### UT Data Analysis & Visualization Bootcamp | Python Project 1 | January 2020
---
### Project Requirements:
- Two to three plots (and think about getting information visualized onto fewer plots). NO PIE CHARTS
- Greater than or equal to two datasets
- At least one dataset comes from merging different tables/sources (deliverable)
- At least 1 dirty dataset (not Kaggle)
- At least one API used
- Export dataframe to SQL Database (explained 1/4/2020)
- 10 minute presentation
- Use Jupyter Lab to present...no PPT.
---
## Project Name: ***Scooters in Austin Data Analysis***

### Project Description: 

### Data Set:
* City of Austin 311 OpenData: https://data.austintexas.gov/resource/7d8e-dm7r 
https://data.austintexas.gov/resource/i26j-ai4z.json
* Austin Shared Mobility API: https://data.austintexas.gov/Transportation-and-Mobility/Shared-Micromobility-Vehicle-Trips/7d8e-dm7r
https://data.austintexas.gov/resource/7d8e-dm7r.json
* FCC API call for lat/long to census tract conversion: https://geo.fcc.gov/api/census/

### Research Questions:

### Actions and Tasks:
- Obtaining all the data
- Data Cleaning and Exploration
- Chart Plotting
- Writing Analysis

### Written Data Analysis:

### Resources:
- https://dev.socrata.com/foundry/data.austintexas.gov/7d8e-dm7r
- https://austintexas.gov/micromobility

### Conclusions:

### Further Reading:

Our Questions:

• Are some neighborhoods guilty of complaining about scooters more, even when adjusted per capita?
• Or, do the neighborhoods with the highest numbers of scooter ride endpoints also have the most scooter related complaints?
• Are people more likely to complain about scooters in a neighborhood where scooters are less commonly found?
• Do local events, month of year, or day of week impact the total number of scooter rides?
• Where are the scooters going?
• What are the average, minimum, and maximum trip distances?
• Do longer scooter rides to farther-out neighborhoods result in more complaints?

Our Resources:

• City of Austin 311 OpenData: https://data.austintexas.gov/resource/i26j-ai4z.json 
• Austin Shared Mobility API: https://data.austintexas.gov/resource/7d8e-dm7r.json 
• FCC API call for lat/long to census tract conversion: https://geo.fcc.gov/api/census/ 
• Flat file for census tract to zip code: https://www.huduser.gov/portal/datasets/usps_crosswalk.html

What we think we'll see:

• We think some neighborhoods complain about scooters regardless of the number of scooter rides per person in the population. 
• We think that scooter rides, and complaints about them, soar when events are happening in town, along with a rise every weekend. 
• We think complaints raise as people take scooters into neighborhoods where scooters are less common.

Our method:

• The first thing we did was use austintexas.gov data to create a data frame with the Austin Shared Micromobility data. This tracks every scooter ride in town, regardless of brand / parent company. This data is visible by census tract. 
• Then, we took the census zipcode key and appended it, to tell us the zipcodes for the various rides. 
• From there, we could join our tables by zipcode and then compare them to the 311 complaints dataset for scooters.
