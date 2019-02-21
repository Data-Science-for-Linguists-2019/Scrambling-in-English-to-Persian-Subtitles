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
- Getting my data to work. Phew -- I've got my files up and running! I found an XML parser that lets me read in the file. There are a few problematic characters in the English file (which I go through in my Python script). Looking up what people did online, it seems that these are buggy encoding errors, so I will try reading these files through different encodings to see if there's anything that works better; there are no trends between the buggy files. Should no other encoding work, I may have to correct and/or delete the errors so that I can work on the file. There aren't too many to fix, and I know what should be there based on the Persian translation, so I may do that.

##### Things that still need to be done:
- POS-tagging both the English and Persian sentences. After talking with Jevon and doing some of my own digging, it looks that I'm going to have to use a shallow parser rather than a dependency parser, as I don't know how to computationally construct a conll file for all of this data from POS-tagged sentences. POS-tagging and a shallow parser should be good enough for now in determining general outlines for scrambling.
- Narrowing my search. I want to examine how English similes may possibly inflect syntactic scrambling in their Persian translations. That being said, quite a few everyday speech patterns use "like" and/or "as", meaning that I'll have to limit the results in some other way rather than just searching for these two words. Perhaps I could also search for the Persian equivalents? I need more time to think (and to visit office hours, most likely). 
##### My data-sharing plan(s)

##### Relevant links: