- Pointwise
    - Relevence Generation: 
    Prompt:
    Passage:{passage}, Query:{query}. Does the passage answer the query?
    Excepted output:
    Yes/NO
    $Score = 1 + P(Yes)$ or $Score = 1 - P(No)$
    - Query Generation: $P(Q^*|passage)$
    - Issue:
        - Can not get the probability from API
        - For ranking tasks, we don't need explicitly the scores but relative order.
    
- Listwise
    - Issue:
        - Missing: Lack of some items
        - Rejection: Refuse to rank and generate Irrelevent outputs
        - Repetition: Output the same item more than once.
        - Inconsistency: Output different rankings for reordered input.
    
- Pairwise: (This paper propses:)
    - Do double evaluation with the inversed order: S(T1, T2) and then S(T2, T1).
    
    - PRP-ALLpair: $S_i = 1\cdot \sum_{j \neq i}\mathbb{I}_{d_i \gt d_j}+0.5\sum_{j \neq i}\mathbb{I}_{d_i = d_j}$
    
      
