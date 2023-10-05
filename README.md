# Final-Project-Tableau
By: Brigitte Sullivan </br>
Submitted on: Monday, September 25, 2023 </br>
Lighthouse Labs Data Science Program </br>

## Project/Goals
The goal for this project was to: 
* Develop insightful, relevant Data visualization for Worldwide tuberculosis (TB) data gathered by the World Health Organization. Available at [who.int](https://www.who.int/teams/global-tuberculosis-programme/data)
* Compile the insights into dashboards that tell a compelling story efficiently

## Process

### 1. Light Research of TB: 
- Seek inspiration from other Health related dashboards 
- Social media review for interesting information about TB.
    - cure found in 1958
    - TB played a role in "causing" WW1, all three individuals tasked with assassinating Princip were suffering from TB and their impending death may have contributed to their willingness to participate in an assassination scheme. 
- Although the original data set was provided, I searched online and found the source data from WHO. So that I could better familiarize myself with the context of the data. 
- used a data dictionary found online to familiarize myself with the terminology used in the data set. These results informed the scope of the project: 
  - Found from WHO that TB fatalities where HIV positive are recorded as HIV deaths so decided to ignore any features indicating HIV positive
  - Found that the high/low bound features were less relevant and could be ignored for this analysis and focus on the metric. However, this does add an important nuance that each data point is more like a range. 
  - research meaning of prevalence vs. incidence, chose to focus this project on prevalence and mortality rates due to time constraints.
  - found that WHO has a target case detection rate of 75% and a target cure rate of 85% for TB 
### 2. EDA
Started building numerous different visualizations
* maps
* line charts 
* scatter plots with clustering
Realised that the most interesting features were mortalities per capita and prevalence per capita so chose to focus on features indicating per capita. This also made comparisons between countries with different populations more meaningful and accurate.

### 2. Dashboards
* From the most interesting visuals created during the EDA begin building a dashboard of TB status worldwide. 
* Found that I wanted more detail at the country level so created country profiles

## Results


Option selected: **Option 2 Data set: IV) Tuberculosis Burden by Country**
Focused on two perspectives:
1. What is the TB burden worldwide over time?
    * Which 10 countries suffer the highest mortality rates over time? (in alphabetical order)
        * Bhutan, Cambodia, Central African Republic, Democratic Peoples Republic of Congo, Gabon, Lao PDR, Mozambique, Myanmar, Namibia, Nigeria
        * Central African Republic made excellent progress reducing mortality rate from 1993 to 2013, although still among top 10 (worldwide dashboard).
        * TB mortality rate in Nigeria remains largely unchanged in the data. 
    * TB has steadily been decreasing over time as access to cures becomes more available. 
    * In developped countries, TB mortality rates remain low over time.
    * Number of TB cases and mortality starts decreasing in 1998, from 1993.
    * mortalities per capita dropped 50% since 1993. 
    * 8.76% is the average mortality rate per capita in 2013


2.  What is the TB burden in a specific country over time?
    * how is that country's performance against WHO's target detection rate? 
        * China was able to significantly reduce its mortality rate per capita between 1990 and 2013
        * Bhutan had the highest decrease in mortality rates between 1990 and 2013 from 277 deaths per capita in 1990 to 12 deaths per capita in 2013 (96% decrease in 14 years) (excluding countries without data for 1990 or 2013). Maldives had the second lowest. 
        * Note that often the WW case detection rate falls short of the target. 

About the visuals used:
* Vizualisations focused on how mortality and cases changed accross time since there was a large range of years of data. 
* Used Pages in Tableau to effectively show continous progress accross time. 
* Chose reds/oranges to represent the urgency and seriousness of mortality data and blues to represent case frequency so that the audience is drawn to mortality rates first, then cases. 
* used geographic maps when comparring how other countries are doing in comparison with each other. 
* used bar charts with reference line to highlight years that a specific country met or exceeded the case detection rate and where the country was in comparison with the worldwide case detection rate.
* used forcasting for country specific cases since this would present the most accurate forecast than using full worldwide data set.  

## Challenges 
- instructions provided were unclear and made it challenging to understand the project requirements
- lack of domain knowledge may have derailed analysis, mitigated this by doing up front research. 

## Future Goals

- reformat percentages as floats then change format to percentage (more accurate. I was able to format the visualizations effectively so this was deprioritized
- Develop a way to identify what the 'cure rate' is by country and measure performance against the 85% cure rate target.

