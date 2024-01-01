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
In my first look at the data when comparing the amount of athletes of each gender versus the lengths of races that those athletes compete in, I found
that the majority of athletes are men, the majority of races are less than 70 miles or so, and less than 24 hours or so. However there are races in this data set that are
up to and past 3000 miles in length, like the transcontinental race where people run across the entirety of the USA. I decided to separate the dataset into two visualizations for more and less than 120 miles, and 80 hours, as everything at and below those numbers makes up over 80% of that data.

In my second visualization I wanted to look at different countries, and see the amount of people that signed up from each country.
Unsurprisingly the USA was at the top of the list, followed by France and Japan, with Canada, Australia and the remaining countries in the western european area like Italy and the UK, where following. There were a lot of countries like most of Africa that had no participation, and Latin America was low as well, as ultra running can be a very expensive sport, especially when it can last for days or weeks, of which you generally need supervision and supplies constantly.

The third visualization shows race entries vs gender and age. This visualization shows that women as they get older enter more and more race, but younger women do not seem to have any interest in doing more than a few ultras. 
Whereas men will enter into more and more races as they get older and will also do a larger amount of races at a young age.
Ultra running is also a sport where you will see people of every age from the teenage years to people in their 90s. I have personally participated in ultra marathons with people, that if I remember correctly, had dentures.

The second to last visualization shows the 15 athletes both male and female, with the most 1st place wins. The first person for both men and women have a very large lead over their gender groups, while the remaining 14 in each gender have a much smaller difference between all.

For my last visualization I wanted to look at overall winners, which means, the winners that had the best results for both men and women. While it is rare, ultra running is one of those rare sports, of which I know no others, where a woman can go in a race and beat every single man in the race. In the dataset given, there seems to be about 5% total of all overall winners that are women. 

## Results
There are lots of outliers in this dataset, and outliers in a dataset like this are examples of exceptional human beings, people that dare to do what most would be too afraid to.
As one would expect the dataset is predominantly male, and the race lengths are predominantly on the shorter side. Relatively very few people come from 2nd, 3rd world countries, as
this sport is definitely one for the more affluent. Most of the time and it is also a sport for older folks where you will see even people in their 90s doing these races, which you might not think because of the extreme nature, and on top of that older athletes will often do the longer races as well, it seems that younger people don't really have the strength to do events that last for days.

None of this comes as a surprise to me personally, as I am already aware of these data points from my exposure to ultra running, but maybe for you they are!

## Acknowledgments
Special thanks to my mentor, Logapriya Viswanathan, for her invaluable guidance and support throughout this project.