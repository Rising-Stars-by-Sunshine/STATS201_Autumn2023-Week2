# Impact of Adding Random Forrest
Incorporating a Random Forest classifier into this research adds a robust and versatile model known for its high accuracy and ability to handle large datasets with multiple features. Random Forest, an ensemble method comprising numerous decision trees, reduces overfitting and increases predictive accuracy. It achieves this by averaging the results of individual trees, which individually may be prone to overfitting. Its inclusion would enhance the research by providing a more comprehensive analysis, especially in complex classification tasks like distinguishing between SLI, ASD, and TD speech patterns.

Current research indicates that Random Forest is highly accurate (Dewi & Imah, 2020; Qureshi et al., 2023). By integrating Random Forest into this study, we can not only identify potential gaps but also contribute significantly to the field. If Random Forest proves effective in Lee's research, it will validate the robustness of the methodology and bolster confidence in the conclusions drawn. Conversely, if it underperforms, it will prompt further investigation into why this is the case, potentially uncovering unique features or aspects of Lee's research approach that differ from or even challenge conventional findings.

# How is Random Forrest Working in classifier_m.py
With the imported function RandomForestClassifier from the “sklearn.ensemble” library, the random forest classifier is functioning to have the machine learning process working. Especially, with the parameters of n_estimators=100 and random_state=0, the parameters for this classifier define how the ensemble of trees should be constructed and how they should behave. Specifically,  n_estimators=100 defines the number of trees and with random_state = 0, we ensure that the random numbers are generated in the same order each time you run the code, which ensures that the output of your algorithm is the same each time it's run with that seed.

In a VotingClassifier with voting='soft' in scikit-learn, weights assign different levels of importance to each classifier in the ensemble. When predictions are made, the predicted probabilities of each classifier (for each class) are multiplied by the classifier's weight and then averaged. The final class prediction is based on these weighted averages. Thus, with my intention to learn the efficiency of random forest efficiency, I have put the newly added random forest classifier ('rf') has a weight of 2, which is the same as the MLP and GNB classifiers as higher weights give more influence to the respective classifier's predictions. Thus, by adjusting these weights, I could fine-tune how much each classifier contributes to the final decision.

# Pre-Processed Result
Below are the results without the teaching process. This result will be compared with the processed result which uses the output_file to train. In doing so, a comparison among the processed results will be present.

## Pre-processed Result
<p float="left">
  <img src="/Code/Data-Analysis/Pre-Processed_Output/Pre_DecisionTree.png" width="240" />
  <img src="/Code/Data-Analysis/Pre-Processed_Output/Pre_EnsembleM.png" width="240" />
  <img src="/Code/Data-Analysis/Pre-Processed_Output/Pre_GaussianN.png" width="240" />
</p>
<p float="left">
  <img src="/Code/Data-Analysis/Pre-Processed_Output/Pre_K-Nearest.png" width="240" />
  <img src="/Code/Data-Analysis/Pre-Processed_Output/Pre_NeuralN.png" width="240" />
  <img src="/Code/Data-Analysis/Pre-Processed_Output/Pre_RandomF.png" width="240" />
  <img src="/Code/Data-Analysis/Pre-Processed_Output/Pre_SVM.png" width="240" />
</p>

## Processed Result
<p float="left">
  <img src="/Code/Data-Analysis/Pre-Processed_Output/DecisionTree.png" width="240" />
  <img src="/Code/Data-Analysis/Pre-Processed_Output/EnsembleM.png" width="240" />
  <img src="/Code/Data-Analysis/Pre-Processed_Output/GaussianN.png" width="240" />
</p>
<p float="left">
  <img src="/Code/Data-Analysis/Pre-Processed_Output/K-Nearest.png" width="240" />
  <img src="/Code/Data-Analysis/Pre-Processed_Output/NeuralN.png" width="240" />
  <img src="/Code/Data-Analysis/Pre-Processed_Output/RandomF.png" width="240" />
  <img src="/Code/Data-Analysis/Pre-Processed_Output/SVM.png" width="240" />
</p>


