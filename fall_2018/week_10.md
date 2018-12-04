## Last Week's Accomplishments

> Last week, I was planning to use the current speed data to calculate the estimate times for each stops. But since I still have problems to run the local shuttle tracker. I try again to install it. It looks works. Actually I am still not that familair with Go and the overall project, so I start with looking through all the code in the master branch to learn how it works. It is hard. When I look a new file I start to forget what the last file says. 
When the local shuttle tracker installed, it shows that "could not get data feed". I remember Frank has told me that We need to add json code in it. I have already has these json files when I calculate the distance, then I put them in. When it add the data in, the page will not appear shuttles until I refresh the page. So I think if it is not that difficult I can change the static files to make it better. 
I look at it, I really not familair with vue. Did some try.

The 2 bugs and changes I made are:
1. 
When I add routes, then delete, the ID number will get greater and greater----cannot get back to the old one. For example, you add a new route which appears as ID-2, when you delete it, the next route you add will appear as ID-3 rather than ID-2. 
For this, I made change on "route.go" file in file "postgres", line 299 to line 303. I have add comment on the change I made.
LOCATION： https://github.com/lisagao2333/shuttletracker/blob/eta/postgres/route.go
2. 
When you add a new route, the page will not automatically refresh. 
For this, I just add an "refresh=true". 
Also, followed bu this, I add an functionality that the people add the route can manually set the ID. For examample, I add a new route, I manually set it as ID-5, and when I add a new route, the newly added route can not be named as ID-5. If the ID number is repeated, then an alert will appear. This change is very small, but I feel it is very user friendly. All the change I made are for "user friendly". They may not change the entire project a lot, but make user friendlier. 
Looks like this: https://drive.google.com/file/d/1xcCWvOMA-QMMvbkAFN-9sz2u8bxxUN92/view?usp=sharing
LOCATION: https://github.com/lisagao2333/shuttletracker/blob/eta/static/js/routes.js
The two change are from line 207 to line 215.


## This Week's Plan

> Continue work with ETAs. The very first thing is to calculate the relative velocity idea we had introduced. I will collect the average speed for each shuttle during 30 days. I think there is no 30 days left for schools, so for this semester I will collect the average speed data for one week.

## Anything Blocking?

> Collecting data.> 