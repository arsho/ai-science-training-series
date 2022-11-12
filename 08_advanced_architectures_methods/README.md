# Advanced AI Architectures and Methods

AI-Driven Science on Supercomputers @ ALCF 2022

**Contact:** Venkat Vishwanath ([venkat@anl.gov](mailto:///venkat@anl.gov)), Bethany Lusch ([blusch@anl.gov](mailto:///blusch@anl.gov)), Carlo Graziani ([cgraziani@anl.gov](mailto:///cgraziani@anl.gov)) 


[AI Accelerators for Science](https://github.com/argonne-lcf/ai-science-training-series/blob/main/08_advanced_architectures_methods/ALCF_AI_Testbed_Vishwanath.pdf)
    
[Gaussian Process Modeling](Gaussian_Process_Modeling.ipynb)

[Advanced AI Methods](https://github.com/argonne-lcf/ai-science-training-series/blob/main/08_advanced_architectures_methods/AITrainingSeries-AdvancedMethods.pdf)

**Useful Links**

 [Getting started on AI Testbed](https://www.alcf.anl.gov/support/ai-testbed-userdocs/index.html)
 
 [Useful AI Testbed Resources](https://github.com/argonne-lcf/AIaccelerators-SC22-tutorial)
 
 **Homework**
 
 Submit a paragraph about: 
 
- How could you use AI for a problem that interests you? 
- What is the task? 
- What kind of data would you use? 
- What kind of method or model might be appropriate? 
- What kind of metric would you use to measure success? 

Feel free to consult the Internet for ideas.

This paragraph can be placed in a README in git and you can submit the link. 

## Homework Solution

Breast cancer is one of the most widespread diseases among women, which is caused by the uncontrolled growth of cells in the breast (Bazazeh & Shubair, 2016). Using fine needle aspiration biopsy, experts can detect if the cells are malignant or benign (Frable, 1983). AI can play a vital role in diagnosing breast cancer. The task is to classify the given cells as malignant (M) or benign (B) using machine learning techniques on the fine needle aspiration dataset. We can train the machine learning model using the Breast Cancer Wisconsin (Diagnostic) Data Set from the UCI machine learning repository (Dua & Graff, 2019). The dataset includes the ID, diagnosis (M or B), and ten real-valued features from the cell nucleus. Before applying the ML-based technique to this data, we need to apply data cleaning and feature engineering steps for outliers detection and to understand the dataset on the feature level. For outlier detection, we may apply the DBSCAN clustering algorithm. To normalize the data for modeling, we can use the StandardScalar function. Finally, we can apply ML-based models and techniques such as SVC, logistic regression, KNeighbors, RandomForest etc. We calculate the model's F1 mean score and accuracy after splitting them into testing and training portions. Using grid search, we may also need to apply hyperparameter tuning on the top-performing model.

### References

- Bazazeh, D., & Shubair, R. (2016, December). Comparative study of machine learning algorithms for breast cancer detection and diagnosis. In 2016 5th international conference on electronic devices, systems and applications (ICEDSA) (pp. 1-4). IEEE.
- Frable, W. J. (1983). Fine-needle aspiration biopsy: a review. Human pathology, 14(1), 9-28.
- Dua, D. and Graff, C. (2019). UCI Machine Learning Repository [http://archive.ics.uci.edu/ml]. Irvine, CA: University of California, School of Information and Computer Science.

