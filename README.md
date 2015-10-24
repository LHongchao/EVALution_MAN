# EVALution_MAN
1.Introduction
This is a dataset for the training and evaluating Distributional Semantic Models (DSMs) on on semantic relations discrimination between words in Chinese. The dataset contains 360 positive relation pairs, distributed in four different semantic relations, including antonymy, synonymy, hypernymy, and nearsynonymy. About 300 pairs were checked manually to estimate their quality and add semantic type information. To the best of our knowledge, EVALution-CH is the first of its kind for Chinese.

The dataset will be enlarged cotinously and each new version will be uploaded to a new branch.

This is the version 1.0 of EVALution_MAN. It includes two groups of files: one is the relation group which contains the information of relation pairs; the other is the relata group which contains the information of relata. Each group contains two files according to the mannual rating and tagging task naming positive_relation.txt, negative_relation.txt and positive relata.txt, negative_relata.txt.

For relation group, Only pairs that had at least three positive ratings (“totally agree”, and “agree”) can be included into the positive_relation.txt.The rest ones will be included into negative results. Finally, we got 360 positive pairs and 132 negative_relation.txt.

For the relata group, only the tags with two or more votes will be treated as positive results and we got 373 relata in positive_relata.txt and 3 in negative_relata.txt.

The format of relation group's files is the same while it is also the case for the relata group.


2.Format

2.1 relation group

These two datasets (positive_relation.txt and negative_relation.txt) contains the relation pairs with annoatation information of whether the relation is reliable or not.

NO.1 to NO.6 are information of the relata and the relatum
  
(1) relata_lemma: this refers to the relata word. "Lemma" is copied from Chinese WordNet but actually Chinese has no inflection and thus we cannot say that the word is a lemma. 

(2) relata_pos: this refers to the POS of the relata. POS tag and their meanings can be found in the following link:

http://app.sinica.edu.tw/kiwi/mkiwi/98-04.pdf


(3) relation_type: the dataset contains four different relationships: synonymy, nearsynonymy, antonymy, hyponymy, meronymy

(4) relatum_lemma: this refers to the word which is related to the relata.

(5) relatum_pos: this refers to the POS of the relatum. POS tag and their meanings can be found in the following link:

http://app.sinica.edu.tw/kiwi/mkiwi/98-04.pdf

(6) template: This transfer the relata,relation type and relatum into a sentence in the following format:

  正式 和 非正式 意思相反
  
  "Formal and informal have the opposite meaning."


NO.7 to NO.11 are information of the relation annotation.We asked 10 linguistics Ph.D. students to do the manual annotation.
We divided ten people into two groups and gave half of the pairs to each group. The subjects were given sentences with pairs in them such as:

  龍 和 鳳 相關。
  
  “Dragon and phoenix are related to each other.”
  
They were required to rate each statement according to ‘totally agree’, ‘agree’, ‘don’t know’, ‘don’t agree’ and ‘totally disagree’. We also added ‘don’t know X’ and ‘don’t know Y’ tags in case an annotator was not familiar with a given word. Only the pairs with three or more agree (including agree or totally agree) votes will be treated as positive results.
  
(7) totally agree;(8) agree;(9) not sure;(10) don't know X;(11) don't know Y



2.2 relata.txt

This dataset contains the relata's frequency in a combined corpus of SINCIA and GigaaWord and the semantic filed of the relata and their relatum both with POS extracted from relation.txt excluding the repeated ones.

(1) relata: this refers to the word extracted from relation.txt including the relata and relatum without repeating.

(2) tt_freq: this is a integer which refers to the total frequency of the word (withouf POS) in the combined corpus.

(3) dominant_pos: this refers to the word's pos with the highest frequency with a format of Na_11. Na is the POS tag while 11 is the frequency.

(4) pos_distr: this refers to the word's pos distribution with a format of Nc_15496/A_1384/Na_12192/VA_1.

NO.5 to NO.21 are information of relata's semantic field tagging by Ph.D. students major in linguistics to do the tagging and they are required to select tags from the following ones:

First group: choose one or more

(5)Basic, (6)Subordinate and (7)Superordinate;

Second group: choose one

(8)General and (9)Specific;

Third group: choose one

(10)Abstract and (11)Concrete;

Fourth group: choose one or more

(12)Event, (13)Time, (14)Space, (15)Object, (16)Animal, (17)Plant, (18)Food, (19)Color, (20)People and (21)Attribute.

Only the tags with two or more votes will be treated as positive results.











