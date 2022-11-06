# Neural Network Charity Analysis

## Overview
  Analysis was done to determine the differences between traditional machine learning classification/regression models, and the neural network models. TensorFlow was used to implement a neural network, and help to explain how different neural network structures would change algorithm performance.
  
  The Alphabet Soup foundation is using the above to predict where to make investments.

## Results

  - Data Preprocessing
    - What variables are considered the targets of the model?
      The target viaribale is the "IS_SUCCESSFUL" column based on the data, as this indicates prior successful investments.
      
    - What variables are considered the features of the model?
      The feature is the "Is_Successful" column, as this is what we are looking more closely at.
      
    - What variables are neither features or targets, and should be removed from the input data?
      The EIN and NAME columns don't do anything to support the accuracy of the model, and these are removed from the input data.
      
  - Compliling, Training, and Evaluating the Model
    - How many neurons, layers, and activation functions were selected for the model and why?
      In the optimized model, layer 1 started with 120 neurons with a relu activation. For layer 2, it dropped to 80 neurons and continued with the relu activation. From there, the sigmoid activation seemed to be the better fit for layers 3 (40 neurons) and layer 4 (20 neurons).

    - Was the target model performance acheived?
      No, the best the model would do is 72%, whereas the target was 75%.

    - What steps were taken to try and increase the model performance?
      Columns were reviewed, with other superfluous columns being dropped - Status and Special_considerations. Other activations were tried, but produced lower results.

## Summary
  The relu and sigmoid activators performed best, but still missing target. Longer training epochs or a random forest classifier would help with handling outliers and get better performance.
