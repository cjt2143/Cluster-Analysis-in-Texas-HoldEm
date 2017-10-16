# Cluster-Analysis-in-Texas-HoldEm
Project Description:
The program allows a user to play Texas Hold 'Em against the computer. The computer will not have access to the player's hand until after the winner for that hand is determined.  After each hand, the program calculates each player's probability of winning (based on their hand) at each point of the hand,i.e pre-flop, flop, turn, river. This value is said to be the true value of the hand. The program then creates the following ratio for each player for each round of the hand:  % of pot bet to calculated true value (ie. there will be 4 points generated for each player after each hand ends).  These points (x,y)=(% of pot bet, ratio) are plotted on a separate graph for each player.  After a pre-determined amount of turns, the computer takes this generated, unstructured data and employs cluster analysis.  With the elbow method, the amount of clusters will be determined.  With k-means clustering, the center of each cluster will be determined.  Now with this structured data, the computer can predict the true % chance of an opponent's hand winning based on their % bet during the hand and the center of the appropriate cluster(s) (y value ie ratio): % true = % of pot bet*1/(weighted avg of ratio).  The computer can then decide to fold or call more intelligently for the hand.  When the hand is over, the program creates a new data point in the graph as described above and re-adjusts the clusters accordingly.  In short, during a hand the computer uses the graph to make predictions based on the players past behavior and after the hand ends, the computer updates the graph which will increase the accuracy of the predictions.   

Included in code here:
-ability for real people to play against each other
-determines who won each hand
-finds the % of pot bet each round
-probability of each player winning given their starting hand
-probability of a player getting each of the possible hand types given flop
 
In progress & to be added:
-probability a player gets each kind of hand at turn
-probability of a player winning at each round
-plot of data points
-k-means clustering on data (code will be from outside source)

