Code repository for the paper: \
"Who Checks the Checkers? Exploring Source Credibility in Twitter’s Community Notes" by Uku Kangur, Roshni Chakraborty and Rajesh Sharma
===

📒 Notebooks

Folder notebook contains the main logic and results of the project. The cell outputs of the notebooks are also given to aid visualization (plots) and interpretation (data samples).

* To explore the analysis of type, bias and factuality in sources (RQ1), see notebooks/source_overview.ipynb

* To explore how factuality and bias scores were calculated and aggregated (RQ2), see notebooks/note_factuality_and_bias_calculation.ipynb

* To explore how notes were merged with ratings given by users (RQ2), see notebooks/ratings_merging_and_filtering.ipynb

* To explore the analysis of bias and factuality in notes (RQ2), see notebooks/note_analysis.ipynb

🗂️ Data

 We utilize two datasets for our study. The Community Notes dataset, which can be downloaded here [here](https://communitynotes.x.com/guide/en/under-the-hood/download-data) and the source bias dataset, which can be found in the repository.

The source bias dataset used is given as the file annotated_sources_final.xlsx. The dataset composes 44524 sources out of which the top 500 most dominant have been annotated with country, type, bias, factuality and reliability labels. The sources have been collected from Community Notes from the period January 23, 2021 to January 27, 2024. The dataset holds the following columns:

* url: the base domain of the source
* frequency: the frequency of occurance of the source domain and its subdomains in community notes
* merged_urls: the subdoimains of the source that occured in the community notes
* country: country of the domain in abbrevated format (i.e. JPN, USA, etc.)
* type: type of the source (i.e. News, Social Media, etc.)
* bias (MBFC): bias label given to source by Media Bias / Fact Check (MBFC)
* bias (AS): bias label given to source by All Sides (AS)
* bias (AF): bias label given to source by Ad Fontes (AF)
* bias (final): majority vote bias label of MBFC, AS and AF bias labels.
* factuality (MBFC): factuality label given to source by Media Bias / Fact Check (MBFC)
* reliability (AF): reliability label given to source by Ad Fontes (AF)
