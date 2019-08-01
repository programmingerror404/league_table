# league_table
Ranking players in a league by sorting the contents

The LeagueTable class tracks the score of each player in a league. After each game, the player records their score with the recordResult function. 
The player's rank in the league is calculated using the following logic:
The player with the highest score is ranked first (rank 1). The player with the lowest score is ranked last.
If two players are tied on score, then the player who has played the fewest games is ranked higher.
If two players are tied on score and number of games played, then the player who was first in the list of players is ranked higher.
Implement the playerRank function that returns the player at the given rank.

```
  For example:
  $table = new LeagueTable(array('Mike', 'Chris', 'Arnold'));
  $table->recordResult('Mike', 2);
  $table->recordResult('Mike', 3);
  $table->recordResult('Arnold', 5);
  $table->recordResult('Chris', 5);
  echo $table->playerRank(1);
  All players have the same score. However, Arnold and Chris have played fewer games than Mike, and as Chris is before Arnold in the list of players, he is ranked first. Therefore, the code above should display "Chris".
```
