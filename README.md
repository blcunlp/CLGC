# CLGC
This is a corpus for Chinese Literary Grace Evaluation. The corpus consists of 10,000 texts from novels and prose, with more than 1.85 million tokens, including 64\% level 1 texts (6,448 texts, 1,192,144 tokens), 19\% level 2 texts (1959 texts, 369,946 tokens) and 15\% level 3 texts (1593 texts, 294,748 tokens). Multi-level annotations are provided for each text in our corpus, including literary grace level, sentence category, and figure-of-speech type.
## Bib
@InProceedings{li-yu-liu:2022:LREC,

  author    = {Li, Yi  and  Yu, Dong  and  liu, pengyuan},
  
  title     = {CLGC: A Corpus for Chinese Literary Grace Evaluation},
  
  booktitle      = {Proceedings of the Language Resources and Evaluation Conference},
  
  month          = {June},
  
  year           = {2022},
  
  address        = {Marseille, France},
  
  publisher      = {European Language Resources Association},
  
  pages     = {5548--5556},
  
  abstract  = {In this paper, we construct a Chinese literary grace corpus, CLGC, with 10,000 texts and more than 1.85 million tokens. Multi-level annotations are provided for each text in our corpus, including literary grace level, sentence category, and figure-of-speech type. Based on the corpus, we dig deep into the correlation between fine-grained features (semantic information, part-of-speech and figure-of-speech, etc.) and literary grace level. We also propose a new Literary Grace Evaluation (LGE) task, which aims at making a comprehensive assessment of the literary grace level according to the text. In the end, we build some classification models with machine learning algorithms (such as SVM, TextCNN) to prove the effectiveness of our features and corpus for LGE. The results of our preliminary classification experiments have achieved 79.71\% on the weighted average F1-score.},
  
  url       = {https://aclanthology.org/2022.lrec-1.594/}
}
## Label Description
- C: declarative sentence. 
- Y: interrogative sentence.
- G: exclamatory sentence.
- Q: imperative sentence.
- BY: bi yu (比喻), including metaphor and simile, describes or illustrates A with B which is similar to A. 
- BN: bi ni (比拟), compares somebody to something, or something to somebody. 
- FF: fan fu (反复), repeatedly uses the same sentence to express strong feelings.
- PB: pai bi (排比), arranges words or sentences with the same or similar structure, closely related meaning, and consistent mood in series (usually contains three or more} sentences) to achieve an effect of strengthening the mood. 
- DO: dui ou (对偶), two phrases or sentences which are equal in the number of words, similar in syntax, related in meaning.
- TG: tong gan (通感), uses the qualifying adjective of A to express B. 
- YY: yin yong (引用), cites ready-made words in speech or writing, such as poems, maxims and idioms, to express their thoughts and feelings. 
## The Format (CLGC.csv)
- The first column is the filename, its format 'linguistic style'+'literary grace tag'+'number', such as 'swlevel01'. There are 6 tags to express the result of literary grace annotation: 1 (all the annotators chose 1); 0.8 (four annotators chose 1, one chose 0); 0.6 (three annotators chose 1, two chose 0); 0.4 (two annotators chose 1, two chose 0); 0.2 (one annotator chose 1, four chose 0); 0 (all annotators chose 0).
- The second column is the sentences of each file, a new sentence a new line. 
- The indexes after the second column are the sentence category tag, the cross-sentence figure of speech tag, figure-of-speech count, and figure-of-speech type tag (contained in '[]' and split by ','). 
- 'pp' means the end of a paragraph, and 'end' means the end of a segment.

| TXT Name  | Setence | Setence Category | P |Figure-of-speech Count | Figure-of-speech Type |
| :-------------: | :-------------: | :-------------: | :-------------: | :-------------: |:-------------: |
|sw1level116| 如一个娇媚的女子，面带微笑、静静地守在那里，等待着有缘人穿越万水千山寻梦在这里。  | C |0 |1 |['BY'] |
|sw1level116| pp |  pp | pp | pp | pp | pp |
|sw1level116|白墙青瓦、小船河道、弯弯的石拱桥，你在这头微笑，我在那头张望| C |0 |1 |['DO'] |
|sw1level116|我从不相信一见钟情，直到我看到那一幅幅美丽的图片，只那么一瞬间。| C |0 |1 |[''] |
|sw1level116|钟情，这个词，便深深的烙在心窝里。 | C |0 |1 |['BN'] |
|sw1level116|西塘，宛如生命中一场艳遇，在钟情的土壤中开始生根发芽。 | C |0 |1 |['BY''BN'] |
|sw1level116|pp |  pp | pp | pp | pp | pp |
|sw1level116|西塘，河流纵横，绿波荡漾，宁静的光阴在桨声四起的水波间开始了一天的美好时光。| C |0 |1 |['BN'] |
|sw1level116|end |end |end |end |end |end |

## The Basic Statistics
| Level  | Count | Character | Word | Sent |C|Y|Q|G|BY|BN|FF|PB|DO|TG|YY|P|
| :-------------: | :-------------: | :-------------: | :-------------: | :-------------: |:-------------: |:-------------: |:-------------: |:-------------: |:-------------: |:-------------: |:-------------: |:-------------: |:-------------: |:-------------: |:-------------: |:-------------: |
|1|6448|1192144|957369|45277|35074|7680|3768|424|1570|747|389|923|418|131|889|537|
|2|1959|369946|323947|13380|11011|1867|859|139|1219|688|205|632|516|108|518|436|4123|
|3|1595|294748|232672|10146|8865|1289|404|41|2014|2457|185|907|1143|306|552|538|7687|

## Others
The file named ``allcorpus'' save the raw corpus. The format of these corpus is shown as following:

![corpus](https://user-images.githubusercontent.com/31537780/149188967-fe4945ed-70d3-425e-9992-13f588fed0fe.png)
