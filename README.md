# LSTM Time Series - Multivariate Stock Price Prediction
This project implements a time series multivariate analysis using RNN/LSTM for stock price predictions. A deep RNN model was created and trained on five years of historical Google stock price data to forecast the stock performance over a two-month period.

## Google Stock Price Dataset 
This dataset comprises historical records for the stock price of Google's Alphabet captured on daily basis.

Initially, the entire dataset was explored and then a specific time period was selected to perform training, validation, and predictions as follows:

- **Training data:** from Jan 2019 till June 2023.
- **Validation data:** from July 2023 till Dec 2023.
- **Testing data:** first two months of 2024.

The initial, filtered and preprocessed datasets can be located in their corresponding subfolders in the Datasets used.


### Segment 1 - Explanatory Data Analysis

The dataset was explored and all the summary and statistics was studied. Initial data cleaning was done and after analyzing the stock performance , the 5 year time frame was selected for analysis and then it was stored after filtering.


### Segment 2 - Data Preprocessing

The filtered dataset was used where firstly the independent and target features were selected and then they were scaled to [0,1] using MinMaxScaler and then seggregated for training, testing and validation dataset. These datasets were then stored independently.


### PHASE 3 - Model Training and Inference

The preprocessed dataset files (train, validate, test) were loaded and data structures were created by creating input sequences. The LSTM Model was built using TenserFlow Sequential and then trained and compiled. The model performance was evaluated on various datasets and inverse scaled to their original distribution. The Future stock prices were predicted and visualized.

