# Random forest in Classifying Specific Language Impairment (SLI) / Autistic Specturm Disorder (ASD) / Typically Developing (TD)

## Project Information
   * **Author**: Yuri Park, Computation and Design - Digital Media, 2025, Duke Kunshan University
   * **Instructor**: Prof. Luyao Zhang, Duke Kunshan University
   * **Disclaimer**: Submissions to the Final Project for [STATS201 Introduction to Machine Learning for Social Science, 2023 Autumn Term (Seven Week - Second)](https://ms.pubpub.org/) instructed by Prof. Luyao Zhang at Duke Kunshan University
   * **Acknowledgments**: I extend my heartfelt appreciation to Professor Zhang for her thoughtful and unwavering guidance during my introduction to machine learning in her class. Her patience was invaluable, particularly when I struggled to settle on a research topic. I am grateful for her consistent support, including the extra office hours she generously dedicated to helping me overcome challenges. I also want to express my sincere thanks to my classmates for creating a supportive environment. Their constructive insights and suggestions played a pivotal role in refining my research, ensuring it became a comprehensive exploration with in-depth explanations. Together, Professor Zhang and my classmates have significantly contributed to my learning experience, and I am truly appreciative of their contributions.
   * **Project Summary**:
     * **Background/Motivation**: Building upon the insights from [Lee's research](https://github.com/jamsawamsa/Autism_SLI_textAnalyzer_NLP_ML.git), this study is motivated by Lee's 2016 findings, which noted, "Comparing the confusion matrices of all classifiers, it is observed that the ASD class has the lowest precision and F-measure across all classes, even after feature extraction" (Lee, 2016, pg. 33). Addressing this concern, the investigation aims to explore the potential of the Random Forest algorithm. This interest is further fueled by Dewi and Imah's 2020 research, which identifies the Random Forest algorithm as the best in classifying ASD in children and adolescents based on specificity and sensitivity values (Dewi & Imah, 2020, pg. 152).
     * **Research Question**: In the context of 2023, the Random Forest algorithm is widely recognized for its effectiveness in various case studies (e.g., Dewi & Imah, 2020; Qureshi et al., 2023). However, Lee's study, which did not incorporate Random Forest and instead endorsed soft voting as the most effective technique, serves as a valuable benchmark for assessing and comparing the efficacy of these methodologies. This study aims to answer the **research question**: _Can Random Forest surpass the consistently high-performing SVM, which attained an accuracy score of 87% +/- 3% in Lee's study (Lee, 2016, pg. 32)? Furthermore, how can the addition of Random Forest contribute to a deeper understanding of language impairment, propelling research advancements in this field?_
   * **Application Scenario**: As the early years are pivotal for speech development, particularly for preschoolers (3-5 years), timely identification of speech and language disorders during this developmental phase significantly enhances communication abilities and facilitates smoother transitions to school, ensuring faster adaptation to the norm. Consequently, with the research focusing on children's speech data and determining the most efficient algorithm, its applications are diverse and effective, ranging from clinical settings to developing AI friend robots tailored to children with language impairments.
   * **Methodology**: Basing the research on [Lee's work](https://github.com/jamsawamsa/Autism_SLI_textAnalyzer_NLP_ML.git), the methodology involves integrating a random forest algorithm into the pre-existing list of algorithms employed by Lee. Using the [scikit-learn Python toolkit for machine learning and data mining](https://scikit-learn.org/stable/), my approach focuses on determining the optimal parameter settings for the random forest. The methodology seeks to discern and apply the most effective parameters for the random forest within the scope of this research, facilitating a comparative analysis of its efficacy against other algorithms.
   * **Results**: Two key outcomes facilitate the comparison process. Firstly, employing the confusion matrix from sklearn allows us to evaluate the accuracy of machine learning algorithms by juxtaposing their predictions against the actual answers. Secondly, leveraging the classification tool from sklearn provides a visual representation of the accuracy range for each machine learning algorithm, particularly in the identification of SLI, ASD, and TD. Additionally, as a supplementary component, the report will highlight the most significant features identified after the complete classification process.
     * Ultimately, the findings revealed that the random forest algorithm performed exceptionally well, ranking as the best algorithm after the SoftVotingEnsembleMethod. Consequently, it is safe to conclude that the random forest demonstrates accurate predictions, aligning with reports from 2023 and validating Lee's research method as consistent with current trends.
    
   * **Intellectual Merit/Practical impact**: Having recognized the random forest as the most effective individual algorithm in this field of study, there is an opportunity for additional investigation to uncover the underlying reasons for its optimal performance. However, a more significant revelation arises from the minor findings: the identification of the most crucial features for detection. This discovery holds the potential to provide novel insights, offering valuable input for advancing the field. Understanding these indicative features can play a pivotal role in enhancing early detection efforts and other applications within the domain.

## Table of Contents
  * **[Literature](Literature/README.md)**: Review of relevant existing literature.
  * **[Method](Method/Readme.md)**: Description of the methodology employed in the research.
  * **[Data](Data/README.md)**: Information about the data used in the study.
  * **[Code](Code/README.md)**: Details related to the code or computational methods used.
  * **[Results](Result/README.md)**: Presentation and analysis of the research findings.
  * **Spotlight**: A special section highlighting specific aspects of the research.
  * **More about the Author**: Information about the background and qualifications of the researcher.
  * **References**: Citations and sources used in the document.

## Spotlight
![](summaryPoster.png)

## More about the Author
I am an undergraduate student at Duke Kunshan University. Driven by a keen interest in education and a passion for effective communication, many of my projects aim to deliver informative and interactive messages. As I aspire to expand my capabilities in design, my curiosity and enthusiasm for machine learning led me to pursue this course.
![](ProfileImage.png)

My portfolio Website: yuripark.me

### Final reflections
  * **Intellectual growthh**:
    * **Through Class**: Gaining proficiency in machine learning has afforded me a more profound comprehension of its contemporary applications. In the realm of social science, employing machine learning and diverse packages to address societal issues has empowered me to explore and resolve these topics more thoroughly. Moreover, the classroom setting facilitated a better grasp of machine learning applications, as students could conduct research aligned with their individual interests. Consequently, the class structure and environment significantly facilitated my in-depth exploration of the practical applications of machine learning.
    * **Interdisciplinary Growth**: In taking this course and hearing everyone's research directions, I was able to observe how interdisciplinary collaboration truly unfolds in research. Specifically, as a computation and design major, most of my research stems from design thinking. However, adding a research topic concerning the global health and linguistic perspective of the impact and features of language impairment allowed me to further broaden my knowledge. Furthermore, witnessing the different approaches that students from various majors take in conducting this research was intriguing. For instance, computer science students may focus more on the coding and efficiency aspects, while I, with a design thinking perspective, consider the potential impact of such research in the context of design. It was interesting to see the diversity of approaches.

  * **Professional growth**: Gaining a general understanding of machine learning has significantly contributed to my professional growth, enabling me to engage in discussions with a diverse range of designers and artists. Particularly, in light of the prevailing trend where many designers utilize machine learning as a tool to enhance their work, I view my decision to advance my professional growth in this direction as a meaningful step forward.
  * **Living a purposeful life**: In the future, I aspire to be acknowledged as a designer characterized by a commitment to care. Given that many of my projects center around improving the learning process and addressing global issues, I aim to be recognized within the design community as a leading advocate for compassionate design. Thus, my feature sentence would potentially be "advocate for compassionate design within the design community". I would like my future contributions to the world to involve encouraging more designers to create things based on care and support for the world.


## References
### Data Source
  * **CHILDES**: https://childes.talkbank.org/
  * **Lee's Research**: https://github.com/jamsawamsa/Autism_SLI_textAnalyzer_NLP_ML.git

### Code Source
  * **Lee's Research**: https://github.com/jamsawamsa/Autism_SLI_textAnalyzer_NLP_ML.git

### Articles & Literature 
Borovsky, Arielle, Donna Thal, and Laurence B. Leonard. “Moving towards Accurate and Early Prediction of Language Delay with Network Science and Machine Learning Approaches.” Scientific Reports 11, no. 1 (April 14, 2021). https://doi.org/10.1038/s41598-021-85982-0.

Dewi, Erina S., and Elly M. Imah. “Comparison of Machine Learning Algorithms for Autism Spectrum Disorder Classification.” www.atlantis-press.com. Atlantis Press, November 24, 2020. https://doi.org/10.2991/aer.k.201124.028.

Félix, Juliana, Maria Emília Santos, and Antonio Benitez-Burraco. “Specific Language Impairment, Autism Spectrum Disorders and Social (Pragmatic) Communication Disorders: Is There Overlap in Language Deficits? A Review.” Review Journal of Autism and Developmental Disorders, August 4, 2022. https://doi.org/10.1007/s40489-022-00327-5.

Lee, Zhong Kein James. “Autism_SLI_textAnalyzer_NLP_ML/Use_of_NLP_and_ML_to_clinically_access_children.pdf at Master · Jamsawamsa/Autism_SLI_textAnalyzer_NLP_ML.” Autism_SLI_textAnalyzer_NLP_ML. GitHub, October 22, 2016. https://github.com/jamsawamsa/Autism_SLI_textAnalyzer_NLP_ML/blob/master/Use_of_NLP_and_ML_to_clinically_access_children.pdf.

NIDCD. “Developmental Language Disorder,” May 8, 2023. https://www.nidcd.nih.gov/health/developmental-language-disorder#Is-DLD-same.

```bibtex
@misc{a2023_developmental,
  month = {05},
  title = {Developmental Language Disorder},
  url = {https://www.nidcd.nih.gov/health/developmental-language-disorder#Is-DLD-same},
  year = {2023},
  organization = {NIDCD}
}

@article{flix_2022_specific,
  author = {Félix, Juliana and Santos, Maria Emília and Benitez-Burraco, Antonio},
  month = {08},
  title = {Specific Language Impairment, Autism Spectrum Disorders and Social (Pragmatic) Communication Disorders: Is There Overlap in Language Deficits? A Review},
  doi = {10.1007/s40489-022-00327-5},
  urldate = {2022-08-09},
  year = {2022},
  journal = {Review Journal of Autism and Developmental Disorders}
}

@article{borovsky_2021_moving,
  author = {Borovsky, Arielle and Thal, Donna and Leonard, Laurence B.},
  month = {04},
  title = {Moving towards accurate and early prediction of language delay with network science and machine learning approaches},
  doi = {10.1038/s41598-021-85982-0},
  urldate = {2022-10-25},
  volume = {11},
  year = {2021},
  journal = {Scientific Reports}
}

@misc{dewi_2020_comparison,
  author = {Dewi, Erina S. and Imah, Elly M.},
  month = {11},
  pages = {152–159},
  publisher = {Atlantis Press},
  title = {Comparison of Machine Learning Algorithms for Autism Spectrum Disorder Classification},
  doi = {10.2991/aer.k.201124.028},
  url = {https://www.atlantis-press.com/proceedings/ijcse-20/125946383},
  urldate = {2023-12-13},
  year = {2020},
  organization = {www.atlantis-press.com}
}

@misc{lee_2016_autism_sli_textanalyzer_nlp_mluse_of_nlp_and_ml_to_clinically_access_childrenpdf,
  author = {Lee, Zhong Kein James},
  month = {10},
  publisher = {GitHub},
  title = {Autism_SLI_textAnalyzer_NLP_ML/Use_of_NLP_and_ML_to_clinically_access_children.pdf at master · jamsawamsa/Autism_SLI_textAnalyzer_NLP_ML},
  url = {https://github.com/jamsawamsa/Autism_SLI_textAnalyzer_NLP_ML/blob/master/Use_of_NLP_and_ML_to_clinically_access_children.pdf},
  urldate = {2023-12-13},
  year = {2016},
  organization = {Autism_SLI_textAnalyzer_NLP_ML}
}
```
