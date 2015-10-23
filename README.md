# EVALution_CH
Introduction
  This is a dataset for the training and evaluating Distributional Semantic Models (DSMs) on on semantic relations discrimination between words in Chinese. The dataset contains 5,400 relation pairs, distributed in four different semantic relations, including antonymy, synonymy, hypernymy, and nearsynonymy. About 300 pairs were checked manually to estimate their quality and add semantic type information. To the best of our knowledge, EVALution-CH is the first of its kind for Chinese.

  The dataset will be enlarged cotinously and each new version will be uploaded to a new branch.

  This is the version 1.0 of EVALution_CH. It includes two files: relation.txt and relata.txt;relation.txt contains 227 pairs while relata.txt contains 376 words.

Format
relation.txt
  NO.1 to NO.6 are information of the relata and the relatum
1) relata_lemma:
2) relata_pos:
3) relation_type:
4) relatum_lemma:
5) relatum_pos:
6) template:
  NO.8 to NO.11 are information of the relation annotation.We asked 10 linguistics Ph.D. students to do the manual annotation.
We divided ten people into two groups and gave half of the pairs to each group. The subjects were given sentences with pairs in them such as:
  龍 和 鳳 相關。
  “Dragon and phoenix are related to each other.”
  They were required to rate each statement according to ‘totally agree’, ‘agree’, ‘don’t know’, ‘don’t agree’ and ‘totally disagree’. We also added ‘don’t know X’ and ‘don’t know Y’ tags in case an annotator was not familiar with a given word. Only the pairs with three or more agree (including agree or totally agree) votes will be treated as positive results.
7) totally agree
8) agree
9) not sure
10) don't know X:
11) don't know Y:






