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

<div class="alert alert-block alert-info">
<b>For the Marathon I have chosen a dataset simplely called 2010-2019 Fall Marathons. This dataset was originally 109.7+ MB and has been reduced to the years 2016-2019. This cut it down to 385.6+ MB. Nulls were then dropped leaving 215.4+ MB. The full dataset can be found at https://www.kaggle.com/datasets/runningwithrock/2010-2019-fall-marathons</b> 
</div>

I researched and found that the youngest person to run a marathon was Umi Taguchi at age 17 at the 2024 Honolulu Marathon. Dropped ages younger than 17.

Through research, the oldest person to run a marathon was Dimitrios Yordanidis in 1976 at age 98. Dropped ages older than 98.

<div class="alert alert-block alert-success">
<b>For the Ultra Marathon dataset I have chosen a dataset of over 7 million race records from 1798-2022. This dataset came in at 740+ MB and was trimmed to years 2016-2022. Since the Event dates were in Day, Month, Year format they were converted to datetime. Doing this left the dataset at 169.5+ MB. Since the Marathon data set covered Fall races, the Ultra Marathon dataset was reduced to fall races (Sept to end of year). Finally taking the dataset to 33.9+ MB. The full dataset can be found at https://www.kaggle.com/datasets/aiaiaidavid/the-big-dataset-of-ultra-marathon-running/data</b> 
</div>

I did not cut ages from the Ultra Marathon list since during the previously mentioned date range there were no finishers younger than 20 and only 2 aged 85 and 1 aged 90. 

In the Ultra Marathon, I've heard rumors of a 100 year old finishing a 50 mile race, and as of 2025, 80 year old Bob Becker completed the 135 mile Badwater Ultra that runs through Death Valley in July.

With distances over 26.2, I expelct the patients and experience to play a factor into the age diferences between the two data sets. I expect the oldest person to finish the event to be from the Ultra Marathon data set. I also expect the average ages to be older in the Ultra Marahon data set from 50 miles and longer, this would encompance cut-off times of 13 hours and up. The average cut-off 50 mile race is 13-15 hours. 

<div class="alert alert-block alert-warning">
<b>I will compare my age to the average marathoner and ultra marathoner age during the timeframs listed above<b>
</div>


## How to Use
1. Clone this repository.
2. Install the required Python packages:  
   pip install -r requirements.txt
3. Open `Endurance_Beyond_Age.ipynb` in Jupyter Notebook or JupyterLab.

## Output
The analysis shows that the average age of fall marathon finishers from 2015-2019 is 39 years old. There are outliers with the youngest age of a marathon finisher being 15, and the oldest age of a marathon finisher being 116.

## Data Sources
- Results2 csv (provided in `data/`)
- Indianapolis Monumental Marathon 2019 csv (provided in 'data/')

## Author
Justin Masters aka Runningbaldman - Emerging Data Analyst

## License
MIT License# Age_and_Endurance
