# springboard_capstone_1_milestone_report

Jason Ho
Data Science Career Track
Milestone Report - Capstone Project 1

Define the Problem

The problem is that the sport of basketball is changing and organizations must consider a player’s talent and basketball IQ which translates to production on the court.  Many teams rely on new players, specifically rookies, to make a team successful in the long run.  Some organizations invest in the wrong players which lead to the teams’ downfall each season.  With a more analytical approach to scouting and statistics, NBA organizations can make the proper decisions when deciding to invest in certain players to be the face of the franchise.  

I hope my project will answer the following question: should we (the organization) invest in this player based on their rookie year statistics?

Identify Your Client

My clients will be general managers for each organization in the NBA.  Managers can consult with scouts and other key figures in their organization when making long term decisions about which players to invest their money in.  

Describe Data Set (Cleaning/Wrangling)

The first step was to find the right data set to do analysis.  I found a set of rookie statistics from many players from different time periods.  There is a column that has a 1 or 0 that tells us if that player played in the NBA for at least five years (1) or not (0).  

I used OpenRefine, a data cleaning tool, to fill in missing values and transformed each attribute to a number except for the player names.  Once the data set was ready, I joined that with another dataset with the same players but with their efficiency.  There were some players who were in one data set but not the other, so the join eliminated the names that were not in both data sets.  

Once the whole data set was joined, I separated it into three sets of players: players who played for at least five years, players who did not play for at least five years, and new players who have not yet been in the league for five years.  I mainly focused on the first two sets of players.
Other Potential Data Sets to Use

Some other potential data sets I could have used (if they exist) are a players’ sophomore (second year) statistics to compare with the rookie statistics and college statistics.  

Since my data sets included every stat used in basketball, I did not need more data to analyze the rookie statistics of all players.  

Explain Initial Findings

My initial finding in descriptive statistics was that the players who played in the NBA for at least five years had higher averages for mostly every statistic than the players who did not play in the NBA for five years.  With the exception of turnovers (in this case, less is better), most players who played at least five years had higher averages in shooting percentages, minutes played per game, and player efficiency rating than those who did not play for five years.  This could be seen visually through normalized histograms and difference of means.  

Efficiency is a calculation of the sum of (points, rebounds, assists, steals, blocks) minus the sum of (missed field goals, missed free throws, and turnovers) all divided by the number of games played.  I decided to focus on efficiency and minutes per game because those stats are good indicators for a player’s talent.  

When performing inferential statistics and running hypothesis tests, my null hypothesis was that there was no statistically significant difference between the two groups of players for <stat>.  All p-values were 0, so I rejected the null in favor of the alternative, that there is a statistically significant difference among the two groups of players.  

I ended up making some edits to my data story and inferential statistics iPython notebooks before submission.  The data story contains the joining of two data sets and descriptive statistics, which now includes normalized histograms.  My inferential statistics looks cleaner throughout the notebook using the functions I wrote.
