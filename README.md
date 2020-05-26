# prohack
McKinsey Prohack

Only two steps prevent us from achieving singularity
· To understand what makes us better off.
Our elders used the composite index to measure our well-being performance, but this knowledge has disappeared in the sands of time.
Use our data and train your model to predict this index with the highest possible level of certainty.
· To achieve the highest possible level of well-being through optimized allocation of additional energy
We have discovered the star of an unusually high energy of 50000 zillion DSML.
We have agreed between ourselves that 
· no one galaxy will consume more than 100 zillion DSML 
and 
· at least 10% of the total energy will be consumed by galaxies in need with existence expectancy index below 0,7.

________________________________________________

The solutions are evaluated on two criteria: predicted future Index values and allocated energy from a newly discovered star
1) Index predictions are evaluated using RMSE metric
2) Energy allocation is also evaluated using RMSE metric and has a set of known factors that need to be taken into account.
Every galaxy has a certain limited potential for improvement in the index described by the following function:
Potential for increase in the Index = -np.log(Index+0.01)+3
Likely index increase dependent on potential for improvement and on extra energy availability is described by the following function:
Likely increase in the Index = extra energy * Potential for increase in the Index **2 / 1000
There are also several constraints:
in total there are 50000 zillion DSML available for allocation and no galaxy at a point in time should be allocated more than 100 zillion DSML or less than 0 zillion DSML. Galaxies with low existence expectancy index below 0.7 should be allocated at least 10% of the total energy available in the foreseeable future
3) Leaderboard is based on a combined scaled metric:
80% prediction task RMSE + 20% optimization task RMSE * lambda where lambda is a normalizing factor
4) Leaderboard is 80% public and 20% private
5) The submission should be in the following format:
Index - Unique index from the test dataset in the ascending order
pred - Prediction for the index on interest
opt_pred - Optimal energy allocation
