### Rock paper scissors:
* Playing against four different bots with four different strategies.

### Result:
* The proposed strategy wins at with a win rate of at least 69% in 1000 matches against each bot.

### Strategy:
* Using multiple strategies with a scoring system to decide the best strategy to follow in each round.
* The score of each strategy gets updated each round.
#### Strategies:
1. Random choice using random.choice function to choose from three options shuffled each round.  
2. Semi random choice using random.choice function to choose from two options based on the opponent previous play.
3. Pattern generation based on the opponent previous play.
4. Pattern generation based on the my previous play.
5. Using the previous round plays, predicts the best next play based on the score. The score table is updated each round. ex: my previous play is R and opponent play(state) is S so based on the score it chooses the maximum between RSR, RSP and RSS to decide the next play(action). the score of a the state-action pair is 0 for a win, -1 for a tie and -2 for a defeat.
