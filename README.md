# Fifa_wc_2018_prediction
# We have predicted the world cup winner along with the semi finalists.
# We have collected data from reddit blogs, official EA player ratings, official FIFA website.
# we have used player rankings, player performance statistics, historical betting odds and even used fan-sentiment variables 
# To avoid overfitting, we didnot use any hostoric World cup data and gave more importance to player recent form and career statistic.
# Since the data for worldcup performances was limited for most of the players, we trained the model using crossvalidation
# We tried buidling the model using decision trees, but the model was very overfitting and bias-variance tradeoff was high
# Hence we decided to go with Random forests.
# We have achieved a R-square of 0.67 and the model predictions are below

#Last 16				
Team 1	Team 2	Result	pvalue	Build_Accuracy
France 	Argentina	 1	0.01	0.76
Uruguay	Portugal	2	0.016	0.78
Spain 	Russia	1	0.01	0.76
Croatia	Denmark	1	0.02	0.68
Brazil	Mexico	1	0.0023	0.89
Belgium	Japan	1	0.017	0.74
Sweden	Switzerland	1	0.021	0.67
Colombia	England	2	0.027	0.63
				
Quarters				
Team 1	Team 2	Result	pvalue	Build_Accuracy
France 	Portugal	1	0.065	0.63
Belgium	Brazil	2	0.074	0.61
England 	Sweden	2	0.15	0.52
Spain	Croatia	1	0.017	0.74
				
Semis				
Team 1	Team 2	Result	pvalue	Build_Accuracy
France	Brazil	1	0.034	0.67
Sweden	Spain	1	0.022	0.72
				
Finals				
Team 1	Team 2	Result	pvalue	Build_Accuracy
France	Spain	1	0.076	0.58
# Please go through the code in Fifa_WC.R for variable considerations and model selection
