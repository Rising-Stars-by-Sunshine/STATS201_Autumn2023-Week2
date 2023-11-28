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
\usepackage{amsmath}
\usepackage{algorithm}
\usepackage[noend]{algpseudocode}

\makeatletter
\def\BState{\State\hskip-\ALG@thistlm}
\makeatother

\begin{document}
\begin{algorithm}
\caption{My algorithm}\label{euclid}
\begin{algorithmic}[1]
\Procedure{MyProcedure}{}
\State $\textit{stringlen} \gets \text{length of }\textit{string}$
\State $i \gets \textit{patlen}$
\BState \emph{top}:
\If {$i > \textit{stringlen}$} \Return false
\EndIf
\State $j \gets \textit{patlen}$
\BState \emph{loop}:
\If {$\textit{string}(i) = \textit{path}(j)$}
\State $j \gets j-1$.
\State $i \gets i-1$.
\State \textbf{goto} \emph{loop}.
\State \textbf{close};
\EndIf
\State $i \gets i+\max(\textit{delta}_1(\textit{string}(i)),\textit{delta}_2(j))$.
\State \textbf{goto} \emph{top}.
\EndProcedure
\end{algorithmic}
\end{algorithm}
\end{document} 
