# Advancements-in-Manipuri-NLP
My repo "Advancements in Manipuri NLP" will provide a comprehensive study of research papers regarding Natural Language Processing (NLP) applications and developments of Manipuri language. It could be regarded as one of those "awesome" github repos for curated stuffs. 

**Note:** This is a work in progress. I will be updating every now and then.


## Introduction
Manipuri (Meiteilon), a language of Tibo-Burman origin is the official language and lingua franca of the northeast Indian state of Manipur. Despite its status as one of India's 22 Scheduled languages and a communication tool for over 1.5 million speakers across states like Manipur, Assam and Tripura, Manipuri remains a low resource language, impeded by sparse annotated data and technological advancements. While Manipuri boasts a rich morphology, complex agglutinative structure, and unique SOV word order, it also presents a thrilling challenge for NLP researchers. This is further compounded by its monosyllabic and compounding nature. Despite these complexities, researchers have made commendable strides in NLP applications like Part-of-Speech tagging, Name Entity Recognition, and machine translation. 

Interestingly, Manipuri uses two writing systems: the borrowed Bengali script and its own indigenous Meitei Mayek. While most research has focused on Bengali script, Meitei Mayek holds immense potential for future exploration. It's clear that significant progress is needed for both scripts to unlock the full potential of Manipuri NLP. This github repo will serve as the ultimate destination for the analysis of the NLP applications, approaches, challenges and future directions of Manipuri. I will post all papers and updates there has been in this realm with a summary and analysis.

## Index
1. [Morphological Analysis](#morphological-analysis)
2. [Syllabification, Stemming, Chunking](#syllabification-stemming-chunking)
3. [POS Tagging](#pOS-tagging)
4. [Named Entity Recognition](#named-entity-recognition)
5. [Word Sense Disambiguation](#word-sense-disambiguation)
6. [RMWE](#rmwe)
7. [Corpus Creation & E-Dictionary](#corpus-creation-&-e-dictionary)
8. [Parsing](#)
9. [Machine Translation](#machine-translation)
10. [Transliteration](#)
11. [Sentiment Analysis](#)
12. [Speech Technologies](#)



### Morphological Analysis

| Author & Date | Paper | Summary | 
|:-----------:|:------------:|:------------| 
| Choudhury et al.,2004   | [Morphological Analyzer for Manipuri: Design and Implementation](https://link.springer.com/chapter/10.1007/978-3-540-30176-9_16)    | implements a Manipuri morphological analyzer by employing Morphographemics and Morphotactics, alongside a model addressing orthographic variations and morphosyntactic feature combinations.    
| Singh et al.,2005     | [Manipuri Morphological Analyzer](https://www.academia.edu/1150157/Manipuri_Morphological_Analyzer)    | utilizes a Manipuri-English dictionary for identifying word morphemes and an affix dictionary for categorizing affix types.
| Singh et al.,2006 | [Word Class and Sentence Type Identification in Manipuri Morophological Analyzer](https://www.academia.edu/1150153/Word_Class_and_Sentence_Type_Identification_in_Manipuri_Morophological_Analyzer)     | The developed Manipuri Morphological Analyzer, utilizing a Manipuri-English dictionary for root words and an affix dictionary for affix types, yields surface-level word analysis aiding in the development of a Manipuri-English machine translation system, showcasing promising results.     |
| Nongmeikapam et al.,2012     | [Manipuri Morpheme Identification](https://aclanthology.org/W12-5008.pdf) | This approach used involves segmenting Manipuri words into syllables and employing 2-gram analysis with Standard Deviation technique for morpheme identification, achieving recall of 59.80%, precision of 83.02%, and an f-score of 69.52%.   |
| Singha et al.,2012     | [Morphological Analysis for Manipuri Nominal Category Words with Finite State Techniques](https://research.ijcaonline.org/volume58/number15/pxc3883688.pdf) | The paper proposes a suffix stripping approach for analyzing nominal category Manipuri words, utilizing finite state machines to model morphotactics and converting non-deterministic finite automata to deterministic finite automata, facilitating morphological analysis without a lexicon. | 
| Singha et al.,2013    | [Morphotactics of Manipuri Adjectives: A FiniteState Approach](https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=4aaa66c6f90c51a9feb8ddc9629548b7d7c3c500)     |This paper presents a constrained finite-state model to represent the morphotactic rule of Manipuri adjective word forms, which are derived from verb roots using specific affixes, with rules composed to describe their simple agglutinative morphology and more complex structures, resulting in a system capable of analyzing and recognizing adjectives through finite-state networks, utilizing a root lexicon and an affix dictionary.  |
| Devi et al.,2015     | [Manipuri morphological generator](https://ieeexplore.ieee.org/abstract/document/7377324/similar#similar)     | The paper presents a morphological generator for Manipuri, focusing on inflecting root words to cater to the complex morphology of Manipuri nouns and verbs, with coverage directly tied to the size of the root list. | 
|  Bablu et al.,2017     | [Morphological Analysis of Manipuri Language](https://www.caeaccess.org/archives/volume6/number8/bablu-2017-cae-652527.pdf)     | The Morphological Analyzer for Manipuri applies computational morphology principles to analyze Manipuri word forms, achieving an 80\% accuracy rate when tested on 3500 Manipuri words in Shakti Standard format using Meitei Mayek script as a source.  | 
| Devi et al.,2020     | [Morphotactics of Manipuri Verbs: A Finite State Approach](https://www.researchgate.net/publication/339709527_Morphotactics_of_Manipuri_Verbs_A_Finite_State_Approach)     | The paper investigates the morphotactics of Manipuri verbs using a Finite State Approach, crucial for understanding word formation in this language, where verbs serve as the main morphology and all other word forms are derived from them through affixation, providing essential insights for Natural Language Processing applications  | 
| Bablu et al.,2020     | [Manipuri Morphological Analysis](https://trp.org.in/wp-content/uploads/2021/01/AJCST-Vol.9-No.2-July-December-2020-pp.-4-10.pdf)    |The Morphological Analyzer for Manipuri language, tested on 4500 Manipuri lexicons using Meitei Mayek Unicode as a source, achieves an 84% accuracy rate, providing valuable grammatical information associated with the lexicon for Natural Language Processing applications. |
| Devi et al.,2022    | [Allomorphs in Meeteilon (Manipuri) Morphology](https://www.nepjol.info/index.php/lsnj/article/view/46557)  | The paper focuses on studying the distribution of phonologically conditioned allomorphs in Meeteilon morphology to understand its morphosyntactic nature, facilitating morpheme segmentation, identification, and parts of speech tagging for natural language processing, alongside an introduction to an optimality theory approach for syllable final devoicing |



### Syllabification, Stemming, Chunking
| Author & Date | Paper | Summary | 
|:-----------:|:------------:|:------------|
| Nongmeikapam et al.,2012     | [Automatic Segmentation of Manipuri (Meiteilon) Word into Syllabic Units](https://arxiv.org/abs/1207.3932)     | This paper presents an algorithmic approach for automatic segmentation of Manipuri language words into syllabic units, achieving a Recall of 74.77, Precision of 91.21, and F-Score of 82.18. | 
| Nandakishor et al.,2015     | [An HMM based semi-automatic syllable labeling system for Manipuri language](https://ieeexplore.ieee.org/document/7148548)     | This paper develops a Semi-Automatic Syllable Labeling System for Manipuri, utilizing HMM toolkit (HTK) and WaveSurfer, achieving an average deviation of 25 ms and employing detection rates based on time deviations for syllable segmentation. |
| Gyanendro et al.,2016     | [Automatic Syllabification for Manipuri language](https://aclanthology.org/C16-1034/)     | This paper introduces a data-driven method for automatic syllabification by employing entropy-based phonotactic segmentation, sequence labeling approaches, and a hybrid method, achieving up to 98\% word accuracy.|
| Devi et al.,2017     | [Automatic Syllabification Rules for Manipuri Language](https://www.ijarcs.info/index.php/Ijarcs/article/view/2852/0)     |This paper introduces an algorithmic approach for automatic syllabification of the language, achieving 99.8\% accuracy compared to manual syllabification, crucial for tasks like text-to-speech conversion and speech recognition.  |
| Nongmeikapam et al.,2014     | [Chunking in Manipuri Using CRF](https://airccse.org/journal/ijnlc/papers/3314ijnlc12.pdf)     |The paper presents a chunking approach for Manipuri language utilizing Conditional Random Field (CRF) for Part of Speech (POS) tagging, achieving a recall of 71.30\%, precision of 77.36\%, and F-measure of 74.21\%. |
| Nongmeikapam et al.,2014     | [Manipuri Chunking: An Incremental Model with POS and RMWE](https://aclanthology.org/W14-5140/)     | This paper utilizes Support Vector Machine (SVM) for chunking, incorporating Part of Speech (POS) tagging and Reduplicated Multiword Expression (RMWE) features, achieving a final chunking with a recall of 70.45\%, precision of 86.11\%, and F-measure of 77.50\%  |
| Meetei et al.,2015     | [Development of a Manipuri stemmer: A hybrid approach](https://ieeexplore.ieee.org/document/7377328)     |This paper introduces a brute force stemming algorithm for Manipuri, incorporating a suffix stripping technique, crucial for enhancing information retrieval systems in the Manipuri language domain.  |


### POS Tagging
| Author & Date | Paper | Summary | 
|:-----------:|:------------:|:------------|
| Doren et al.,2008    | [Morphology Driven Manipuri POS Tagger](https://aclanthology.org/I08-3015.pdf)     | This paper introduces a morphology-driven POS tagger for Manipuri language, utilizing dictionaries of root words, prefixes, and suffixes to achieve an accuracy of 69\% on 3784 sentences containing 10917 unique words. |
| Doren et al.,2008   | [Manipuri POS Tagging using CRF and SVM: A Language Independent Approach](https://www.academia.edu/1150196/Manipuri_POS_Tagging_using_CRF_and_SVM_A_Language_Independent_Approach)     | This improves the performance of the above Manipuri POS tagger using Conditional Random Field (CRF) and Support Vector Machine (SVM), achieving accuracies of 72.04\% and 74.38\% respectively. |
| Nongmeikapam et al.,2010  | [CRF Based POS Tagging of Manipuri](https://www.academia.edu/1856859/CRF_Based_POS_Tagging_of_Manipuri)     | This CRF approach achieves a recall of 70.00\%, precision of 77.78\%, and F-measure of 73.68\% |
| Singha et al.,2012     | [Part of Speech Tagging in Manipuri: A Rule-based Approach](https://research.ijcaonline.org/volume51/number14/pxc3881727.pdf)     | This paper presents a rule-based Part of Speech (POS) tagger for Manipuri, employing hand-written linguistic rules and affix stripping technique to handle the challenges of classifying the lexical categories.   |
| Nongmeikapam et al.,2012     | [Improvement of CRF Based Manipuri POS Tagger by Using Reduplicated MWE (RMWE)](https://www.semanticscholar.org/paper/Improvement-of-CRF-Based-Manipuri-POS-Tagger-by-MWE-Nongmeikapam/8994caf486abbae92e6bb121fc6608828a4beefd)     | This paper presents a modified feature selection approach for Conditional Random Field (CRF) based Manipuri Part of Speech (POS) tagging, achieving improved performance with a recall of 80.20\%, precision of 74.31\%, and F-measure of 77.14\% by incorporating Reduplicated Multiword Expression (RMWE) as an additional feature.  |
| Nongmeikapam et al.,2012    | [A Transliteration of CRF based Manipuri POS Tagging](https://www.sciencedirect.com/science/article/pii/S2212017312006159#aep-article-footnote-id3)     | This paper employs Conditional Random Field (CRF) for Part of Speech (POS) tagging of Bengali Script Manipuri text, followed by transliteration to Meitei Mayek script. |
| Nongmeikapam et al.,2012    | [Transliterated SVM Based Manipuri POS Tagging](https://link.springer.com/chapter/10.1007/978-3-642-30157-5_98)     |This presents a Support Vector Machine (SVM) approach for Part of Speech (POS) tagging of Bengali Script Manipuri text, followed by transliteration to Meitei Mayek.|
| Nongmeikapam et al.,2012     | [SVM based Manipuri POS tagging using SVM based identified reduplicated MWE (RMWE)](https://dl.acm.org/doi/10.1145/2381716.2381767)     |This paper employs Support Vector Machine (SVM) for identifying Reduplicated Multiword Expressions (RMWE) in Manipuri, achieving a recall of 86.11\%, precision of 92.08\%, and F-measure of 88.99\%, and subsequently utilizes these identified RMWE as features in SVM-based POS tagging, yielding a recall of 71.15\%, precision of 83.15\%, and F-measure of 76.68\%. |
| Nongmeikapam et al.,2012     | [Will the Identification of Reduplicated Multiword Expression (RMWE) Improve the Performance of SVM Based Manipuri POS Tagging?](https://link.springer.com/chapter/10.1007/978-3-642-28604-9_10)     | This inspects a possible performance improvement of SVM based Manipuri POS tagging by incorporating identified Reduplicated Multiword Expressions (RMWEs) as an additional feature, resulting in improved performance with an F-Score increase from 77.67\% to 79.61\%. |
|Singha et al.,2012     | [Part of Speech Tagging in Manipuri with Hidden Markov Model](https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=61269edc218657f89014ee616324773de9f689ca)     | This paper employs a stochastic model, Hidden Markov Model, for Part of Speech Tagging in Manipuri, utilizing the tagged output of the Manipuri rule-based tagger as the tagged corpus.  |

### Named Entity Recognition
| Author & Date | Paper | Summary | 
|:-----------:|:------------:|:------------|
| Doren et al.,2009  | [Named Entity Recognition for Manipuri Using Support Vector Machine](https://aclanthology.org/Y09-2045.pdf)     | This paper presents the development of a Manipuri Named Entity Recognition (NER) system utilizing Support Vector Machine (SVM) and active learning techniques, achieving an overall average Recall of 93.91\%, Precision of 95.32\%, and F-Score of 94.59\%. |
| Doren et al.,2010    | [Web Based Manipuri Corpus for Multiword NER and Reduplicated MWEs Identification using SVM](https://aclanthology.org/W10-3605.pdf)     | This paper describes the development of a web-based Manipuri corpus for identifying reduplicated multiword expressions (MWE) and multiword named entities (NE) using a Support Vector Machine (SVM) learning technique, achieving recall, precision, and F-score values of 94.62\%, 93.53\%, and 94.07\% respectively for reduplicated MWEs, and 94.82\%, 93.12\%, and 93.96\% respectively for multiword NE. |
| Nongmeikapam et al.,2011   | [CRF based Name Entity Recognition (NER) in Manipuri: A highly agglutinative Indian Language](https://ieeexplore.ieee.org/document/5751390)     |This paper employs Conditional Random Field (CRF) for Manipuri Name Entity Recognition (NER), achieving a Recall of 81.12\%, Precision of 85.67\%, and F-Score of 83.33\%.  |
| Jimmy et al.,2013   | [Named Entity Recognition in Manipuri: A Hybrid Approach](https://link.springer.com/chapter/10.1007/978-3-642-40722-2_11)     |This paper introduces a hybrid approach to Named Entity Recognition (NER) in Manipuri language, combining Conditional Random Field (CRF) statistical approach with rule-based techniques, achieving Recall, Precision, and F-score of 92.26\%, 94.27\%, and 93.3\% respectively. |
| Jimmy et al.,2020    | [Deep Neural Model for Manipuri Multiword Named Entity Recognition with Unsupervised Cluster Feature](https://aclanthology.org/2020.icon-main.57/)     |This paper presents an approach for recognizing Multi-Word Named Entities (MNEs) in Manipuri using a Long Short Term Memory (LSTM) recurrent neural network model augmented with Part Of Speech (POS) embeddings and word cluster information obtained through K-means clustering, demonstrating performance comparison with other machine learning-based models.  |
| Jimmy et al.,2022     | [BiLSTM-CRF Manipuri NER with Character-Level Word Representation](https://link.springer.com/article/10.1007/s13369-022-06933-z)     |This paper proposes a Manipuri Named Entity Recognition (NER) model employing Bidirectional Long Short Term Memory (BiLSTM) deep neural network with character-level word representation and word embedding, augmented by a Conditional Random Field (CRF) classifier, achieving an F-Score measure of approximately 98.19\% with RMSprop Gradient Descent (GD) optimizer, and an average clustering accuracy of 88.14\% for all NE classes. |


### Word Sense Disambiguation
| Author & Date | Paper | Summary | 
|:-----------:|:------------:|:------------|
| Singh et al.,2014    | [Word Sense Disambiguation](https://airccse.org/journal/acij/papers/5414acij03.pdf)     |  This paper introduces a word sense disambiguation system for Manipuri language, employing conventional positional and context-based features to predict the senses of polysemous words with an accuracy of 71.75\%.   |

## RMWE 
| Author & Date | Paper | Summary | 
|:-----------:|:------------:|:------------|
| Nongmeikapam et al.,2011  | [Identification of Reduplicated MWEs in Manipuri: A Rule Based Approach](https://www.researchgate.net/profile/Kishorjit-Nongmeikapam/publication/224960630_Kishorjit_Nongmeikapam_Sivaji_BandyopadhyayIdentification_of_Reduplicated_MWEs_in_Manipuri_A_Rule_based_Approached/links/09e414fb5fbaca3b1d000000/Kishorjit-Nongmeikapam-Sivaji-Bandyopadhyay-Identification-of-Reduplicated-MWEs-in-Manipuri-A-Rule-based-Approached.pdf)     |  This paper developes a rule-based model to identify reduplicated Multiword Expressions (MWEs) in Manipuri language texts, achieving an overall average Recall of 94.24\%, Precision of 82.27\%, and F-Score of 87.68\%.   |
|  Nongmeikapam et al.,2010   | [Identification of MWEs Using CRF in Manipuri and Improvement Using Reduplicated MWEs](https://www.semanticscholar.org/paper/Identification-of-MWEs-Using-CRF-in-Manipuri-and-Bandyopadhyay/a2c55e1b672b5eba4c9c9771bb26edc3e0bb388c)     | This paper employs Conditional Random Field (CRF) machine learning techniques for identifying Multiword Expressions (MWE) in Manipuri text, achieving a recall of 62.24\%, precision of 86.06\%, and F-measure of 72.24\% after accounting for reduplicated MWEs.  |
| Doren et al.,2010     | [Web Based Manipuri Corpus for Multiword NER and Reduplicated MWEs Identification using SVM](https://aclanthology.org/W10-3605/)     | The paper presents a novel approach utilizing support vector machine (SVM) learning technique for identifying reduplicated multiword expressions (MWE) and multiword named entities (NER) in a web-based Manipuri corpus, achieving recall, precision, and F-score values of 94.62\%, 93.53\%, and 94.07\% respectively for reduplicated MWE. |
| Nongmeikapam et al.,2011  | [Transliteration of CRF Based Multiword Expression (MWE) in Manipuri](https://ijcsit.com/docs/Volume%202/vol2issue4/ijcsit2011020415.pdf)     | The study focuses on the transliteration of identified Multiword Expressions (MWE) in Manipuri using Conditional Random Field (CRF), achieving a recall of 64.08\%, precision of 86.84\%, and F-measure of 73.74\%, with an accuracy of 90.01\% when comparing the transliterated output with both Meitei Script and Bengali Script Manipuri. |
| Nongmeikapam et al.,2011    | [Identification of Reduplicated Multiword Expressions Using CRF](https://link.springer.com/chapter/10.1007/978-3-642-19400-9_4)     | The study focuses on the identification of Reduplicated Multiword Expressions (RMWEs) in Manipuri language texts using Conditional Random Field (CRF) tool, achieving overall average recall, precision, and F-score values of 92.91\%, 91.90\%, and 92.40\% respectively.   |
| Nongmeikapam et al.,2011     | [Genetic Algorithm (GA) in Feature Selection for CRF Based Manipuri Multiword Expression (MWE) Identification](https://arxiv.org/abs/1111.2399)     | The paper presents a feature selection approach using Genetic Algorithm (GA) to enhance the identification of Multiword Expressions (MWEs) in Manipuri using Conditional Random Field (CRF), achieving a recall of 64.08\%, precision of 86.84\%, and F-measure of 73.74\%, demonstrating improvement over CRF-based MWE identification.   |


### Corpus Creation & E-Dictionary
| Author & Date | Paper | Summary | 
|:-----------:|:------------:|:------------|
| Doren et al.,2010    | [Semi–Automatic Parallel Corpora Extraction from Comparable News Corpora](https://www.scielo.org.mx/scielo.php?script=sci_arttext&pid=S1870-90442010000100003)     | The paper introduces a technique for extracting parallel corpus between Manipuri and English from web-collected news corpora, leveraging morphological information to improve alignment quality, thus demonstrating effectiveness for resource-constrained, agglutinative, and inflective Indian languages.|
| Doren et al.,2012    | [Building Parallel Corpora for SMT System: A Case Study of English-Manipuri](https://research.ijcaonline.org/volume52/number14/pxc3881876.pdf)     | The paper presents a technique for extracting parallel corpus between Manipuri and English from web-based comparable news corpora to improve translation quality in Statistical Machine Translation (SMT) systems for resource-constrained language pairs.|
| Moirangthem et al.,2022     | [Embeddings-Based Parallel Corpus Creation for English-Manipuri](https://link.springer.com/chapter/10.1007/978-981-99-2100-3_38)     | The paper introduces an efficient English-Manipuri automatic sentence aligner based on embeddings to create an English-Manipuri parallel corpus, reducing manual alignment effort by 47.72\% and facilitating neural machine translation in Low-Resource languages.|
| Huidrom et al.,2021    | [EM Corpus: a comparable corpus for a less-resourced language pair Manipuri-English](https://aclanthology.org/2021.bucc-1.8)     | The paper presents a sentence-level comparable text corpus for the Manipuri-English language pair, consisting of 1.88 million Manipuri sentences, 1.45 million English sentences, and 124,975 Manipuri-English sentence pairs crawled from 'The Sangai Express' website, aimed at supporting MT/NLP tasks for low-resourced languages. |
| Laitonjam et al.,2022    | [Manipuri–English comparable corpus for cross-lingual studies](https://link.springer.com/article/10.1007/s10579-021-09576-y)     | The paper introduces Mni-EnCC, a Manipuri–English comparable corpus, created by collating text from Sangai Express and Poknapham news sources, and verified through a semi-automated process, aiming to facilitate cross-lingual studies between Manipuri and English languages.|
| Ningombam et al.,2011   | [Building Manipuri-English Machine Readable Dictionary by Implementing Ontology](https://www.semanticscholar.org/paper/Building-Manipuri-English-Machine-Readable-by-Ningombam-Meitei/4db11aa18cc227abef0e93d8218b2c4eefea30a6)     |  The paper outlines the development process of a Manipuri-English machine-readable dictionary using ontology, aiming to provide an effective combination of traditional bilingual lexicographic information and conceptual knowledge essential for Natural Language Processing applications.|
| Meitei et al.,2012     | [An Analysis towards the Development of Electronic Bilingual Dictionary(Manipuri-English)-A Report](https://www.ijcsit.com/docs/Volume%203/Vol3Issue2/ijcsit2012030226.pdf)     |The paper outlines the ongoing development of an Electronic Manipuri Bilingual dictionary, aiming to provide a more effective combination of traditional English-Manipuri bilingual lexicographic information and conceptual knowledge essential for Natural Language Processing applications.  |
| Meitei et al.,2012     | [Word Search in a WWW Manipuri-English Electronic Dictionary](https://research.ijcaonline.org/volume55/number3/pxc3882969.pdf)     | The paper introduces an online Manipuri-English bilingual dictionary, emphasizing its word search functionality categorized into simple word search, wild card search, and search by lexical item, thereby contributing to language learning and natural language processing. |
| Meitei et al.,2017     | [DEVELOPMENT OF ENGLISH TO MANIPURI ELECTRONIC DICTIONARY: A database approach](https://www.researchgate.net/publication/316825188_DEVELOPMENT_OF_ENGLISH_TO_MANIPURI_ELECTRONIC_DICTIONARY_A_database_approach)     | The paper outlines the development of an electronic English to Manipuri dictionary based on a database model, providing an advanced alternative to traditional paper dictionaries for language learning and accessibility across various digital platforms.|
| Singh et al.,2017     | [Corpus & Wordnet Based MMD (Multilingual Manipuri Dictionary)]([https://www.semanticscholar.org/paper/Corpus-%26-Wordnet-Based-MMD-(-Multilingual-Manipuri-Singh-Purkayashtha/0c62c1c278f05908f5972cc21e967bef032d8175)](https://www.ijiras.com/2017/Vol_4-Issue_6/paper_14.pdf))     | The paper describes the development of MMD (Multilingual Manipuri Dictionary), employing a trie (M-ary tree) data structure, to facilitate language learning and various Natural Language Processing (NLP) tasks, including machine translation and corpus-based language processing.|

### Machine Translation
| Author & Date | Paper | Summary | 
|:-----------:|:------------:|:------------|
| Doren et al.,2010 | [Manipuri-English Example Based Machine Translation System](https://www.gelbukh.com/ijcla/2010-1-2/Manipuri-English%20Example.pdf)   | The paper presents a Manipuri-English example-based machine translation system, utilizing parallel corpus alignment techniques including POS tagging, morphological analysis, NER, and chunking, achieving BLEU and NIST scores of 0.137 and 3.361 respectively, outperforming a baseline SMT system with the same training and test data.   | 
| Doren et al.,2010    | [Statistical Machine Translation of English-Manipuri using Morpho-syntactic and Semantic Information](https://aclanthology.org/2010.amta-srw.1/)    |The paper introduces a factored Statistical Machine Translation (SMT) system for the English-Manipuri language pair, highlighting the significance of suffixes, dependency relations, and case markers in translation, resulting in improved translation quality, as evidenced by both BLEU score and subjective evaluation.  | 
| Doren et al.,2010    | [Manipuri-English Bidirectional Statistical Machine Translation Systems using Morphology and Dependency Relations](https://aclanthology.org/W10-3811/)     | The paper presents the development of bidirectional Manipuri-English statistical machine translation systems, highlighting the importance of suffixes, dependency relations, and case markers, with factored BLEU scores improved from 13.045 to 16.873 for English-Manipuri and from 13.452 to 17.573 for Manipuri-English translations, alongside subjective evaluation showing enhanced fluency and adequacy compared to baseline systems. | 
|Doren et al.,2011     | [Integration of Reduplicated Multiword Expressions and Named Entities in a Phrase Based Statistical Machine Translation System](https://aclanthology.org/I11-1146/)     |The paper presents the integration of reduplicated multiword expressions (RMWEs) and Multiword Named Entities (MNEs) into a Manipuri-English Phrase Based Statistical Machine Translation (PBSMT) system, utilizing SVM-based machine learning and GIZA++ alignment techniques, resulting in improved BLEU and NIST scores over baseline systems, as well as subjective evaluation indicating enhanced adequacy  | 
| Doren et al.,2012   | [Addressing some Issues of Data Sparsity towards Improving English-Manipuri SMT using Morphological Information](https://www.academia.edu/2973911/Addressing_some_Issues_of_Data_Sparsity_towards_Improving_English_Manipuri_SMT_using_Morphological_Information)     |The paper explores enriching parallel corpora resources for morphologically rich languages like Manipuri, enhancing SMT system performance in terms of both automatic scoring and subjective evaluation over baseline systems through mapping from source to target side using a factored model.    |
| Doren et al.,2013     | [Taste of Two Different Flavours: Which Manipuri Script Works Better for English-Manipuri Language Pair SMT Systems?](https://aclanthology.org/W13-0802.pdf)     |The paper compares the performance of phrase-based statistical machine translation (PBSMT) systems for the English-Manipuri language pair using Bengali script and transliterated Meitei Mayek script, showing that the Bengali script-based PBSMT outperforms in terms of BLEU and NIST scores, despite slight variations in subjective evaluation against automatic scores. | 
| Islam et al.,2017     | [A Review on  Electronic Dictionary and Machine Translation System Developed in North-East India](https://www.computerscijournal.org/vol10no2/a-review-on-electronic-dictionary-and-machine-translation-system-developed-in-north-east-india/)     |The paper discusses the importance and approaches of Electronic Dictionary (E-dictionary) and Machine Translation (MT) systems, highlighting their significance in Natural Language Processing (NLP), particularly in multilingual regions like North-East (NE) India, where few such systems have been developed, underscoring the growing demand for research in this area. | 
| Michael et al.,2020     | [Unsupervised Neural Machine Translation for English and Manipuri](https://aclanthology.org/2020.loresmt-1.10/)   |The paper introduces an unsupervised neural machine translation (UNMT) system for the low-resource English-Manipuri language pair, achieving BLEU scores of 3.1 for en → mni and 2.7 for mni → en translations, with subjective evaluation yielding encouraging results on the translated output.   |
| Meetei et al.,2020    | [English to Manipuri and Mizo Post-Editing Effort and its Impact on Low Resource Machine Translation](https://aclanthology.org/2020.icon-main.7/)     |The paper presents a study on post-editing effort in building a parallel dataset for English-Manipuri and English-Mizo, revealing positive correlations between technical effort and function words for both language pairs, and negative correlations between technical effort and noun words for English-Mizo, with an increase in HBLEU of up to 4.6 for English-Manipuri when using the post-edited dataset for incremental training.  |
| Huidrom et al.,2020     | [Zero-shot translation among Indian languages](https://aclanthology.org/2020.loresmt-1.7)  |The paper explores zero-shot translation on low-resource Indian languages, achieving an increase in translation accuracy, with a balanced data settings score multiplied by 7 for Manipuri to Hindi during Round-III of zero-shot translation.  |
| Laitonjam et al.,2021    | [Manipuri-English Machine Translation using Comparable Corpus](https://aclanthology.org/2021.mtsummit-loresmt.8/)     |The paper explores the effectiveness of unsupervised Machine Translation (MT) models over a Manipuri-English comparable corpus, demonstrating feasibility and identifying future directions for developing effective MT for the Manipuri-English language pair under unsupervised scenarios.   |
| Rahul et al.,2021 | [Statistical and Neural Machine Translation for Manipuri-English on Intelligence Domain](https://link.springer.com/chapter/10.1007/978-981-33-6987-0_21)     |The paper presents the development and outcomes of a Manipuri-English machine translation system in an intelligence domain, utilizing 56,678 parallel corpora from open-source intelligence (OSINT) sources, with statistical machine translation (SMT) achieving a BLEU score of 23.91 and neural machine translation (NMT) outperforming with a BLEU score of 40.67. Additionally, language-specific morphological analysis, particularly focusing on suffixes, yields further improvements, with SMT achieving a BLEU score of 25.03 and NMT achieving a BLEU score of 44. |
| Michael et al.,2022    | [Low resource machine translation of english–manipuri: A semi-supervised approach](https://www.sciencedirect.com/science/article/abs/pii/S0957417422013513)     |This paper introduces a semi-supervised neural machine translation system for English-Manipuri, employing self-training and back-translation techniques, yielding a +0.9 BLEU score improvement with external noise introduction, and outperforming supervised and mBART baselines by up to +4.5 and +1.2 BLEU improvements respectively. |
| Michael et al.,2022   | [An empirical study of low-resource neural machine translation of manipuri in multilingual settings](https://link.springer.com/article/10.1007/s00521-022-07337-8)     |This paper presents a multilingual LSTM-based neural machine translation system for Manipuri and English, incorporating cross-lingual features, which demonstrates improvement over vanilla multilingual and bilingual baselines, with enhanced performance across Manipuri-English and other Indian language-English translation tasks, including zero-shot translation evaluations. |
|Huidrom et al.,2022   | [Introducing EM-FT for Manipuri-English Neural Machine Translation](https://aclanthology.org/2022.wildre-1.1/)   |This paper employs pretrained fastText word embeddings for Manipuri, enhancing machine translation experiments using neural network models, where the Transformer architecture with fastText word embedding model EM-FT consistently outperforms alternatives, while noting a negative impact on translation accuracy with additional training data from a different domain.  |
|Devi et al.,2022 | [An Analysis of Phrase based SMT for English to Manipuri Language](https://aircconline.com/csit/papers/vol12/csit121904.pdf) |This paper presents a phrase-based Statistical Machine Translation (SMT) system from English to Manipuri, leveraging the Moses toolkit and Bengali script, and evaluates its performance using the BLEU metric on tourism, agriculture, and entertainment corpora. |
|Devi et al.,2023    |[An Exploratory Study of SMT Versus NMT for the Resource Constraint English to Manipuri Translation](https://link.springer.com/chapter/10.1007/978-981-99-3761-5_31)   |This study investigates and compares the performance of Statistical Machine Translation (SMT) and Neural Machine Translation (NMT) methods for English-to-Manipuri translation using BLEU, Meteor, TER, and F-measure scores as well as expert evaluation, to determine the most suitable approach for low-resource language pairs. |
| Singh et al.,2023    | [Subwords to Word Back Composition for Morphologically Rich Languages in Neural Machine Translation](https://aclanthology.org/2023.paclic-1.69/)     | This paper proposes a novel approach for neural machine translation (NMT) in morphologically rich languages, segmenting words into morphemes and composing word representations from them, showing improved translation accuracy over baseline subword models in Manipuri-English, Tamil-English, and Marathi-English translation tasks, highlighting the importance of leveraging word boundary information and interrelationships between word morphemes in NMT. |
|Lalrempuii et al.,2023     | [Low-Resource Indic Languages Translation Using Multilingual Approaches](https://link.springer.com/chapter/10.1007/978-981-99-6690-5_27)   |This study explores the effectiveness of multilingual pre-trained transformers—mBART and mT5—on low-resource Indic languages, including Hindi, Bengali, Assamese, Manipuri, and Mizo, comparing their performance with multiway multilingual translation trained from scratch using a one-to-many and many-to-one approach, highlighting the scalability of multilingual neural machine translation (MNMT) and its potential for improving translation quality in low-resource language settings.  |
|Pal et al.,2023   | [Findings of the WMT 2023 Shared Task on Low-Resource Indic Language](https://aclanthology.org/2023.wmt-1.56.pdf)    |This paper outlines the outcomes of the low-resource Indic language translation task conducted alongside the Eighth Conference on Machine Translation (WMT) 2023, where participants were tasked with developing machine translation systems for English-Assamese, English-Mizo, English-Khasi, and English-Manipuri language pairs. The evaluation of these systems will include both automatic metrics (BLEU, TER, RIBES, COMET, ChrF) and human assessment, utilizing the IndicNE-Corp1.0 dataset, comprising parallel and monolingual corpora for northeastern Indic languages like Assamese, Mizo, Khasi, and Manipuri.  |
|Singh et al.,2023     | [NITS-CNLP Low-Resource Neural Machine Translation Systems of English-Manipuri Language Pair](https://aclanthology.org/2023.wmt-1.92.pdf)     | This paper presents a transformer-based Neural Machine Translation (NMT) system developed by NITS-CNLP for the English-Manipuri language pair, achieving BLEU scores of 22.75 for English to Manipuri and 26.92 for Manipuri to English translations, along with character level n-gram F-score (chrF), RIBES, TER, and COMET evaluations.  |
|Agrawal et al.,2023     | [Neural Machine Translation for English - Manipuri and English - Assamese](https://aclanthology.org/2023.wmt-1.86.pdf)  |In the WMT23 shared task: low resource Indic language translation challenge, our team, ATULYA-NITS, utilized the NMT transformer model for English to/from Assamese and English to/from Manipuri language translation, achieving BLEU scores of 15.02 and 18.7 for English to Manipuri and Manipuri to English translations respectively, as well as 5.47 for English to Assamese and 8.5 for Assamese to English translations.  |
