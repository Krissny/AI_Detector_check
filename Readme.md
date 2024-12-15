AI Detector Check
=================

Project Overview
----------------

This project analyzes the accuracy of AI text detector tools by testing them on **900+ data points**. The data consists of PubMed article abstracts collected using **Biopython**. The analysis is based on the following key assumption:

-   **Abstracts published before 2015** are unlikely to contain AI-generated text.
-   **Abstracts published after 2022** may contain AI-generated text.

This comparative analysis allows us to evaluate how effectively current AI text detectors identify AI-generated content in academic writing.

Data Collection
---------------

-   **Source**: PubMed abstracts were collected using **Biopython**, specifically from articles published:
    -   **Before 2015**: Assumed to have no AI text.
    -   **After 2022**: Likely to have AI-generated text.
-   **Data Size**: 900+ abstracts for both before 2015 and after 2022.

* * * * *

Analysis
--------

-   The analysis compares results from multiple **AI text detection tools** such as GPT-2 and Sapling.
-   Accuracy is measured by checking whether the tools identify AI-generated text correctly for the two time periods: pre-2015 and post-2022.

* * * * *

Notebooks and Scripts
---------------------

1.  **Abstract Scripts**:

    -   `abstract_collection.ipynb`: Collects abstracts from PubMed.
    -   `abstract_cleaning.ipynb`: Cleans and processes the abstract data.
2.  **AI Tools Results**:

    -   `GPT_2.ipynb`, `sapling.ipynb`, `writer.ipynb`: Analyze the performance of different AI text detector tools.
3.  **Excel Files**:

    -   Results and raw data are stored in structured Excel files.

* * * * *

Requirements
------------

To reproduce this analysis, install the following dependencies:

`pip install biopython pandas openpyxl`

* * * * *

Usage
-----

1.  **Run Abstract Scripts**: Collect and clean PubMed abstracts using scripts in `Abstract_scripts/`.
2.  **Analyze AI Detection Tools**: Use notebooks in `AI_tools_result/` to test various AI detectors on the collected data.
3.  **View Results**: Processed results are available in `Excel_files/`.

* * * * *

Results
-------

The project aims to evaluate the following:

-   Are AI text detection tools reliable in identifying AI content?
-   How do these tools perform for pre-2015 versus post-2022 abstracts?

* * * * *
