## Overview of the analysis: 
`Alphabet Soup, a nonprofit foundation, seeks to optimize its funding process by identifying applicants most likely to succeed in their ventures. Given the foundation's mission and limited resources, it's crucial to allocate funds effectively to maximize positive outcomes. The foundation has provided a dataset containing metadata on over 34,000 organizations that have previously received funding. The challenge is to analyze this dataset to develop a tool that can predict the success of future applicants.`

Results: Using bulleted lists and images to support your answers, address the following questions:

## Data Preprocessing

__Features are Target variables__
* Features variables: `APPLICATION_TYPE`, `AFFILIATION`, `CLASSIFICATION`, `USE_CASE`, `ORGANIZATION`, `STATUS`, `INCOME_AMT`, `ASK_AMT`
- Target varible: `IS_SUCCESSFUL`

* Variables that were removed:  `EIN`, `Name`
    ![Features and Target Variables](https://github.com/mjardinico/deep-learning-challenge/blob/main/Resources/Images/application_df_drop2.png)

__Compiling, Taining, and Evaluating the Model__
* Initial model training:
    `During the initial model training, there were two hidden layers that were employed.The 'relu' activation function was used on both layers.`

    ![Model Training](https://github.com/mjardinico/deep-learning-challenge/blob/main/Resources/Images/model_structure.png)

* Evaluation of the initial Model:
    
    ![Evaluation of model training](https://github.com/mjardinico/deep-learning-challenge/blob/main/Resources/Images/accuracy_loss_1.png)

* Model Optimization: There are four hidden layers that were employed.
    `In the optimized model training, there were four hidden layers that were employed.The 'relu' activation function was used on all layers`

    ![Model Training Optimization](https://github.com/mjardinico/deep-learning-challenge/blob/main/Resources/Images/model_structure2.png)

* Evaluation of the Optimized Model:

    ![Evaluation of model training](https://github.com/mjardinico/deep-learning-challenge/blob/main/Resources/Images/accuracy_loss_2.png)


__SUMMARY__

`In efforts to enhance the model's accuracy, several adjustments were made including increasing the number of hidden layers from two to four and modifying the model's architecture by adjusting neuron counts in these layers. Additionally, a feature was removed to streamline the input data, and the activation function was switched from relu to tanh to explore different non-linear transformations. The cutoff value for binning rare occurrences in categorical variables was also adjusted. Despite these comprehensive modifications aimed at refining the model's learning capability, the alterations did not yield an improvement in the overall accuracy of the deep learning model.`

__Conclusion and Recommendations:__

`Despite various attempts to optimize the neural network model—including adjusting the number of hidden layers, altering neuron counts, changing activation functions, and refining data preprocessing techniques — no significant improvement in accuracy was observed. This outcome suggests that the challenges in enhancing model performance may not be obtained solely through architecture adjustments or data preprocessing strategies used thus far. There can be other alternative, such as using the deep learning regularization technique, which is a more advanced technique or other methods`

