John R. Starr; jrs294@pitt.edu; 01/29/19

# Scrambling in the Tehran English-Persian parallel corpus 

#### SUMMARY
Looking at parallel colloquial-speech corpora between English and 
Persian, I will investigate the effects that translation has on 
syntactic scrambling.

#### DATA
I'm looking to use the Tehran English-Persian parallel corpus (TEP). The 
corpus can be downloaded at the following URL: 
http://opus.nlpl.eu/TEP.php

This corpus consists of approximately 1.22 million sentence fragments 
of English subtitles and their Persian translations. According to an 
article written about the corpus (which is cited at the URL provided), 
the corpus is already "clean and pre-processed with special care for the 
Persian part"; that being said, I have not been able to examine the 
Persian file yet, as my computer has been acting up. The English file is 
an xml file that separates the sentences by the following string; " . "
The OPUS resources also have pre-compiled word alignments and other 
formatting niceties.

#### ANALYSIS
As someone interested in translational studies, I am intrigued to see 
how the subtitles handle syntactic scrambling. Persian is a language 
that allows for this linguistic process, especially when spoken 
colloquially. I intend on using tagged sentences to determine the word 
order of the sentence and then examining which syntactic patterns in 
English initiate scrambling in Persian. I anticipate that there will be 
significant scrambling caused by idiomatic expressions in English of 
which there are few equivalents in Persian. As noted in the comments of 
my original proposal of this idea, I will need to find a reliable parser 
for Persian. Thankfully, I have found a plethora of resources to help 
parse the words. They can be found at the following links:

Collection of various resources: 
https://github.com/mhbashari/awesome-persian-nlp-ir

Paper on ParsPer, which achieves approximately 82-87% accuracy:
https://www.diva-portal.org/smash/get/diva2:881563/FULLTEXT01.pdf

Paper on MaltParser and MST Parser (trained on Uppsala Persian 
Dependency Treebank): 
https://pdfs.semanticscholar.org/2759/a770ef731544e946cf47dbb198e0f6ef153e.pdf
It should be noted that I don't believe the latter two parsers here 
would be the ones to use, as their accuracies are too low (though it 
would be an interesting comparison, nonetheless)!
 

After testing this and determining if it is true or not, I would be interested in seeing if I 
could build a machine learning model that anticipates the word order 
for the Persian sentences based on the English model, though I am not 
entirely sure how to do that.
