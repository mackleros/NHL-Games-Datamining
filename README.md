# NHL-Games-Datamining
Using some data mining approaches to examine statistics from NHL Games

## Question:

Can we identify what the most important statistics for winning games are, other than scoring goals? For example: Is face off win%, shots on goal and takeaways among the most important things in order to win games? 

By “most important statistics”, we mean the statistics that are most effective in increasing win chances for a team if they are improved, and perhaps if a combination of certain statistics shows to be important. Data mining approaches such as feature selection and association rule mining can help answer these questions more effectively than correlation analysis, since their more exploratory nature could help uncover patterns and connections that might not be found otherwise. 

This research question is relevant because it could be used to see what areas a team would want to improve in order to win more games. For example, if it’s identified that being good in certain metrics leads to high win percentage, the coach of a team can make informed decisions about what statistics the team should focus on and what they should practice in order to win more games. Perhaps the coach could also tailor the tactics in order to improve the identified key statistics. Let’s say that we find shot blocking and power play percentage to be key factors in winning games. It would suggest to a coach that these areas should be in focus during practice and that you’d want to find tactics to minimize your opponents success in these statistics (e.g. avoid shooting into blocks and have an effective boxplay).


## Method

The data will have to be preprocessed to remove data points with missing values and synthesize data such as power play percentage.  Feature selection will be used to find the metrics that can be used to predict whether games are won or lost. 

Association rule mining will be used to see relationships in the data, for this we might have to preprocess the data so that we get some binary data for shots, blocks, giveaways/takeaways etc. For example: “shots: won/lost” (e.g. if the team shot more or less shots than the opponent), “blocks: won/lost”, “giveaway/takeaway-ratio: <0.5  or >0.5”. 

Once we believe we’ve found the most important statistics, we’ll use classification to see how well we can classify wins/losses with the metrics that have been selected.


## GRADING QUESTIONS



- [5] The chosen algorithm is appropriate (motivate the choice with respect to the
features of the data).


- [5] For the chosen algorithm, computational reductions, measures, approximations (e.g.
appropriate proximity function, addressing correlation issues, ...) are motivated.


- [5] Modelling bias and errors (e.g. noise, overfitting, class imbalance) has been
addressed.


- [5] A good validation / evaluation test has been generated.


- [5] The results are supported by sufficient evidence (large leaf sizes, high support, ...).


- [5] The results have been interpreted, and related to the original problem (Was the
problem solved? How can the results be used? Have any new hypotheses been
generated?