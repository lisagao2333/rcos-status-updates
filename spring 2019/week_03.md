## Last Week's Accomplishments

>Last week, I have done several things.

- Commit the json file for the historical data for the last 30 days. This file contains 11 dictionaries, representing 11 
shuttles that currently work for the RPI shuttle system. Each of the dictionary includes thousands of data collected from 
the database every 5 minutes.
- Make new pull request to the origin responsitory, for merging eta branch in my responsitory to the master branch in wtg 
responsitory; then I switch the base, which makes both responsitories consist with each other. 
- Finish the documentation _Relative Velocity Explainations_ that neatly explain the algorithms for "relative velocity", 
and commit to my responsitory. Relative velocity stands for: the amount of vehicles minus one, then multiply by the average 
velocity, then add the current velocity, finally the sum divided by the amount of vehicle. Different from reading data 
from json file, this time I directly read real time data from the https://shuttles.rpi.edu/history and 
https://shuttles.rpi.edu/updates, which makes the estimated calculations more precise. When calculating with the average 
velocity based on the historical data, there are two choices for calculating average velocity: 1. Average velocity 
for all the data records in the history endpoint. 2. First find average velocities for each shuttle, then find the average 
velocity of these 11 shuttle. I think the second one is better, since later we may need the individual data for each shuttle.
- Finish the calculations for relative velocity in python, and commit to my responsitory. When run the program, it will 
print out the number of shuttles, average velocity, and current velocity, and finally the relative velocity. Current 
velocity shows 0 when there is no data flow.
- Plan for this semester explanations: I used to code in Go lang for the last semester, and complete several milestones. 
This semester, Frank decides to do all work in python, then ports to Go lang, since he thinks that would be easier for 
coding process. So this semester I will work in python and work together with ETA my groupmates. Then I will continue be
working on my go lang part. 

## This Week's Plan

> For this week. I will enjoy my spring break. Have a nice spring break every one!


## Anything Blocking?

> None.


## Notes

> None.
