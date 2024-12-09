<h1>Sky Sports-Football Digest Project</h1>
This project to analysis the Sky Sports-Football Digest Project in MySQL. To analyze to gain insights into growth, sex ratio, literacy rate. 

<h1>Project overview:</h1>
Sports Analyst uses MySQL to access two tables of data: one containing information on each team's performance in each game, and another 
containing data on individual team statistics. Both the tables gets updated with each match at FIFA WOORLD CUP performance. 
The analyst uses this data to provide insights into each match, highlighting key moments, performances, and tactical decisions made by the coaches. 
These insights are presented on the program, giving viewers a deeper understanding of each match's events and the factors that contributed to a team's success or failure.

<h1>Dataset:</h1>
The dataset consists of two tables:<br>

Table 1: group_stage_team_stats<br>
• Group - The group that the team belongs to in the current FIFA World Cup tournament.<br>
• Rank - The current ranking of the team based on their performance in the tournament.<br>
• Team - The name of the team.<br>
• Matches played - The total number of matches played by the team in the tournament.<br>
• Wins - The number of matches won by the team in the tournament.<br>
• Draws - The number of matches drawn by the team in the tournament.<br>
• Losses - The number of matches lost by the team in the tournament.<br>
• Goals Scored - The total number of goals scored by the team in the tournament.<br>
• Goals Against -The total number of goals conceded by the team in the tournament.<br>
• Goal Difference - The difference between the total number of goals scored and the total number of goals conceded by the team in the tournament.<br>
• Points - The total number of points earned by the team in the tournament based on the FIFA World Cup point system. (3 points for a win, 1 point for a draw, and 0 points for a loss)<br>
• Expected Goal Scored - The expected number of goals that the team is expected to score based on their performance in the tournament so far.<br>
• Exp Goal Conceded - The expected number of goals that the team is expected to concede based on their performance in the tournament so far.<br>
•  Exp Goal Difference - The difference between the expected number of goals scored and the expected number of goals conceded by the team in the tournament.<br>
• Exp Goal Difference Per 90 - The expected goal difference per 90 minutes played by the team in the tournament, which is calculated by dividing the expected goal 
difference by the total number of minutes played by the team in the tournament and multiplying the result by 90. This is a useful metric for comparing teams' 
defensive and offensive abilities on a per-minute basis.<br>

Table 2: overall_wc_stats<br>

• Players Uused: (Number of Players Used in Games) The total number of players utilized in the games.<br>
•  Avg Age: (Average Age) The average age of players weighted by minutes played.<br>
• Possession: (Possession) The percentage of passes attempted, indicating possession of the ball.<br>
• Games: (Matches Played) The number of games played by a player or squad.<br>
• Games Starts: (Games Started) The number of games started by a player.<br>
• Minutes 90s: (90s Played) The number of 90-minute intervals played by a player, calculated by dividing the total minutes played by 90.<br>
• Goals: (Goals) The number of goals scored or allowed.<br>
• Assists: (Assists) The number of assists provided.<br>
• Goals Pens: (Non-Penalty Goals) The number of goals scored excluding penalty kicks.<br>
• Pens Made: (Penalty Kicks Made) The number of penalty kicks successfully converted.<br>
• Pens Att: (Penalty Kicks Attempted) The number of penalty kicks taken.<br>
• Cards Yellow: (Yellow Cards) The number of yellow cards received.<br>
• Cards Red: (Red Cards) The number of red cards received.<br>
• Goals Per90: (Goals per 90 minutes) The average number of goals scored per 90 minutes of play, with a minimum qualification of 30 minutes 
played per squad game to be considered a leader.<br>
• Assists Per90: (Assists per 90 minutes) The average number of assists provided per 90 minutes of play, with a minimum qualification of 30 minutes 
played per squad game to be considered a leader.<br>
• Goals Assists Per90: (Goals and Assists per 90 minutes) The combined average of goals and assists per 90 minutes of play, with a minimum 
qualification of 30 minutes played per squad game to be considered a leader.<br>
• Goals Pens Per90: (Goals minus Penalty Kicks made per 90 minutes) The average number of goals scored excluding penalty kicks per 90 minutes 
of play, with a minimum qualification of 30 minutes played per squad game to be considered a leader.<br>
• Goals Assists Pens Per90: (Goals plus Assists minus Penalty Kicks made per 90 minutes) The combined average of goals and assists minus 
penalty kicks made per 90 minutes of play, with a minimum qualification of 30 minutes played per squad game to be considered a leader.<br>
• Xg: (Expected Goals) The expected number of goals based on statistical analysis, including penalty kicks but excluding penalty shootouts (unless specified). Provided by Opta.
• Npxg: (Non-Penalty Expected Goals) The expected number of goals excluding penalty kicks based on statistical analysis. Provided by Opta.<br>
• Xg Assist: (Expected Assisted Goals) The expected number of goals that follow a pass leading to a shot based on statistical analysis. Provided by Opta.<br>
• Npxg Xg Assist: (Non-Penalty Expected Goals plus Assisted Goals) The combined expected number of goals excluding penalty kicks plus assisted goals based 
on statistical analysis, excluding penalty shootouts (unless specified). Provided by Opta, with a minimum qualification of 30 minutes played per squad game to be considered a leader.<br>
• Xg Per90: (Expected Goals per 90 minutes) The average expected number of goals per 90 minutes of play, including penalty kicks but excluding penalty 
shootouts (unless specified). Provided by Opta, with a minimum qualification of 30 minutes played per squad game to be considered a leader.<br>
• Xg Assist Per90: (Expected Assisted Goals per 90 minutes) The average expected number of assisted goals per 90 minutes of play based on statistical analysis. 
Provided by Opta, with a minimum qualification of 30 minutes played per squad game to be considered a leader.<br>
• Xg Xg Assist Per90: (Expected Goals plus Assisted Goals per 90 minutes) The combined average of expected goals and assisted goals per 90 minutes of play, 
including penalty kicks but excluding penalty shootouts (unless specified). Provided by Opta, with a minimum qualification of 30 minutes played per squad game to be considered a leader.<br>
• Npxg Per90: (Non-Penalty Expected Goals per 90 minutes) The average expected number of goals excluding penalty kicks per 90 minutes of play based on statistical analysis.<br>
Provided by Opta, with a minimum qualification of 30 minutes played per squad game to be considered a leader.<br>
• Npxg Xg Assist Per90: (Non-Penalty Expected Goals plus Assisted Goals per 90 minutes) The combined average of expected goals excluding penalty kicks plus assisted 
goals per 90 minutes of play based on statistical analysis, excluding penalty shootouts (unless specified). Provided by Opta, with a minimum qualification of 30 minutes
played per squad game to be considered a leader.<br>
• Gk Games: (Matches Played by Goalkeeper) The number of matches played by the goalkeeper or squad.<br>
• Gk Games Starts: (Games Started by Goalkeeper) The number of games started by the goalkeeper.<br>
• Gk Goals Against: (Goals Against by Goalkeeper) The number of goals conceded by the goalkeeper.<br>
• Gk Goals Against Per90: Goals Against per 90 minutes. This column represents the average number of goals conceded by the goalkeeper per 90 minutes of play.<br>
• Gk Shots on target against: Shots on Target Against. This column indicates the total number of shots on target faced by the goalkeeper.<br>
• Gk save pct: Save Percentage. This column calculates the percentage of shots on target against the goalkeeper that are saved, using the formula 
(Shots on Target Against - Goals Against) / Shots on Target Against. It's important to note that not all shots on target are stopped by the goalkeeper, 
as some may be saved by defenders. This metric does not include penalty kicks.<br>
• Gk wins: Wins. This column represents the number of matches won by the goalkeeper or the squad they play for.<br>
• Gk ties: Draws. This column denotes the number of matches resulting in a draw for the goalkeeper or the squad.<br>
• Gk losses: Losses. This column indicates the number of matches lost by the goalkeeper or the squad.<br>
• Gk clean sheets: Clean Sheets. This column represents the number of full matches played by the goalkeeper in which no goals are allowed.<br>
• Gk clean sheets pct: Clean Sheet Percentage. This column calculates the percentage of matches resulting in clean sheets for the goalkeeper.
It is the ratio of clean sheets to total matches played.<br>
• Gk pens att: Penalty Kicks Attempted. This column denotes the total number of penalty kicks attempted against the goalkeeper.<br>
• Gk pens allowed: Penalty Kicks Allowed. This column represents the total number of penalty kicks allowed by the goalkeeper.<br>
• Gk pens saved: Penalty Kicks Saved. This column indicates the total number of penalty kicks saved by the goalkeeper.<br>
• Gk pens missed: Penalty Kicks Missed. This column represents the total number of penalty kicks missed by the opponents against the goalkeeper.<br>
• Gk pens save pct: Penalty Save Percentage. This column calculates the percentage of penalty kicks saved by the goalkeeper, using the formula 
Penalty Kick Goals Against / Penalty Kick Attempts. It's important to note that penalty shots that miss the target are not included in this calculation.<br>
• Gk free kick goals against: Free Kick Goals Against. This column denotes the number of goals scored against the goalkeeper from free kicks.<br>
•  Gk corner kick goals against: Corner Kick Goals Against. This column represents the number of goals scored against the goalkeeper from corner kicks.<br>
• Gk own goals against: Own Goals Scored Against Goalkeeper. This column indicates the number of own goals scored against the goalkeeper by their own team.<br>
• Gk psxg: Post-Shot Expected Goals. This column represents the expected goals based on the likelihood of the goalkeeper saving the shot after it has been taken.<br> 
It includes penalty kicks but excludes penalty shootouts (unless specified). Provided by Opta. An underline indicates missing data, which will be updated when available.<br>
• Gk psnpxg per shot on target against: Post-Shot Expected Goals per Shot on Target. This column represents the expected goals per shot on target faced by the goalkeeper, 
excluding penalty kicks. It indicates how difficult the shots on target are to save and the likelihood of scoring. An underline indicates missing data, 
which will be updated when available.<br>
• Gk psxg net: Post-Shot Expected Goals minus Goals Allowed. This column represents the difference between the post-shot expected goals and the actual
goals allowed by the goalkeeper. Positive numbers suggest better luck or an above-average ability to stop.<br>
• Gk psxg net per90: Post-Shot Expected Goals minus Goals Allowed per 90 minutes. This column represents the difference between the post-shot expected 
goals and the actual goals allowed by the goalkeeper per 90 minutes of play. Positive numbers suggest better luck or an above-average ability to stop shots.<br> 
It does not include own goals. PSxG is expected goals based on how likely the goalkeeper is to save the shot. xG totals include penalty kicks but exclude penalty 
shootouts (unless otherwise noted). Provided by Opta. An underline indicates missing data, which will be updated when available.<br>
• Gk passes completed launched: Passes Completed (Passes Longer than 40 Yards). This column represents the number of passes longer than 40 yards that were 
successfully completed by the goalkeeper.<br>
• Gk passes launched: Passes Attempted (Passes Longer than 40 Yards). This column denotes the total number of passes longer than 40 yards attempted by the goalkeeper.<br>
• Gk passes pct launched: Pass Completion Percentage (Passes Longer than 40 Yards). This column calculates the percentage of passes longer than 40 yards that were 
successfully completed by the goalkeeper.<br>
• Gk passes: Passes Attempted (Excluding Goal Kicks). This column represents the total number of passes attempted by the goalkeeper, excluding goal kicks.
• Gk passes throws: Throws Attempted. This column denotes the total number of throws attempted by the goalkeeper.<br>
• Gk pct passes launched: Percentage of Passes that were Launched (Excluding Goal Kicks and Passes Longer than 40 Yards). This column calculates the percentage 
of passes (excluding goal kicks) that were longer than 40 yards and launched by the goalkeeper.<br>
• Gk passes length avg: Average Length of Passes (in Yards, Excluding Goal Kicks). This column represents the average length of passes made by the goalkeeper, excluding goal kicks.
• Gk goal kicks: Goal Kicks Attempted. This column denotes the total number of goal kicks attempted by the goalkeeper.<br>
• Gk pct goal kicks launched: Percentage of Goal Kicks that were Launched (Passes Longer than 40 Yards). This column calculates the percentage of goal kicks that 
were longer than 40 yards and launched by the goalkeeper.<br>
• Gk goal kick length avg: Average Length of Goal Kicks (in Yards). This column represents the average length of goal kicks taken by the goalkeeper.<br>
• Gk crosses: Opponent's Attempted Crosses into Penalty Area. This column denotes the total number of crosses attempted by the opponent into the penalty area.<br>
• Gk crosses stopped: Number of Crosses into Penalty Area Successfully Stopped by the Goalkeeper. This column represents the number of crosses into the penalty 
area that were successfully stopped by the goalkeeper.<br>
• Gk crosses stopped pct: Percentage of Crosses into Penalty Area Successfully Stopped by the Goalkeeper. This column calculates the percentage of crosses into the 
penalty area that were successfully stopped by the goalkeeper.<br>
• Gk def actions outside pen area: Number of Defensive Actions Outside of Penalty Area. This column denotes the number of defensive actions performed by the goalkeeper 
outside of the penalty area.<br>
• Gk def actions outside pen area per90: Defensive Actions Outside of Penalty Area per 90 Minutes. This column represents the average number of defensive actions 
performed by the goalkeeper outside of the penalty area per 90 minutes of play.<br>
• Gk avg  distance def actions: Average Distance from Goal (in Yards) of All Defensive Actions. This column represents the average distance from the goal of all 
defensive actions performed by the goalkeeper.<br>
• Shots: Total Shots (Excluding Penalty Kicks). This column represents the total number of shots taken, excluding penalty kicks.<br>
• Shots on target: Shots on Target (Excluding Penalty Kicks). This column denotes the total number of shots that were on target, excluding penalty kicks. 
Note: Shots on target do not include penalty kicks.<br>
• Shots on target pct: Percentage of Shots on Target. This column represents the percentage of shots that are on target. To qualify as a leader, a minimum of .395 
shots per squad game is required. Note: Shots on target do not include penalty kicks.<br>
• Shots per90: Total Shots per 90 Minutes. This column denotes the average number of shots taken per 90 minutes of play. To qualify as a leader, a minimum of 
30 minutes played per squad game is required.<br>
• Shots on target per90: Shots on Target per 90 Minutes. This column represents the average number of shots on target per 90 minutes of play. To qualify 
as a leader, a minimum of 30 minutes played per squad game is required. Note: Shots on target do not include penalty kicks.<br>
• Goals per shot: Goals per Shot. This column calculates the average number of goals scored per shot taken. To qualify as a leader, a minimum of .395 
shots per squad game is required.<br>
• Goals per shot on target: Goals per Shot on Target. This column represents the average number of goals scored per shot on target. To qualify as a leader, 
a minimum of .111 shots on target per squad game is required. Note: Shots on target do not include penalty kicks.<br>
• Average shot distance: Average Distance from Goal (in Yards) of All Shots Taken. This column denotes the average distance from the goal of all shots taken. 
To qualify as a leader, a minimum of .395 shots per squad game is required. This metric does not include penalty kicks.<br>
• Shots free kicks: Shots from Free Kicks. This column represents the number of shots taken from free kicks.<br>
• Npxg per shot: Non-Penalty Expected Goals per Shot. This column calculates the expected goals per shot, excluding penalty kicks. To qualify as a leader,
a minimum of .395 shots per squad game is required.<br>
• Xg net: Goals minus Expected Goals. This column represents the difference between the actual goals scored and the expected goals. xG totals include 
penalty kicks but do not include penalty shootouts. An underline indicates that there is a match missing data, which will be updated when available.<br>
• Npxg net: Non-Penalty Goals minus Non-Penalty Expected Goals. This column calculates the difference between the non-penalty goals scored and the 
non-penalty expected goals. xG totals include penalty kicks but do not include penalty shootouts. An underline indicates that there is a match missing data, 
which will be updated when available.<br>
• Passes completed: Passes Completed. This column denotes the total number of passes successfully completed.<br>
• Passes: Passes Attempted. This column represents the total number of passes attempted.<br>
• Passes pct: Pass Completion Percentage. This column calculates the percentage of passes successfully completed. To qualify as a leader, a minimum of 
30 minutes played per squad game is required.<br>
• Passes total distance: Total Distance of Completed Passes. This column represents the total distance, in yards, that completed passes have traveled in any direction.<br>
• Passes progressive distance: Progressive Distance of Completed Passes. This column denotes the total distance, in yards, that completed passes have traveled 
towards the opponent's goal. Note that passes away from the opponent's goal are counted as zero progressive yards.<br>
• Passes completed short: Passes Completed (Short Passes). This column represents the number of passes completed between 5 and 15 yards.
• Passes short: Passes Attempted (Short Passes). This column denotes the total number of passes attempted between 5 and 15 yards.<br>
• Passes pct short: Pass Completion Percentage (Short Passes). This column calculates the percentage of short passes (between 5 and 15 yards) 
that were successfully completed. To qualify as a leader, a minimum of 30 minutes played per squad game is required.<br>
• Passes completed medium: Passes Completed (Medium Passes). This column represents the number of passes completed between 15 and 30 yards.
• Passes medium: Passes Attempted (Medium Passes). This column denotes the total number of passes attempted between 15 and 30 yards.<br>
• Passes pct medium: Pass Completion Percentage (Medium Passes). This column calculates the percentage of medium passes (between 15 and 30 yards) 
that were successfully completed. To qualify as a leader, a minimum of 30 minutes played per squad game is required.<br>
• Passes completed long: Passes Completed (Passes longer than 30 yards). This column represents the number of passes longer than 30 yards that were successfully completed.<br>
• Passes long: Passes Attempted (Passes longer than 30 yards). This column denotes the total number of passes longer than 30 yards attempted.<br>
• Passes pct long: Pass Completion Percentage (Passes longer than 30 yards). This column calculates the percentage of passes longer than 30 yards that 
were successfully completed. To qualify as a leader, a minimum of 30 minutes played per squad game is required.<br>
• Pass xa: Expected Assists. This column represents the likelihood that each completed pass becomes an assist in terms of goal probability. It considers 
factors such as pass type, phase of play, location, and distance. To qualify as a leader, a minimum of 30 minutes played per squad game is required.<br>
• Xg assist net: Assists minus Expected Goals Assisted. This column represents the difference between the number of assists and the expected goals assisted. 
It quantifies the effectiveness of an assist in creating more goals than expected. Provided by Opta.<br>
• Assisted shots: Passes that directly lead to a shot (assisted shots). This column represents the number of passes that directly lead to a shot taken by another player.<br>
• Passes into final third: Completed passes that enter the final third of the pitch closest to the opponent's goal. This column denotes the number of passes played
into the final third of the field. It does not include set pieces.<br>
• Passes into penalty area: Completed passes into the opponent's penalty area. This column represents the number of passes played into the 18-yard box. It does 
not include set pieces.<br>
• Crosses into penalty area: Completed crosses into the opponent's penalty area. This column represents the number of crosses attempted into the 18-yard box. 
It does not include set pieces.<br>
• Progressive passes: Progressive Passes. This column denotes the number of completed passes that move the ball towards the opponent's goal by at least 10 
yards from its furthest point in the last six passes or any completed pass into the penalty area. It excludes passes from the defending 40% of the pitch.<br>
• Passes live: Live-ball passes. This column represents the number of passes that are played while the ball is in play during the course of the game.<br>
• Passes dead: Dead-ball passes. This column represents the number of passes that are played from free kicks, corner kicks, kick-offs, throw-ins, and goal kicks.<br>
• Passes free kicks: Passes attempted from free kicks. This column denotes the number of passes attempted from free kick situations.<br>
• Through balls: This column represents the number of passes that penetrate the defensive line and create opportunities for attackers.<br>
• Passes switches: Passes that travel more than 40 yards of the width of the pitch. This column represents the number of passes that switch the play 
from one side of the field to the other.<br>
• Crosses: This column denotes the total number of crosses attempted.<br>
• Throw ins: This column represents the number of throw-ins taken by the player.<br>
• Corner kicks: This column represents the total number of corner kicks taken by the player.<br>
• Corner kicks in: This column represents the number of corner kicks taken with an in swinging trajectory.<br>
• Corner kicks out: This column represents the number of corner kicks taken with an out swinging trajectory.<br>
• Corner kicks straight: This column represents the number of corner kicks taken with a straight trajectory.<br>
• Passes off sides: This column represents the number of passes played to teammates who were in an offside position.<br>
• Passes blocked: This column represents the number of passes that were blocked by opponents who were standing in the passing lane.<br>
• Sca: (Shot-Creating Actions) This column represents the total number of offensive actions directly leading to a shot attempt, including passes, dribbles, and drawing fouls. 
Note that a single player can receive credit for multiple actions, and the shot-taker can also receive credit.<br>
• Sca per90: (Shot-Creating Actions per 90 minutes) This column calculates the rate of shot-creating actions per 90 minutes of play. To qualify as a leader, 
a minimum of 30 minutes played per squad game is required.<br>
• Sca passes live: (Completed live-ball passes that lead to a shot attempt) This column represents the number of completed passes during live play that directly lead to a shot attempt.<br>
• Sca passes dead: (Completed dead-ball passes that lead to a shot attempt) This column represents the number of completed passes from free kicks, corner kicks, 
kick-offs, throw-ins, and goal kicks that directly lead to a shot attempt.<br>
• Sca dribble: (Successful dribbles that lead to a shot attempt) This column represents the number of successful dribbles that directly lead to a shot attempt.<br>
• Sca shots: (Shots that lead to another shot attempt) This column represents the number of shots taken that result in another shot attempt.<br>
• Sca fouled: (Fouls drawn that lead to a shot attempt) This column represents the number of fouls drawn by a player that directly lead to a shot attempt.<br>
• Sca defense: (Defensive actions that lead to a shot attempt) This column represents the number of defensive actions by a player that directly lead to a shot attempt.<br>
• Gca :(Goal-Creating Actions. This column represents the total number of offensive actions directly leading to a goal, such as passes, dribbles, and drawing fouls. 
Note that a single player can receive credit for multiple actions, and the shot-taker can also receive credit.<br>
• gca_per90: Goal-Creating Actions per 90 minutes. This column calculates the rate of goal-creating actions per 90 minutes of play. To qualify as a leader, 
a minimum of 30 minutes played per squad game is required.<br>
• gca_passes_live: Completed live-ball passes that lead to a goal. This column represents the number of completed passes during live play that directly lead to a goal.<br>
• gca_passes_dead: Completed dead-ball passes that lead to a goal. This column represents the number of completed passes from free kicks, corner kicks, kick-offs, 
throw-ins, and goal kicks that directly lead to a goal.<br>
• gca_dribbles: Successful dribbles that lead to a goal. This column represents the number of successful dribbles that directly lead to a goal.<br>
• gca_shots: Shots that lead to another goal-scoring shot. This column represents the number of shots taken that result in another shot attempt resulting in a goal.<br>
• gca_fouled: Fouls drawn that lead to a goal. This column represents the number of fouls drawn by a player that directly lead to a goal.<br>
• gca_defense: Defensive actions that lead to a goal. This column represents the number of defensive actions by a player that directly lead to a goal.
• tackles: Number of players tackled. This column represents the total number of successful tackles made by a player.
• tackles_won: Tackles in which the tackler's team won possession of the ball. This column represents the number of tackles made by a player where their 
team gained possession of the ball afterward.<br>
• tackles_def_3rd: Tackles in the defensive 1/3 of the field. This column represents the number of tackles made by a player in the defensive third of the field.<br>
• tackles_mid_3rd: Tackles in the middle 1/3 of the field. This column represents the number of tackles made by a player in the middle third of the field.<br>
• tackles_att_3rd: Tackles in the attacking 1/3 of the field. This column represents the number of tackles made by a player in the attacking third of the field.<br>
• dribble_tackles: Number of dribblers tackled. This column represents the total number of successful tackles made by a player against opponents attempting to dribble past them.<br>
• dribbles_vs: Number of times dribbled past plus number of tackles. This column represents the total number of times a player has been successfully dribbled past by an opponent, 
added to the number of successful tackles made by the player.<br>
• dribble_tackles_pct: Percentage of dribblers tackled. This column calculates the percentage of dribblers tackled by dividing the number of successful dribble tackles by the 
sum of successful dribble tackles and the number of times the player has been dribbled past. To qualify as a leader, a minimum of 0.625 dribblers contested per squad game is required.<br>
• dribbled_past: Number of times dribbled past by an opposing player. This column represents the total number of times a player has been successfully dribbled past by an opponent.<br>
• blocks: Number of times blocking the ball by standing in its path. This column represents the total number of times a player has successfully blocked the ball by positioning
themselves in its path.<br>
• blocked_shots: Number of times blocking a shot by standing in its path. This column represents the total number of shots blocked by a player by standing in the shooting player's path.<br>
• blocked_passes: Number of times blocking a pass by standing in its path. This column represents the total number of passes blocked by a player by standing in the passing lane.<br>
• interceptions: Interceptions. This column represents the total number of times a player successfully intercepted a pass or ball from the opponent.<br>
• tackles_interceptions: Number of players tackled plus number of interceptions. This column represents the sum of successful tackles made by a player and the number of 
interceptions they have made.<br>
• clearances: Clearances. This column represents the total number of times a player successfully cleared the ball from their own defensive area.<br>
• errors: Mistakes leading to an opponent's shot. This column represents the number of mistakes made by a player that directly resulted in an opponent having a shot opportunity.<br>
• touches: Number of times a player touched the ball. This column represents the total number of times a player made contact with the ball during a match. Note that receiving a pass, 
dribbling, and then passing the ball counts as one touch.<br>
• touches_def_pen_area: Touches in the defensive penalty area. This column represents the number of times a player touched the ball while inside their team's defensive penalty area.<br>
• touches_def_3rd: Touches in the defensive 1/3 of the field. This column represents the number of times a player touched the ball while in the defensive third of the field.<br>
• touches_mid_3rd: Touches in the middle 1/3 of the field. This column represents the number of times a player touched the ball while in the middle third of the field.<br>
• touches_att_3rd: Touches in the attacking 1/3 of the field. This column represents the number of times a player touched the ball while in the attacking third of the field.<br>
• touches_att_pen_area: Touches in the attacking penalty area. This column represents the number of times a player touched the ball while inside the opponent's penalty area.<br>
• touches_live_ball: Live-ball touches. This column represents the number of times a player touched the ball during live play, excluding corner kicks, free kicks, throw-ins,
kick-offs, goal kicks, or penalty kicks.<br>
• dribbles_completed: Dribbles Completed Successfully. This column represents the total number of successful dribbles completed by a player.<br>
• dribbles: Dribbles Attempted. This column represents the total number of dribble attempts made by a player.<br>
• dribbles_completed_pct: Percentage of Dribbles Completed Successfully. This column calculates the percentage of dribbles completed successfully by dividing the 
number of successful dribbles by the total number of dribble attempts. To qualify as a leader, a minimum of 0.5 dribbles per squad game is required.<br>
• miscontrols: Number of times a player failed when attempting to gain control of a ball. This column represents the total number of times a player failed to gain 
control of the ball successfully.<br>
• dispossessed: Number of times a player loses control of the ball after being tackled by an opposing player. This column represents the total number of times a 
player lost possession of the ball due to being tackled by an opponent. It does not include attempted dribbles.<br>
• passes_received: Number of times a player successfully received a pass. This column represents the total number of passes that were successfully received by a player.<br>
• progressive_passes_received: Progressive Passes Received. This column represents the total number of passes received by a player that moved the ball towards the 
opponent's goal by at least 10 yards from its furthest point in the last six passes or any completed pass into the penalty area. It excludes passes from the defending 40% of the pitch.<br>
• minutes_per_game: Minutes Per Match Played. This column represents the average number of minutes played by a player per match.<br>
• minutes_pct: Percentage of Minutes Played. This column represents the percentage of the team's total minutes in which a player was on the pitch. 
It is calculated by dividing the player's minutes played by the team's total minutes played. To qualify as a leader, a minimum of 30 minutes played per squad game is required.<br>
• minutes_per_start: Minutes Per Match Started. This column represents the average number of minutes played by a player in matches where they started. 
To qualify as a leader, a minimum of 30 minutes played per squad game is required.<br>
• games_complete: Complete matches played. This column represents the total number of matches in which a player played the full duration of the match.<br>
• games_subs: Games as a substitute. This column represents the total number of games in which a player did not start and came on as a substitute.<br>
• minutes_per_sub: Minutes Per Substitution. This column represents the average number of minutes played by a player per substitution. To qualify as a leader,
a minimum of 30 minutes played per squad game is required.<br>
• unused_subs: Games as an unused substitute. This column represents the total number of games in which a player was named as a substitute but did not enter the match.<br>
• points_per_game: Points per Match. This column represents the average number of points earned by the team from matches in which the player appeared. To qualify as a leader, 
a minimum of 30 minutes played per squad game is required.<br>
• on_goals_for: Goals scored by the team while the player was on the pitch. This column represents the total number of goals scored by the player's team while the player was on 
the field.<br>
• on_goals_against: Goals allowed by the team while the player was on the pitch. This column represents the total number of goals conceded by the player's team while the player 
was on the field.<br>
• plus_minus: Plus/Minus. This column represents the goal differential while the player was on the pitch. It is calculated by subtracting the goals conceded by the player's team
from the goals scored by the team.<br>
• plus_minus_per90: Plus/Minus per 90 Minutes. This column represents the goal differential per 90 minutes played while the player was on the pitch. It is calculated by dividing
the plus/minus value by the player's total minutes played and multiplying it by 90. To qualify as a leader, a minimum of 30 minutes played per squad game is required.<br>
• on_xg_for: Expected goals by the team while the player was on the pitch. This column represents the total expected goals scored by the player's team while the player was 
on the field. The expected goals (xG) totals include penalty kicks but do not include penalty shootouts (unless otherwise noted). The data is provided by Opta. An underline 
indicates that there is a match missing data, but it will be updated when available.<br>
• on_xg_against: Expected goals allowed by the team while the player was on the pitch. This column represents the total expected goals conceded by the player's team while 
the player was on the field. The expected goals (xG) totals include penalty kicks but do not include penalty shootouts (unless otherwise noted). The data is provided by Opta. 
An underline indicates that there is a match missing data, but it will be updated when available.<br>
• xg_plus_minus: Expected Goals Plus/Minus. This column represents the difference between expected goals scored and expected goals allowed by the team while the player was 
on the pitch. The expected goals (xG) totals include penalty kicks but do not include penalty shootouts (unless otherwise noted). The data is provided by Opta. An underline 
indicates that there is a match missing data, but it will be updated when available.<br>
• xg_plus_minus_per90: Expected Goals Plus/Minus per 90 Minutes. This column represents the expected goals plus/minus per 90 minutes played while the player was on the pitch. 
It is calculated by dividing the xG plus/minus value by the player's total minutes played and multiplying it by 90. The expected goals (xG) totals include penalty kicks but 
do not include penalty shootouts (unless otherwise noted). To qualify as a leader, a minimum of 30 minutes played per squad game is required.<br>
• cards_yellow_red: Second Yellow Card. This column represents the number of times a player received a second yellow card in a match, resulting in a red card.<br>
• fouls: Fouls Committed. This column represents the total number of fouls committed by a player.<br>
• fouled: Fouls Drawn. This column represents the total number of fouls drawn by a player.<br>
• offsides: Offsides. This column represents the total number of times a player was caught in an offside position.<br>
• pens_won: Penalty Kicks Won. This column represents the total number of penalty kicks won by a player.<br>
• pens_conceded: Penalty Kicks Conceded. This column represents the total number of penalty kicks conceded by a player's team.<br>
• own_goals: Own Goals. This column represents the total number of own goals scored by a player.<br>
• ball_recoveries: Number of loose balls recovered. This column represents the total number of loose balls recovered by a player.<br>
• aerials_won: Aerials won. This column represents the total number of aerial duels won by a player.<br>
• aerials_lost: Aerials lost. This column represents the total number of aerial duels lost by a player.<br>
• aerials_won_pct: Percentage of aerials won. This column represents the percentage of aerial duels won by a player. It is calculated by dividing 
the number of aerial duels won by the sum of aerial duels won and aerial duels lost. To qualify as a leader, a minimum of 0.97 aerial duels per squad game is required.<br>

<h1>Data Sources:</h1>
The data use for this project available from the kaggle. Which  contain information on group, team, golas,etc.


<h1>Technology used:</h1>
SQL: For querying of the analysis include.<br>
Tableau: For data visualization.<br>
Pandas: For data cleaning.<br>


<h1>Tasks:</h1>
1.	Data cleaning and preparation: Clean and pre process the data by handling missing values, data formatting.<br>
2.	Data Analysis: Perform descriptive statistics and data visualization to identify trends, patterns and correlations.<br>
3.	SQL Querying: Write a SQL Queries to retrieve specific data, perform aggregation and join tables.<br>
4.	Insight Generation: Generate actionable insights and recommendations based on the analysis.<br>



<h1>Insights and Findings:</h1>

•	Highest wins group: First No: Group 8 led with the highest wins by teams Uruguay.<br> 
Second No:  Group 8 led with the highest wins by teams Portugal.<br>
Third No:  Group 8 led with the highest wins by teams Korea Republic.<br>

•	Expected Goals scored with Team: First No: Germany scored 10.100 in group 5.<br>
Second No: France scored 7.200 in group 4.<br> 
Third No: Argentina 6.000 in group 3. <br>

•	Most fouls: First No: Group:3, Team: Argentina, Fouls:100.<br>
 Second No: Group:6, Team: Morocco, Fouls:96. <br>
Third No: Group:6, Team: Croatia, Fouls:90.<br>

•	Clean sheets: First No: Team: Morocco, Clean sheet: 4, Matches played:3.<br> 
Second No: Team: England, Clean sheet: 3, Matches played:3.<br>
Third No: Team: Argentina, Clean sheet: 3, Matches played:3.<br>

•	Youngest average age: First No: Team: Costa Rica, Average Age: 30, Played used: 22.<br> 
Second No: Team: Belgium, Average Age: 30, Played used: 20.<br> 
Third No: Team: Croatia, Average Age: 29, Played used:21.<br>

•	High possession: First No: Team: Croatia, Ball Recoveries: 409.<br>
Second No: Team: Morocco, Ball Recoveries: 369.<br>
 Third No: Team: France, Ball Recoveries: 369. <br>
 
•	Shots on target: First No: Team: Argentina, Shots on target: 41. <br>
Second No: Team: Brazil, Shots on target: 40.<br> 
Third No: Team:  France, Shots on target: 33.<br>
 
•	Expected goals: First No: Team: Germany, Expected Goal Score: 10,100.<br> 
Second No: Team: France, Expected Goal Score: 7.200.<br>
 Third No: Team: Argentina, Expected Goal Score: 6.000.<br>
 
•	Passing efficiency: First No: Group: 3, Passes Completed Short: 2131.<br> 
Second No: Group: 6, Passes Completed Short: 1911. <br>
Third No: Group: 4, Passes Completed Short: 1484.<br>

•	Penalty saves: First No: Team: Croatia, Crosses into penalty area: 22. <br>
Second No: Team: France, Crosses into penalty area: 20.<br>
Third No: Team: Portugal, Crosses into penalty area:14.<br>



