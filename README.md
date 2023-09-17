## Abstract
In this study, we aimed to construct a deep learning classification model to recommend which discussion board a post should go to after a user has written it on the Cancer Survivors Network, which is a cancer-related public discussion forum. Additionally, we explored multiple types of models and compared their performance on this natural language processing task. We concluded that a stacked model, which was a combination of the Bidirectional LSTM and the transformer encoder outputs, provided the best results with an accuracy of 70.7%.

## Data
All data was pulled from the Cancer Survivors Network which resulted in a total of 27 classes. All classes with less than 1000 posts were dropped from the data set as the final accuracy was greatly affected by the classes with small amounts of data.
![](https://github.com/thomasdurkin/Classification-of-Cancer-Discussion-Posts/blob/master/Discussion_Board_Count_Bar_Chart.PNG)

## Models Tested
All models were created using PyTorch.
| model                    | accuracy |
| ------------------------ | -------- |
| Decision Tree (Baseline) | 56.0%    |     
| CNN                      | 63.1%    |
| RNN                      | 39.5%    |
| Bi-LSTM                  | 68.7%    |
| Transformer              | 67.9%    | 
| Stacked Model            | 70.7%    | 

## Results
Below is the confusion matrix for the best model.
![](https://github.com/thomasdurkin/Classification-of-Cancer-Discussion-Posts/blob/master/Confusion_Matrix_For_Best_Model.PNG)
