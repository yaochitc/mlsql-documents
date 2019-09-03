### Example
register GBTRegressor.`/tmp/model/model/0/` as  rf_predict;
select rf_predict(features) as predict_label, label from data limit 10
as output;