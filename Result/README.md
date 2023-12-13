# Result Analysis
With my research question being
> Can Random Forest surpass the consistently high-performing SVM, which attained an accuracy score of 87% +/- 3% in Lee's study (Lee, 2016, pg. 32)? Furthermore, how can the addition of Random Forest contribute to a deeper understanding of language impairment, propelling research advancements in this field?
the results below help answer the two questions asked

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
Illustrated in the above graph, the efficiency of each algorithm in detection is assessed based on the degree to which the color encompasses the actual points plotted on the linear graph. Noteworthy, the outcomes for Random Forest demonstrate a wider coverage of specific ranges compared to other algorithms. This observation underscores the heightened specificity attained by the Random Forest algorithm in the detection process.

> Hence, regarding the first hypothesis, it is safe to conclude that our initial assumption has been affirmed. The evidence supports the assertion that Random Forest is indeed the most effective algorithm for conducting the overall classification process when compared to other algorithms.

# Minor Result Output
![](/Result/Feature_Result.png)
The image on the left displays the rankings of the most important features before the implementation of the random forest. On the right, the image illustrates the rankings after the addition of the random forest. Notably, the top important feature remains consistent; however, the features following the first one differ entirely. These findings affirm a positive response to the second question, indicating a change in the importance of features. However, a comprehensive explanation is intentionally omitted, as it is intended for further research.

>  In the conclusion of the second hypothesis, it becomes evident that the addition of Random Forest has yielded unexpected findings. These go beyond merely confirming its efficacy and extend to revealing valuable insights—specifically, identifying more accurate features that significantly impact the prediction process.

