## Project Overview

This project is a collaboration between Aggregate Intellect, McGill University, and Ryerson University on explainable information retrieval. Information retrieval and search systems normally use various techniques to generate candidates and then to rank them. Users’ trust of the shortlisting and then ranking process has a significant impact on their willingness to use the system.

This project aims to explore various post-hoc and embedded methods that can be used to introduce explainability to systems like this. The group will then move on to implement a few potential solutions, and package those as open source libraries. The goal is to create open source libraries and publish papers on the topics of post-hoc or embedded explainability in Info Retrieval, Search, or related tasks. 

## Project resources
https://ai.science/l/236a6202-3495-4a8e-bbad-aedeee4bd21d@/assets

## datasets:
Due to the copyright, please email me at yujing.yang2@mail.mcgill.ca to get the dataset. 

API related to robust04 dataset (developed by ir_dataset) [robust04_ir_dataset.ipynb](https://github.com/Aggregate-Intellect/xir/blob/main/robust04_ir_dataset.ipynb)

#### BEIR
https://huggingface.co/datasets/BeIR/beir

#### 2022 Clinical Trials Track
https://www.trec-cds.org/2022.html

## current work:
Building IR using robust04 dataset and vector search [robust04_Processed.ipynb](https://github.com/Aggregate-Intellect/xir/blob/main/robust04_Processed.ipynb)

Building IR using BEIR (scifact) dataset and BEIR vector search [BEIR_dataset.ipynb](https://github.com/Aggregate-Intellect/xir/blob/main/BEIR_dataset.ipynb)

Building QA using BEIR (scifact) dataset and Haystack DensePassageRetriever [Haystack_scifact_DensePassageRetriever.ipynb](https://github.com/Aggregate-Intellect/xir/blob/main/Haystack_scifact_DensePassageRetriever.ipynb)

Building QA using wikipedia snippets dataset, with EmbeddingRetriever, Seq2SeqGenerator, and FARMReader from Haystack [haystack_wiki.ipynb](https://github.com/Aggregate-Intellect/xir/blob/main/haystack_wiki.ipynb)
