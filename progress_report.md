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
