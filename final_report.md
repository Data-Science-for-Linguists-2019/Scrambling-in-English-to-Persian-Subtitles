# Final Report
#### John R. Starr; jrs294@pitt.edu

### The Hypothesis
I believe that SVO sentences will display more complex metaphorical structures involving simile, as transfer of English similes to Persian often creates strange errors in syntactic structures.

### The Corpus
My corpus is the Tehran English-Persian Parallel Corpus, or TEP for short. This corpus is comprised of English and Persian subtitles that have been taken from an online movie corpus. More information about the TEP can be found [at this link](http://opus.nlpl.eu/TEP.php).

### The Process
##### Aligning Data
First, I had to align the two large .xml files. Unfortunately, the data had some encoding errors that had to be modified, which can be found [here](https://github.com/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/blob/master/data/data_modifications.txt). 
I lined the English and the Persian data using pandas and and numpy methods to manipulate the indices provided in the .xml files themselves. After this, I created columns for the length, tokens (and their number), and type (and their number) for both Persian and English. No conclusions were suggested yet.
##### POS-tagging & Chunking
For the Persian data, I used a POS-tagger and chunker under the free-to-download software [hazm](https://github.com/sobhe/hazm). For English, I used nltk's POS-tagger. Because I was unable to implement pre-installed chunkers for English due to the limitations of my computer, I had to use another computer to chunk the English sentences. I ended up capitalizing on nltk's regular expression parsers to get the English chunks in working conditions.

##### Generalizing Chunks
To generalize chunks into either SOV, SVO, or "Other" word orders, I utilized regular expressions, defining what counted as an NP/VP and what didn't in order to build a restrictive but also open generalizer. The top ten word counts are as follows: ![png](images/word_order_count_final.png).


A great deal of the data ended up being classified as "Other" ([see here](https://nbviewer.jupyter.org/github/Data-Science-for-Linguists-2019/Scrambling-in-English-to-Persian-Subtitles/blob/master/notebooks/4_generalizing_chunks.ipynb#Section-4:-Examining-Other-Data), which was followed by SOV and then SVO. This is not entirely surprising, since the data consists of many one-word sentences for the quick discourse necessary for subtitles; also, the default word order of Persian is SOV. The counts for the generalized word orders can be seen as follows:
![png](images/gen_word_order_final.png)

##### Analyzing the Data
Unfortuantely, analysis of my data did not provide much support for my hypothesis. Regardless, I will continue to pursue alternative methods after this semester has ended.

##### Issues, Failed Attempts, and Other Problematic Situations
I encountered many issues with my project. Firstly, I had encoding issues with my Persian .xml file. Secondly, regular expressions are not yet my friend. They gave me lots of problems, sometimes overmatching, othertimes undermatching. Thirdly, I am not satisfied by how my chunker operated, as it made many mistakes.





