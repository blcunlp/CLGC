# CLGC
This is a corpus for Chinese Literary Grace Evaluation. The corpus consists of 10,000 texts from novels and prose, with more than 1.85 million tokens, including 64\% level 1 texts (6,448 texts, 1,192,144 tokens), 19\% level 2 texts (1959 texts, 369,946 tokens) and 15\% level 3 texts (1593 texts, 294,748 tokens). Multi-level annotations are provided for each text in our corpus, including literary grace level, sentence category, and figure-of-speech type.
## The Format
- The first column is the filename, its format 'linguistic style'+'literary grace tag'+'number', such as 'swlevel01'. There are 6 tags to express the result of literary grace annotation: 1 (all the annotators chose 1); 0.8 (four annotators chose 1, one chose 0); 0.6 (three annotators chose 1, two chose 0); 0.4 (two annotators chose 1, two chose 0); 0.2 (one annotator chose 1, four chose 0); 0 (all annotators chose 0).
- The second column is the sentences of each file, a new sentence a new line. 
- The indexes after the second column are the sentence category tag, the cross-sentence figure of speech tag, figure-of-speech count, and figure-of-speech type tag (contained in '[]' and split by ','). 
- 'pp' means the end of a paragraph, and 'end' means the end of a segment.
