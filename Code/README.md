# Significance of Getting Pre-processed Data
The data file created during the preprocessing stage is pivotal for the successful execution of classifier_m.py 
in distinguishing between ASD (Autism Spectrum Disorder), SLI (Specific Language Impairment), and TD (Typically 
Developing) categories. This file, essentially a feature matrix, encapsulates a range of linguistic attributes 
meticulously extracted from speech samples. These features include, but are not limited to, word usage frequencies, 
syntactic variations, and morphological patterns.  Each line of data about the children ends with a tag of 0, 1, or 2, 
which tells if he or she is ASD, SLI, or TD. Thus, in all, the output_file act as data for conducting supervised learning.

As the foundation for training algorithms, feeding this structured data into classifier_m.py allows the script to apply
classification models to discern subtle yet significant patterns that differentiate ASD, SLI, and TD speech 
characteristics. The comprehensiveness and accuracy of these features are critical, as they directly influence 
the model's ability to learn and make precise predictions or classifications.

Ultimately, this preprocessed data doesn’t just feed into an algorithm; it shapes the algorithm’s understanding and 
recognition capabilities, forming the backbone of the machine learning process. The end goal is to enable the 
classifier to make informed and reliable predictions about new, unseen data, categorizing them into ASD, SLI, or TD, 
based on the learned patterns.

## Simple [Data Query and Pre-Processing](Code/Data-Query) Steps

| Step                        | Action                                                                                                   |
|-----------------------------|----------------------------------------------------------------------------------------------------------|
| Install Dependencies        | Install scripts: `LanguageModel.py`, `classifier_m.py`, `features.py`, `driver_m.py`, `subject_object_extraction.py` |
| Environment Setup           | Align Python interpreter in PyCharm with the terminal's interpreter. Use Anaconda or a virtual environment. |
| Check Python Path           | Run `import sys; print(sys.executable)` in Python and `which python` in the terminal to verify paths.     |
| Update Python Interpreter   | In PyCharm (macOS), update the interpreter in Settings to match the terminal's Python path.               |
| Download Packages           | Download necessary packages and update as needed. Pay attention to version compatibility.                 |
| Additional nltk Functions   | Download additional nltk functions as required (e.g., `nltk.download('wordnet')`).                        |
| Run Pre-processing          | Execute `driver_m.py` with print statements for tracking. Generates `output_file` with processed data.    |

Please adjust your necessary downloads based on your warning/error messages.

## Simple Outline: How Data Query Works
![](/DataQuery.png)


\documentclass{article}
\usepackage{amsfonts}
\usepackage{booktabs}
\usepackage{siunitx}

\begin{document}

\begin{tabular}{SSSSSSSS} \toprule
    {$m$} & {$\Re\{\underline{\mathfrak{X}}(m)\}$} & {$-\Im\{\underline{\mathfrak{X}}(m)\}$} & {$\mathfrak{X}(m)$} & {$\frac{\mathfrak{X}(m)}{23}$} & {$A_m$} & {$\varphi(m)\ /\ ^{\circ}$} & {$\varphi_m\ /\ ^{\circ}$} \\ \midrule
    1  & 16.128 & +8.872 & 16.128 & 1.402 & 1.373 & -146.6 & -137.6 \\
    2  & 3.442  & -2.509 & 3.442  & 0.299 & 0.343 & 133.2  & 152.4  \\
    3  & 1.826  & -0.363 & 1.826  & 0.159 & 0.119 & 168.5  & -161.1 \\
    4  & 0.993  & -0.429 & 0.993  & 0.086 & 0.08  & 25.6   & 90     \\ \midrule
    5  & 1.29   & +0.099 & 1.29   & 0.112 & 0.097 & -175.6 & -114.7 \\
    6  & 0.483  & -0.183 & 0.483  & 0.042 & 0.063 & 22.3   & 122.5  \\
    7  & 0.766  & -0.475 & 0.766  & 0.067 & 0.039 & 141.6  & -122   \\
    8  & 0.624  & +0.365 & 0.624  & 0.054 & 0.04  & -35.7  & 90     \\ \midrule
    9  & 0.641  & -0.466 & 0.641  & 0.056 & 0.045 & 133.3  & -106.3 \\
    10 & 0.45   & +0.421 & 0.45   & 0.039 & 0.034 & -69.4  & 110.9  \\
    11 & 0.598  & -0.597 & 0.598  & 0.052 & 0.025 & 92.3   & -109.3 \\ \bottomrule
\end{tabular}

\end{document}
