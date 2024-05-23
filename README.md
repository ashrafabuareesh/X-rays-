# X-rays-
![download](https://github.com/ashrafabuareesh/X-rays-/assets/123064338/c3389bd6-8917-4eb8-a1e3-aad4ef6d2d40)

* For this assignment, you will classify chest X-rays as "normal," "pneumonia," or "covid" using Convolutional Neural Networks.


# Context
* X-ray samples of COVID-19 were retrieved from different sources for the unavailability of a large specific dataset. Firstly, a total 1401 samples of COVID-19 were collected using GitHub repository [1] , [2] , the Radiopaedia [3] , Italian Society of Radiology (SIRM) [4] , Figshare data repository websites [5] , [6] . Then, 912 augmented images were also collected from Mendeley instead of using data augmentation techniques explicitly [7] . Finally, 2313 samples of normal and pneumonia cases were obtained from Kaggle [8] , [9] .
* Data : https://www.kaggle.com/datasets/amanullahasraf/covid19-pneumonia-normal-chest-xray-pa-dataset?resource=download


# Comparison of Model Performance
* Two models have been evaluated for classifying chest X-ray images into three categories: "normal," "pneumonia," and "covid." Let's compare the performance metrics of the initial model and the VGG-16 model.


## Initial Model: 
*  Classification Metrics: Test Data
----------------------------------------------------------------------
              precision    recall  f1-score   support

           0       0.91      0.94      0.92       221
           1       0.87      0.85      0.86       251
           2       0.89      0.88      0.89       222

    accuracy                           0.89       694



## VGG-16 Model: 
 Classification Metrics: Test Data
----------------------------------------------------------------------
              precision    recall  f1-score   support

           0       0.96      0.98      0.97       215
           1       0.89      0.96      0.93       253
           2       0.99      0.88      0.93       226

    accuracy                           0.94       694

## Summary of Comparison
### Precision:
* Initial Model:

  * Class 0 (normal): 0.91
  * Class 1 (pneumonia): 0.87
  * Class 2 (covid): 0.89
  * Weighted average: 0.89
* VGG-16 Model:

    * Class 0 (normal): 0.96
    * Class 1 (pneumonia): 0.89
    * Class 2 (covid): 0.99
    * Weighted average: 0.95
### Recall:
* Initial Model:

   * Class 0 (normal): 0.94
   * Class 1 (pneumonia): 0.85
   * Class 2 (covid): 0.88
   * Weighted average: 0.89
* VGG-16 Model:

  * Class 0 (normal): 0.98
  * Class 1 (pneumonia): 0.96
  * Class 2 (covid): 0.88
   * Weighted average: 0.94
### F1-Score:
* Initial Model:

  * Class 0 (normal): 0.92
  * Class 1 (pneumonia): 0.86
  * Class 2 (covid): 0.89
  * Weighted average: 0.89
* VGG-16 Model:

  * Class 0 (normal): 0.97
  * Class 1 (pneumonia): 0.93
  * Class 2 (covid): 0.93
  * Weighted average: 0.94
* Overall Accuracy:
  * Initial Model: 0.89
  * VGG-16 Model: 0.94
# Summary
* The VGG-16 model outperforms the initial model in all key metrics:

* Precision: The VGG-16 model has higher precision for all classes, especially for "normal" and "covid" categories.
* Recall: The VGG-16 model shows significant improvement in recall for the "normal" and "pneumonia" categories.
* F1-Score: The F1-score, which is the harmonic mean of precision and recall, is higher for all classes in the VGG-16 model.
* Accuracy: The overall accuracy of the VGG-16 model is higher at 0.94 compared to 0.89 for the initial model.
The improved performance of the VGG-16 model indicates it is more effective at accurately classifying chest X-ray images into the specified categories.
