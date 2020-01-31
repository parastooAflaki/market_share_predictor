# market_share_predictor
## Summary of work
#### to keep track of the work please review the notebooks in the following order:
### 1. Dats_Analysis.ipynb :
analysing data and deciding which unnecessary features to drop
### 2. Train_Model.ipynb :
Preprocessing the train data and evaluate different models (using 70% of train data for training and the rest 30% for testing the model) and compared their r2 score and mae to choose the best.
as a result, the ensemble model __RandomForestRegressor__ is the best model for us.
#### result table :
| Model | R2 Score | MAE | CV R2-Score |
|:---:|:---:|:---:|:---:|
| __RandomForestRegressor__  |  0.9006 | 0.9263  | 0.8946 (+/-) 0.0015 |

### 3. Test_Prediction.ipynb :
Preprocessing train and test data, training the __RandomForestRegressor__ model on train data and then predict the test data.

the final prediction is saved in __test_prediction.csv__ file.

## Requirments :
* sklearn
* pandas
* numpy
* matplotlib
