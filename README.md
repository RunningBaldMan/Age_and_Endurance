# Endurance and Age: Marathons vs. Ultra Marathons

    Do older athletes participate in ultra marathons at higher rates than traditional marathons?

Unlike short-distance track events (100m–10,000m), endurance running often appears to attract a disproportionate number of older athletes—those in their 30s, 40s, 50s, and beyond. This project explores whether that perception is supported by data.

    Project Overview

For this analysis, I compare two major endurance race types:
Marathons (26.2 miles) — used as a baseline endurance distance
Ultra Marathons (distances greater than 26.2 miles) — events that emphasize patience, experience, and long-duration effort
The working hypothesis is that ultra marathons skew older than marathons, particularly at longer distances (50 miles and above), where experience and pacing may offset age-related declines in speed.

## Datasets Used

    Marathon Dataset

Source: Kaggle – 2010–2019 Fall Marathons - https://www.kaggle.com/datasets/runningwithrock/2010-2019-fall-marathons

Original size: 109.7+ MB
Filtered years: 2016–2019
Final size after cleaning: 215.4+ MB
Data cleaning steps:
Restricted to years 2016–2019
Dropped null values
Removed runners younger than 17 and older than 98

Age boundaries were informed by real-world records:

Youngest known marathon finisher: Umi Taguchi (17) – 2024 Honolulu Marathon
Oldest known marathon finisher: Dimitrios Yordanidis (98) – 1976

    Ultra Marathon Dataset

Source: Kaggle – The Big Dataset of Ultra Marathon Running - https://www.kaggle.com/datasets/aiaiaidavid/the-big-dataset-of-ultra-marathon-running/data

Original size: 740+ MB (1798–2022)
Filtering and transformation steps:
Restricted to years 2016–2022
Converted event dates to datetime format
Filtered to fall races (September–December) to align with marathon seasonality
Final dataset size: 33.9+ MB
Notably, during this time period:
No finishers were under age 20
Only 3 finishers were age 85 or older

This aligns with anecdotal evidence of extreme longevity in ultra running, such as:

Reports of 100-year-old 50-mile finishers
Bob Becker, who completed the 135-mile Badwater Ultra at age 80 (as of 2025)

    Expectations 

Based on the nature of ultra endurance events, I expect:
The oldest finishers to appear in the ultra marathon dataset
Higher average ages among ultra marathoners compared to marathoners
The age difference to become more pronounced at distances 50 miles and longer, where cutoff times typically range from 13–15 hours or more

These longer durations may favor experience, pacing, and mental endurance over raw speed.

The analysis includes:

Age distribution comparisons between marathon and ultra marathon participants
Age bracket aggregation and visualization
Distance-based comparisons within ultra marathon events
A personal comparison of my own age relative to average marathon and ultra marathon participants during the selected years


## How to Use
1. Clone this repository.
2. Install the required Python packages:  
   pip install -r requirements.txt
3. Open `Endurance_Beyond_Age.ipynb` in Jupyter Notebook or JupyterLab.

## Output
The analysis shows that the average age of fall marathon finishers from 2016-2019 is 39 years old. There are outliers with the youngest age of a marathon finisher being 15, and the oldest age of a marathon finisher being 116.

## Data Sources
- Results_marathon csv (provided in `data/`)
- Indianapolis Monumental Marathon 2019 csv (provided in 'data/')
- Results_um csv (provided in 'data/')

## Author
Justin Masters aka Runningbaldman - Emerging Data Analyst

## License
MIT License# Age_and_Endurance

## References
ChatGPT and other AI tools were used as supplementary learning resources for code troubleshooting, error handling, and idea development. The author retains full responsibility for all analyses, interpretations, and conclusions.
