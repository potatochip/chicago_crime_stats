##Chicago Violent Crime in a Nutshell

I acquired Chicago violent crime data for a project on the effect of media violence on violent crime (will post about this soon, I swear). As I was browsing the data, I noticed a very strange trend.

Most of the date looks like this:

```
10027862,04/10/2015 07:20:00 PM,BATTERY
10028400,04/10/2015 07:17:00 PM,BATTERY
10027915,04/10/2015 07:03:00 PM,ASSAULT
10028127,04/10/2015 07:00:00 PM,BATTERY
10027914,04/10/2015 07:00:00 PM,ROBBERY
10027859,04/10/2015 07:00:00 PM,BATTERY
10028087,04/10/2015 06:48:00 PM,BATTERY
10027831,04/10/2015 06:45:00 PM,BATTERY
10028119,04/10/2015 06:40:00 PM,BATTERY
10027829,04/10/2015 06:30:00 PM,ASSAULT
10031052,04/10/2015 06:30:00 PM,BATTERY
10028294,04/10/2015 06:24:00 PM,BATTERY
10028130,04/10/2015 06:00:00 PM,ROBBERY
10027783,04/10/2015 06:00:00 PM,BATTERY
10027785,04/10/2015 05:50:00 PM,BATTERY
10027846,04/10/2015 05:48:00 PM,BATTERY
10027786,04/10/2015 05:45:00 PM,BATTERY
10027767,04/10/2015 05:45:00 PM,BATTERY
10027736,04/10/2015 05:30:00 PM,ASSAULT
10027807,04/10/2015 05:25:00 PM,ASSAULT
10027903,04/10/2015 05:20:00 PM,BATTERY
10027874,04/10/2015 05:20:00 PM,BATTERY
10027898,04/10/2015 05:18:00 PM,BATTERY
10027756,04/10/2015 05:15:00 PM,BATTERY
10027781,04/10/2015 05:07:00 PM,BATTERY
10027960,04/10/2015 05:00:00 PM,BATTERY
10027737,04/10/2015 05:00:00 PM,ROBBERY
10027902,04/10/2015 05:00:00 PM,BATTERY
10027995,04/10/2015 05:00:00 PM,BATTERY
10027780,04/10/2015 04:57:00 PM,ASSAULT
```

But then when you get to New Years, a pattern starts to emerge. 

```
9447124,01/01/2014 12:33:00 AM,ASSAULT
9902846,01/01/2014 12:30:00 AM,CRIM SEXUAL ASSAULT
9446760,01/01/2014 12:30:00 AM,BATTERY
9446848,01/01/2014 12:30:00 AM,BATTERY
9448651,01/01/2014 12:25:00 AM,BATTERY
9446789,01/01/2014 12:25:00 AM,BATTERY
9446832,01/01/2014 12:24:00 AM,ASSAULT
9446849,01/01/2014 12:20:00 AM,BATTERY
9446780,01/01/2014 12:20:00 AM,BATTERY
9446844,01/01/2014 12:15:00 AM,BATTERY
9446869,01/01/2014 12:14:00 AM,BATTERY
9446816,01/01/2014 12:10:00 AM,BATTERY
9446917,01/01/2014 12:10:00 AM,ROBBERY
9446764,01/01/2014 12:10:00 AM,BATTERY
9446958,01/01/2014 12:05:00 AM,ASSAULT
9574233,01/01/2014 12:01:00 AM,CRIM SEXUAL ASSAULT
9897526,01/01/2014 12:01:00 AM,CRIM SEXUAL ASSAULT
9447582,01/01/2014 12:01:00 AM,CRIM SEXUAL ASSAULT
9515113,01/01/2014 12:01:00 AM,CRIM SEXUAL ASSAULT
9925981,01/01/2014 12:01:00 AM,CRIM SEXUAL ASSAULT
9447168,01/01/2014 12:01:00 AM,BATTERY
9490406,01/01/2014 12:01:00 AM,CRIM SEXUAL ASSAULT
9613833,01/01/2014 12:01:00 AM,CRIM SEXUAL ASSAULT
9634981,01/01/2014 12:01:00 AM,CRIM SEXUAL ASSAULT
9659025,01/01/2014 12:00:00 AM,CRIM SEXUAL ASSAULT
9993250,01/01/2014 12:00:00 AM,CRIM SEXUAL ASSAULT
9593821,01/01/2014 12:00:00 AM,CRIM SEXUAL ASSAULT
9599640,01/01/2014 12:00:00 AM,CRIM SEXUAL ASSAULT
9728010,01/01/2014 12:00:00 AM,CRIM SEXUAL ASSAULT
9728020,01/01/2014 12:00:00 AM,CRIM SEXUAL ASSAULT
9448361,12/31/2013 11:55:00 PM,BATTERY
```
Let me know if you can spot the trend. Maybe, you might think to yourself, this is just a random occurrence. I promise, it is not. At first I thought that this must be some sort of sick crime-ring that the police busted one year. Unfortunately, that is not the case. 

##A Pattern Emerges
The following is a time-series plot of the last 15 years of criminal sexual assault in Chicago.

![Sexual Assaults Over 15 Years]({{ site.baseurl }}/images/sexual_assault_post/sexual_assaults_per_day_15_years.png)

Those massive regularly occuring spikes? You guessed it, New Years.

Let's zoom in a bit. Here is the same data over a four-year period.

![Sexual Assaults Over Four Years]({{ site.baseurl }}/images/sexual_assault_post/sexual_assaults_per_day_four_years.png)

And further in. One year, 2010.

![Sexual Assaults Over One Year]({{ site.baseurl }}/images/sexual_assault_post/sexual_assaults_per_day_one_year.png)

Let us take it one final step. Here we are down to just two months: December and January. What will it look like?

![Sexual Assaults Over Two Months]({{ site.baseurl }}/images/sexual_assault_post/sexual_assaults_per_day_two_months.png)

This is so ridiculous. New Years accounts for a full 34% of all the sexual assaults that occur in the month of January.

![Sexual Assaults in January]({{ site.baseurl }}/images/sexual_assault_post/sexual_assaults_pie.png)

##More Numbers
The following is a description of the number of sexual assaults reported in Chicago in 2010.

	count    381.000000
	mean       3.742782
	std        2.965056
	min        1.000000
	25%        2.000000
	50%        3.000000
	75%        5.000000
	max       41.000000

According to these numbers, in 2010, you were 1,095% more likely to be a victim of sexual assault on New Years in Chicago versus the average day. I had to really think about how to format that percentage, since I don't normally work with percents that high. That's how high it is. That is almost 1,100% more likely! I'm not sure I can emphasize that. 

###***Almost 1,100% more likely!!!***

Alright, I emphasized it.

##Final Thoughts
![Sexual Assaults Per Year]({{ site.baseurl }}/images/sexual_assault_post/sexual_assaults_per_year.png)

Chiacago's performance record *is* getting better. However, I think it is important to note that 68% of sexual assaults go unreported.[^fn-footnote] We are not just looking at 41 separate reported incidences of sexual assault on New Years (when one time alone is disturbing enough). What we are looking at is likely over 128 separate occurences of sexual assault. Seriously messed up.

In 2014, there were 1,234 separate reported incidences of sexual assault. That is 3,856 sexual assaults. In one year. In one city in America. Something is very wrong here.

We can speculate as to why. People are out with large groups of people they don't know, they're out late, and the alcohol is flowing. But still, the increase seems a little astronomical.

To some, maybe this seems like it would be obvious. However, I feel like parents and loved one's are always giving out warnings for other holidays. "It's Halloween, don't take unwrapped candy." "It's St. Patrick's Day, look out for drunk drivers." But I have never once heard someone say, "it's New Years, be careful, you might get raped."

##Future Topics

With part 2 of this post-series, I am planning a similar analysis extended to the rest of the violent crimes in Chicago. I'm hoping to finish a regression predicting amount of crime per date for each category.

Thanks for reading, and be careful going out for New Years.

[^fn-footnote]: Justice Department, National Crime Victimization Survey: 2008-2012