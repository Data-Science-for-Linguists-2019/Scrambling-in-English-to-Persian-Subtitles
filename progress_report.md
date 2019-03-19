John R. Starr; jrs294@pitt.edu

# Progress Reports

### 0: The General Plan
This repository and all the files within have been gathered and created 
for my final project for the Spring 2019 semester of LING 1340/2340. 
Files will continue to be added as time goes on, and there will be three 
major progress reports. 

By the first official progress report, I hope to have a Persian parser 
(or some combination of Persian parsers) that allows me to reliably 
search the TEP. Fingers crossed!

### 1: First Progress Report (02/21/19)
##### Things that I accomplished:
- Getting my data to work (for the most part). Phew -- I've got my files up and running! I found an XML parser that lets me read in the file. There are a few problematic characters in the English file (which I go through in my Python script). Looking up what people did online, it seems that these are buggy encoding errors, so I will try reading these files through different encodings to see if there's anything that works better; there are no trends between the buggy files. Should no other encoding work, I may have to correct and/or delete the errors so that I can work on the file. There aren't too many to fix, and I know what should be there based on the Persian translation, so I may do that. Surprisingly enough, there were no problems reading the Persian file. 
##### Things that still need to be done:
- POS-tagging both the English and Persian sentences. After talking with Jevon and doing some of my own digging, it looks that I'm going to have to use a shallow parser rather than a dependency parser, as I don't know how to computationally construct a conll file for all of this data from POS-tagged sentences. POS-tagging and a shallow parser should be good enough for now in determining general outlines for scrambling.
- Narrowing my search. I want to examine how English similes may possibly inflect syntactic scrambling in their Persian translations. That being said, quite a few everyday speech patterns use "like" and/or "as", meaning that I'll have to limit the results in some other way rather than just searching for these two words. Perhaps I could also search for the Persian equivalents? I need more time to think (and to visit office hours, most likely). 
##### My data-sharing plan(s):
   As "usage of this package for any research or non-commercial purposes requires the precondition that you cite the following paper(s)", I have included the necessary references in the "Relevant Links" section below. However, because the TEP is available for free download, there is no need to include a significant portion of the corpus; also, the license does not provide much informationa about publication of data. I take this to mean that what I release must be within the domain of fair use. To maintain the integrity, I will provide a minimal number of relevant sentences, probably under 50, to demonstrate how my files work. I will run the my scripts on the complete corpus and use that as my results, but not publish the corpus itself. 
   The POS-tagger and shallow parser I am using, Parsivar, can be freely used and published as long as one has all the required documentation, as provided by the Github link below.
##### Relevant links:
- Tehran English-Persian Parallel Corpus download link: http://opus.nlpl.eu/TEP.php
    - M. T. Pilevar, H. Faili, and A. H. Pilevar, _TEP: Tehran English-Persian Parallel Corpus_, in proceedings of 12th International Conference on Intelligent Text Processing and Computational Linguistics_ (CICLing-2011)
    J. Tiedemann, 2012, _Parallel Data, Tools and Interfaces in OPUS_, in Proceedings of the 8th International Conference on Language Resources and Evaluation (LREC 2012)
- Parsivar: https://github.com/ICTRC/Parsivar
- My Python script: https://github.com/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/blob/master/project_script.ipynb


### 2: Second Progress Report (03/18/19)
##### Things that I accomplished:
- Finished Data Summmary. I added some more information and exported a pkl file. It seems that my file is 612086 lines long! Luckily, no null pieces.
- POS-tagging both English and Persian, chunking for Persian. I found a really nice POS-tagger and chunker for Persian named Perpos (see Relevant links section below). For English, I am trying out NLTK's POS-tagger and chunkers, though I'm on the hunt for better taggers and chunkers. 
- Becoming extremely frustrated with Windows and wishing that I had Linux instead. 
##### Things that still need to be done:
- Chunking English sentences. I wasn't able to get the chunkers to work.
- Simplifying the chunks. I want to modify the chunks for both the English and the Persian sentences so that they are mutually compatible, allowing me to work on analysis!
- Analysis!!! So much to be done.. I'm really not happy with how far I got for this progress report, and I will be making at least a few appointments for OH's so that I can get to where I want/need to be. 
##### Sharing scheme for data:
   Maintaining a similar position as to what I stated in the first progress report, I will only be releasing a small portion of my found data. The license for the TEP corpus does not outline much about the publication of its data, but it does indicate that the corpus is free to use and any work incorporating its files must cite a few specific papers (see Relevant Links section above). 
   I will be including derived data and some data that I included myself in the form of a sample_df.pkl file. It consists of only 50 sentences of POS-tagged (English, Persian) and chunked (Persian) subtitles. Considering the length of the full dataset is over 600,000 lines long, I believe I am operating within fair use. Should someone be interested in seeing all of the data, they can modify my code and run the files themselves. 
##### Licensing information:
   I chose the MIT license for a few reasons. Firstly, my project is intended to be easily adaptable for others to navigate and use, and therefore needs a license that is compatible witht this idealogy. The MIT license allows any person to use my data freely, as long as they provide the proper license and copyright from this file. This project is very much a "starting point" that can be more extrapolated upon by more advanced programmers. Secondly, it appears that the MIT license is a very popular license to use on Github, as the platform itself tends towards quick and easy access of shared code and data. Thirdly, this license is compatible with the licenses of the software and data that I am using; Perpos uses the MIT license as well, and the TEP only requires one to cite a paper or two. 
##### Relevant links:
- See above for links that are still relevant:
Resources and Evaluation (LREC 2012)
- [Perpos](https://github.com/mhbashari/perpos)
- My scripts:
    - [Data Summary](https://github.com/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/blob/master/data_summary.ipynb)
    - [Tagging and Chunking](https://github.com/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/blob/master/tagging_chunking.ipynb)
    - [Data Analysis (Unfinished)](https://github.com/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/blob/master/data_analysis_new.ipynb)