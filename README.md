# Scrambling in Persian based on a Subtitle Corpus
Hello, viewer! My name is John R. Starr, and I am an undergraduate student at the University of Pittsburgh. I am double majoring in English Writing (Poetry) and Linguistics, the latter of which being the reason that this repo exists in the first place. This repo is the term project for my Data Science for Linguists course. Now, let's dive in, shall we?

### Description of Project
Persian is an SOV language that is prone to scrambling to SVO in a variety of contexts. This project examines SOV, SVO, and other, more complex word orders, hoping to find some possible explanations for scrambling. In particular, it analyzes how Persian similes and complex sentences are affected by scrambling. 

The corpus that this project derives its data from is the Tehran English-Persian Parallel Corpus, which is a compilation of over 550,000 subtitles in both English and Persian. The corpus consists of two large .xml files, one for each language, with easy-to-read indices that align the two files. This corpus is available for free download [here](http://opus.nlpl.eu/TEP.php) and can be used for any research and/or non-commercial purposes.

Comments on my project from my peers can be found [here](https://github.com/Data-Science-for-Linguists-2019/Class-Plaza/blob/master/guestbooks/guestbook_john.md).

### Repo Directory:
- Notebooks:
    - [1. Data Summary](https://github.com/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/blob/master/notebooks/1_data_summary.ipynb) focuses on the structure of the data itself. [NB Version](https://nbviewer.jupyter.org/github/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/blob/master/notebooks/1_data_summary.ipynb)
    - [2. Tagging, Chunking](https://github.com/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/blob/master/notebooks/2_tagging_chunking.ipynb) POS-tags the Persian and English data and chunks the Persian data. [NB Version](https://nbviewer.jupyter.org/github/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/blob/master/notebooks/2_tagging_chunking.ipynb)
    - [3. Chunking English](https://github.com/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/blob/master/notebooks/3_chunking_english.ipynb), as the name suggests, chunks the English data. This is a separate file due to some limitations of running Anaconda on Windows. [NB Version](https://nbviewer.jupyter.org/github/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/blob/master/notebooks/3_chunking_english.ipynb)
    - [4. Generalizing Chunks](https://github.com/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/blob/master/notebooks/4_generalizing_chunks.ipynb) is where word orders are derived from the chunks. [NB Version](https://nbviewer.jupyter.org/github/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/blob/master/notebooks/4_generalizing_chunks.ipynb)
    - [5. Data Analysis](https://github.com/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/blob/master/notebooks/5_data_analysis.ipynb) navigates the data for three different structures, looking to make sense of why the word orders may be the way they are. [NB Version](https://nbviewer.jupyter.org/github/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/blob/master/notebooks/5_data_analysis.ipynb)
- Project Information:
    - [Project Plan](https://github.com/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/blob/master/project_plan.md) outlines the preliminary ideas for this project.
    - [Progress Report](https://github.com/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/blob/master/progress_report.md) shows the process of building this repo throughout the semester.
    - [Information on Persian](https://github.com/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/blob/master/pers_info) provides some basic information about Persian.
    - [Final Report](https://github.com/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/blob/master/final_report.md) sums up the project as a whole.
- [Images](https://github.com/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/tree/master/images) is where you will find image files found in my notebooks.
- [Data](https://github.com/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/tree/master/data) contains an example DataFrame constructed from the files, along with a text documents of all the changes that I made to the orignal file.

References: 
M. T. Pilevar, H. Faili, and A. H. Pilevar, “TEP: Tehran English-Persian Parallel Corpus”, in proceedings of 12th International Conference on Intelligent Text Processing and Computational Linguistics (CICLing-2011)