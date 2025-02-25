# M3-Embedding: Multi-Linguality, Multi-Functionality, Multi-Granularity Text Embeddings Through Self-Knowledge Distillation

- M3: Linguality, Functionality, Granualrity
- Task?: Long-document Retrieval?
- Semantic Retrieval
    - Dense
    - Multi-Vector (Only for Long Input?)
    - Sparse (Frequence-based)
- Versatility Issues:
    - Only English
    - Single Retrieval Functionality
    - Only short inputs support for long-doc retrieval
- Langs: 100+
- Self Knowledge distillation: Multiple retrieval functionalities jointly learn
- Teacher Signal ??? relevance scores from different retrieval functions?
- Data Curation from 3 sources:
    - Extraction **Unsupervised data**: title-body, title-abstract...
    - Intergrate the related **supervised data**
        - Parallel training for cross-lingual semantic matching:
            - NLLB
            - CCMatrix
    - Synthesize scarce training data
- Multilingual Benchmark:
    - MIRACL
    - MKQA




