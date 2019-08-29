# Fantasy-Football-and-Machine-Learning
The first problem encountered was choosing a target and features. The target is the future season fantasy position rank, which turns out is very difficult to predict. The second problem was setting up the data so that we are using, for example, the 2015 season data to predict the 2016 season end of season ranking. This is difficult with the data as there is a lot of variance between players between seasons due to rookies, injuries, and depth chart change. To avoid this I used a inner join merge, which essentially merges data together on a shared value. So I filtered out all players that did not start over 10-12 games depending on the position. After that I merged together the two dataframes from for example the 2015 and 2016 seasons containing qb's that had started over 12 games. When merging, I merged based on name as the shared value, because if a player did not start over 12 games in both seasons their data was meaningful.

I was now able to use the sklearn linear regression model to fit, predict, and score, the quarterback, runningback, wide reciever, and tight end position. The linear regression model performed best with the tight end position and worst with the quarterback position. I plan on changing models to compare performance between models.

I hope to find data for the upcoming season to predict the future bright performers in the NFL and have a fantasy advantage in my upcoming drafts.

I plan on utilizing different methods from sklearn to compare scores to the linear regression model.

Also go to www.fantasysportsrogue.com to see personal rankings and more analysis.
