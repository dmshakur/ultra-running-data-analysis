# Ultra running data analysis project

## Introduction
**Project Duration**: Started on December 19th, finished on December 

### Personal Information
- **Name**: D'angelo Shakur
- **Current Location**: Medellín, Colombia
- **Country of Origin**: United States
- **Contact**: 
  - Email: dangeloshakur@gmail.com
  - Phone: +57 321 450 7954 (Colombia)

### Files and file structure
- data/
    - ultra_marathons.csv
    - male_ultra_marathon_runners.csv
    - female_ultra_marathon_runners.csv
- figures/
    -
- notebooks/
    - data_processing.ipynb
    - data_analysis.ipynb
- README.md

### Data Source and Characteristics
- **Source**: [The big dataset of ultra marathon running](https://www.kaggle.com/datasets/aiaiaidavid/the-big-dataset-of-ultra-marathon-running)
- **Size**: 790 Megabytes
- **Structure**:
  - Rows: 7461195
  - Original columns: 13 (
      Event, 
      Event dates, 
      Event name, 
      Event distance/length, 
      Event number of finishers, 
      Athlete performance, 
      Athlete club, 
      Athlete country, 
      Athlete year of birth, 
      Athlete gender
    )
  - New Columns: 16 (
      year_of_event,
      event_name,
      distance_or_length,
      no_of_finishers,
      total_distance, 
      athlete_club, 
      athlete_country, 
      birth_year, 
      gender, 
      age_category, 
      average_speed, 
      athlete_id, 
      race_metric, 
      start_date, 
      end_date, 
      fastest_time
  )

## Purpose & personal reasons for doing this project
I of course wanted to choose to work on a dataset that interested me first and foremost. I wanted to do something in an athletic field that I am interested in like running, martial arts or lifting weights. And upon looking at Kaggle's datasets I saw that there was an ultra running dataset. The data looked robust enough so that I wouldn't get too bored, as some datasets are kind of dull in their data, as in they will only have a few columns, with less interesting data points. My goal for this project is not like my last project, where I had a specific question that I wanted to ask of the data. For this project I simply want to put into practice my presentation, visualizations and to do a good and thorough job of cleaning the data, and analyzing it.

## Data processing
#### Dates
I was able to ge the data processing finshed in one day. There was a constant slew of small problems that needed to be solved, of which I didn't have very much trouble at all. But when I went and tried to turn a date column into a start and end date column, that took several hours just working on that. I had originally wanted to get the entire thing done in one notebook cell, but I eventually decided to compartmentalize each different case into separate cells for a total of 4 cells. After I did that it solved the problem almost immediately. But the issue that I had still boggles my mind. There was one date, `18.03.2018`, which for some strange reason kept throwing an error saying that the day was out of range for the month, which is clearly impossible for the 18th of any month. Strange, I wish I could have figured out why that was happening.

#### Everything else
For the most part everything fit in place, with some tinkering of course. I learnt a few things as well, and I spent quite a bit of time with Pandas. I learnt about masks and now I understand what they are, and that I have been using them for a while, I just never knew it. 

## Data analysis and exploration
The data analysis portion of this project took a bit longer than normal. There were some difficult to solve problems, like dealing with plotly and trying to create a heatmap showing different countries and the amount of runners from each, it took a while to figure it out, but I eventually got it to work.
I also spent a substantial amount of time trying to query the data properly for certain visualizations in order to create data that could properly be used for each visualization, some were quite easy, some took a while and lots of trial and error.
Upon completing the project I ended up having to go back into previous visualizations and rework my data queries after working on the last visualizationn or so I had realized that I incorrectly queried the data and had to fix those issues.

#### Findings
In my first visualization I found that there seems to be an even number of athletes of both genders signing up for races of similar length. 
