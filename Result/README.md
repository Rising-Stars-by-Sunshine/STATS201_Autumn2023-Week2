# Main Result Output
The result are divided in the catagory of pre-processed and processed. In such way, understading of the before and after the application of each algorithm can be obsereved.

## Pre-processed Result
<p float="left">
  <img src="/Result/Pre_DecisionTree_Result.png" width="240" />
  <img src="/Result/Pre_EnsembleM_Result.png" width="240" />
  <img src="/Result/Pre_GaussianN_Result.png" width="240" />
</p>

<p float="left">
  <img src="/Result/Pre_K-Nearest_Result.png" width="240" />
  <img src="/Result/Pre_NeuralN_Result.png" width="240" />
  <img src="/Result/Pre_RandomF_Result.png" width="240" />
  <img src="/Result/Pre_SVM_Result.png" width="240" />
</p>

## Processed Result
<p float="left">
  <img src="/Result/DecisionTree_Result.png" width="240" />
  <img src="/Result/EnsembleM_Result.png" width="240" />
  <img src="/Result/GaussianN_Result.png" width="240" />
</p>
<p float="left">
  <img src="/Result/K-Nearest_Result.png" width="240" />
  <img src="/Result/NeuralN_Result.png" width="240" />
  <img src="/Result/RandomF_Result.png" width="240" />
  <img src="/Result/SVM_Result.png" width="240" />
</p>

## Processed Result Comparision
By tabulating both the count of accurate predictions and the individual performance of each machine learning algorithm, I've generated a chart that organizes the results from most accurate to least accurate. Comparing these findings to Lee's, it's intriguing that, like Lee's results, the soft voting ensemble method is the best predictor—logical given its ability to choose the best-performing algorithms. However, the notable discovery is that Random Forest emerges as the second-best, suggesting it excels as a standalone algorithm for prediction.
|            | SLI | ASD | TD |
|------------|-----|-----|----|
| Ensembled  | 26  | 8   | 36 |
| Random Forest | 26 | 6 | 35 |
| KNN | 25 | 5 | 36 |
| Neural Network | 24 | 6 | 34 |
| Decision Tree | 24 | 7 | 31 |
| Gaussian | 25 | 8 | 26 |
| SVM | 22 | 6 | 30 |

## Overall Classification Result
![](/Result/Classification_Result.png)
As depicted in the graph above, the effectiveness of each algorithm in detection can be gauged by the extent to which the color encapsulates the actual points plotted on the linear graph. Notably, the results for Random Forest reveal a broader coverage of specific ranges compared to other algorithms. This observation highlights the heightened specificity achieved by the Random Forest algorithm in the detection process.

# Minor Result Output
![](/Result/Feature_Result.png)

# Result Analysis
With my research question being
> Can Random Forest surpass the consistently high-performing SVM, which attained an accuracy score of 87% +/- 3% in Lee's study (Lee, 2016, pg. 32)? Furthermore, how can the addition of Random Forest contribute to a deeper understanding of language impairment, propelling research advancements in this field?

