## Setting up the Pre-processing Workplace
After following the Data Query steps, the following content below is some additional comments based on the step-by-step procedure shared on Lee's GitHub page:

- [x] Install the dependencies
* LanguageModel.py
* classifier_m.py (mainly used for the processing)
* features.py
* driver_m.py (mainly used for the pre-processing)
* subject_object_extraction.py

- [x] Working Environment Setup using PyCharm
* Adjust the discrepancy in the Python interpreter paths 
Have your Python Interpreter and your terminal located/using the same  interpreter. For example, you need to have both be using Anaconda or a virtual environment.
You can check this information by running

import sys
print(sys.executable) in .py and
which python in the terminal

doing so, you should import and update the package information on the same track. I highly suggest you have the Python Interpreter adjusted based on the virtual environment because the change you made to the PATH variable in your terminal session is not permanent—it only applies to the current terminal session. When you close this terminal window and open a new one, the PATH will revert to its previous state, and you will have to make the adjustment again.

Example: If your terminal responds /Users/yuri/opt/anaconda3/bin/python when you run which python, you need to manually change the Python Interpreter from (if you are a Mac user) PyCharm > Settings > Python Interpreter > Add and have Anaconda with the path you have given in the terminal response

[!](/Demo_Anaconda.png)

* Download all the necessary packages that were mentioned briefly in the Data Query steps
Check the warnings: Some packages need to be updated in terms of the version of the other following package that works hand in hand thus,
Example: if the downloaded default version of the spaCy is version 3.3.1 and your en_core_web_sm pipeline is version 3.7.1 you can either
1. conda update spacy then check with python -m spacy --version or
2. python -m spacy download en_core_web_sm==3.3.1 then check with python -m spacy validate

* Download additional necessary functions
In my case, I had to download some function features in nltk package to run the code.

nltk.download('wordnet')
nltk.download('punkt')
nltk.download('stopwords')
nltk.download('averaged_perceptron_tagger')
nltk.download('universal_tagset')
nltk.download('cmudict')

Please adjust your necessary downloads based on your warning/error messages

## Pre-processing Final: Getting the output_file data
When running the code, I suggest you have a print("") function in-between so that you know the loop is running to have the data processing for each line in XML. When the whole loop is done, you will be able to find a file made in the folder named output_file. (I have attached my output result also in this folder)
