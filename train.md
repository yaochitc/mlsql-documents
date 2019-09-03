### Example
train train_data as GBTRegressor.`/tmp/model` where

-- once set true,every time you run this script, MLSQL will generate new directory for you model
keepVersion="true"

-- specicy the test dataset which will be used to feed evaluator to generate some metrics e.g. F1, Accurate
and evaluateTable="eval_data"

-- specify group 0 parameters
and `fitParam.0.featuresCol`="features"
and `fitParam.0.labelCol`="label"
and `fitParam.0.maxDepth`="5"
and `fitParam.0.maxBins`="32"
and `fitParam.0.minInstancesPerNode`="1"
and `fitParam.0.minInfoGain`="0"
and `fitParam.0.cacheNodeIds`="false"
and `fitParam.0.checkpointInterval`="10"
and `fitParam.0.subsamplingRate`="1"
and `fitParam.0.maxIter`="20";