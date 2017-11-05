# Submission 550
## Mind the (Language) Gap: Neural Generation of Multilingual Wikipedia Summaries from Wikidata for ArticlePlaceholders
This repository contains code for the Submission 550 at The Web Conference.

The baselines are contained in **baselines**, there respective results as well as the results from our model are in
**results**.


The code contained in **crowdevaluation** was made in order to prepare and evaluate the community evaluation. The languages are abbreviated with their respective language codes (ar for Arabic and eo for Esperanto).
- **Preparation** contains files that were used to create the surveys.
  - **Arabic** and **Esperanto** respectively contain:
    - **\<languagecode\>-final-file**: sample of generated summaries evaluated 
    - **\<languagecode\>-news-sentences.csv**: sentences of the news corpus
    - **\<languagecode\>-wikipedia-sentences.csv**:sentences from the original Wikipedia 
  - The **code** folder contains scripts to prepare the corpus according to the requirements of the survey. It contains a README how to use those scripts.
- **Results** contains the result files of the survey, after annonymization and cleaning 
- **evaluation-results** contains scripts that were used to process the results
  - **Arabic** and **Esperanto** respectively contain:
    - **Fluency** for processing the results of the Fluency and Appropriateness survey
      - \<languagecode\>-quality.py calculates scores for the quality in terms of fluency
      - \<languagecode\>-approp.py calculates scores for the quality in terms of fluency
    - **Editors** for processing the results of the Editors 
