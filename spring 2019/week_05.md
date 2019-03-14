## Last Week's Accomplishments

>Last week, I have done several things.
 
- I complete the documentation MD file on "How to add Images in MD files", and commit it to Github.
- I start to write the python file on calculate the ETA of the 11 shuttles we have on campus. Based on exploring the history 
endpoint, we can see currently we have 11 shuttles in service, so the code I write will finally come out 11 data. Since 
there are only 3 or 4 shuttles operating at a time, when we do the calculations, the shuttles that are not in service 
will show a "0" for their ETA result. This will be done in 3 or 4 weeks. And I will use Go lang block to export those 11 
data, so the front end team can use there 11 data from Go file to do the front end. 
- As I plan, the code will run every 5 seconds to get data from endpoint web page and do the calculations. I think 5
seconds time period is very proper for ETA, since the update endpoint https://shuttles.rpi.edu/updates updates every 
3 or 5 seconds. As I plan, the ETA time finally will be accurate to seconds.
- I meet with my group members, and talk to them about my plan, so we can work together, and made the ETA figure done 
by the end of the semester.

## This Week's Plan

> For this week, I will continue to write about the ETA python file. 


## Anything Blocking?

> When I deal with the history endpoint https://shuttles.rpi.edu/history, I have meet several problems. And I also came 
out solutions for each.
- I find it take times to load the entire page of data, more than 5 seconds. So to achieve faster speed and for better 
convenience, I decide to download the json file. Rather than read from web page, for the history endpoint I will read 
from local file. Since this endpoint records the data for the past 30 days, I will also write code to renew 
the history local json file every 30 days.
- When the history endpoint finishes loading, I usually right click the web page and save, as json file, just as same as 
what I do for downloading other small size json files. However, since the size of the history json file is too large
(more than 700 MB) and when I use usual way to save it does not work(it usually only save 24.45 MB of the entire file). 
So I just copy and paste all the text on the web and made a json file. 
- The problem above is solved, however, the portion that I wrote for automatically renew the load json file will 
probably not work. I need to find a new way to do it, rather than manually renew the file. Probably change the renewing 
time, not every 5 seconds but more. I will test the loading time and make a proper time period. But right now, I will use 
5 seconds. We can do improvement when I finish write the whole thing.



## Notes

> None.
