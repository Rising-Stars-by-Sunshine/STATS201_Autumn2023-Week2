## CHILDES (Data's Origin)

Utilizing Natural Language Processing was crucial for accessing open text data. Following Lee's research approach, the CHILDES database (http://childes.talkbank.org/) was identified as a valuable resource. CHILDES offers labeled text transcripts for individuals with Autism Spectrum Disorder, Specific Language Impairment, or Typical Development. This data is instrumental in classifying children according to these categories.

## How to Access Data
Following the step-by-step procedure shared in Lee's GitHub page:

- [x] Download the two .7z files and extract them into your working directory:
* plain_text.7z
* xml.7z

The text transcript files inside the plain_text.7z are already classified in the folder of "asd", "sli", and "td." To allow the computer to find the for instance differentiation for who the investigator and children speaker is, tags are within the text file.
### Sample Tag Examples

| Tag   | Description                                                                                                                                 |
|-------|---------------------------------------------------------------------------------------------------------------------------------------------|
| `%err`| Indicates a correction for an error in the preceding utterance, for example, noting the correct form of a mispronounced word.             |
| `*INV`| Identifies the speaker as the 'investigator' or interviewer in the conversation.                                                            |
| `*CHI`| Identifies the speaker as the 'child', used in child language acquisition studies.                                                          |
| `%mor`| Provides a morphological breakdown of the preceding utterance, decomposing the sentence into its grammatical components like pronouns, verbs, nouns, etc. |
| `[ ]` | Square brackets are used for various annotations, such as marking unclear speech (`xxx`), self-corrections, or non-standard forms.           |
| `< >` | Angle brackets are often used alongside square brackets to indicate the beginning and end of self-corrections or revisions in speech.       |
| `%com`| Used for comments by the transcriber or researcher, providing context or additional information about the utterance or situation.          |


