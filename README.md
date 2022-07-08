## Project Overview

This project is a collaboration between Aggregate Intellect, McGill University, and Ryerson University on explainable information retrieval. Information retrieval and search systems normally use various techniques to generate candidates and then to rank them. Users’ trust of the shortlisting and then ranking process has a significant impact on their willingness to use the system.

This project aims to explore various post-hoc and embedded methods that can be used to introduce explainability to systems like this. The group will then move on to implement a few potential solutions, and package those as open source libraries. The goal is to create open source libraries and publish papers on the topics of post-hoc or embedded explainability in Info Retrieval, Search, or related tasks. 

## datasets:
#### Robust 04
link to download dataset: https://ir.nist.gov/cd45/   
Username: TREC#cd45!   
Password: ZD3CmcA8?%EL

Please sign and keep the individual agreement: https://trec.nist.gov/data/cd45/ind_appl_trec.html

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
