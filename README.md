## Project Overview

This project is the source code of the paper "Towards Improving the Explainability of Text-based Information Retrieval with Knowledge Graphs".

This project is a collaboration between Aggregate Intellect, McGill University, and Ryerson University on explainable information retrieval. Information retrieval and search systems normally use various techniques to generate candidates and then to rank them. Users’ trust of the shortlisting and then ranking process has a significant impact on their willingness to use the system.

This project aims to explore various post-hoc and embedded methods that can be used to introduce explainability to systems like this. The group will then move on to implement a few potential solutions, and package those as open source libraries. The goal is to create open source libraries and publish papers on the topics of post-hoc or embedded explainability in Info Retrieval, Search, or related tasks. 

more resources at here: [ai.science resources](https://ai.science/l/236a6202-3495-4a8e-bbad-aedeee4bd21d@/assets)


## Approach:

#### Knowledge Graph for Most Important Sentence
The most important sentence (MIS) is the most relevant part of a passage and explains how the passage is related to the query. We identified the entities in the query, matched entities with the knowledge graph, and expanded the query using the information retrieved from the knowledge graph. The expanded query is used for retrieving the most important sentence and improving the explainability.

code: [manually_entity_retriever.ipynb](https://github.com/Aggregate-Intellect/xir/blob/main/query_expansion_kg/manually_entity_retriever.ipynb)
Manually labeled data: [entity&relationship_extraction.csv](https://github.com/Aggregate-Intellect/xir/blob/main/query_expansion_kg/entity%26relationship_extraction.csv)

#### Knowledge Graph for Reranking
After entity matching, an explainable feature of query-document relatedness is proposed, which relies on entity relatedness calculated from knowledge graph to find how two texts are related to each other. Basically, two texts are first translated into a list of entities, and then the pair-to-pair entity relatedness score is calculated and aggregated to represent the relatedness of two texts which, in our case, are the query and the document.

code: [robust04_Reranking_Document.ipynb](https://github.com/Aggregate-Intellect/xir/blob/main/reranking_kg/robust04_Reranking_Document.ipynb)

## datasets:

#### Wikidata

#### wikiQA
- 3000+ search queries start with a WH-word
- all candidate sentences are from wikipedia summary paragraph
- sentence that answer the question is labeled manually
more information is at https://aclanthology.org/attachments/D15-1237.Presentation.pptx

#### Robust04
- Due to the copyright, please email yujing.yang2@mail.mcgill.ca to get the dataset. 
- API related to robust04 dataset (developed by ir_dataset) [robust04_ir_dataset.ipynb](https://github.com/Aggregate-Intellect/xir/blob/main/reranking_kg/robust04_ir_dataset.ipynb)

#### BEIR
- https://huggingface.co/datasets/BeIR/beir

#### 2022 Clinical Trials Track
- https://www.trec-cds.org/2022.html

## current work:
Building IR using robust04 dataset and vector search [robust04_Reranking_Document.ipynb](https://github.com/ChenKua/xir/blob/main/reranking_kg/robust04_Processed_DS_Haystack.ipynb)

Building IR using BEIR (scifact) dataset and BEIR vector search [BEIR_dataset.ipynb](https://github.com/Aggregate-Intellect/xir/blob/main/BEIR_dataset.ipynb)

Building QA using BEIR (scifact) dataset and Haystack DensePassageRetriever [Haystack_scifact_DensePassageRetriever.ipynb](https://github.com/Aggregate-Intellect/xir/blob/main/Haystack_scifact_DensePassageRetriever.ipynb)

Building QA using wikipedia snippets dataset, with EmbeddingRetriever, Seq2SeqGenerator, and FARMReader from Haystack [haystack_wiki.ipynb](https://github.com/Aggregate-Intellect/xir/blob/main/haystack_wiki.ipynb)

Evaluation of information retrieval using haystack [haystack_evaluation.ipynb](https://github.com/Aggregate-Intellect/xir/blob/main/Haystack_evaluation.ipynb)

Passage-level retriever and sentence-level retriever on wikiQA dataset 
(passage-level accuracy: 0.98, sentence-level accuracy: 0.61)
[wikiQA_sentence_level_retriever.ipynb](https://github.com/Aggregate-Intellect/xir/blob/main/wikiQA_sentence_level_retriever.ipynb)

## Slide:
- [July 19 update](https://docs.google.com/presentation/d/1MSRtEfu1F7CeO0tNgg2Uzs_QBT2Y4f_Q92u_8wG9XSk/edit?usp=sharing)
- [July 11 update](https://docs.google.com/presentation/d/1X_ylGDiU-DLbVcgzU4qjKBBtwKOindJpChK4R4ngD50/edit?usp=sharing)
- [July 5 update](https://docs.google.com/presentation/d/1Xjq3BrhGhUpfGpPIfjJ1-Skss35qzlE_WhB4rzzHZh0/edit?usp=sharing)

