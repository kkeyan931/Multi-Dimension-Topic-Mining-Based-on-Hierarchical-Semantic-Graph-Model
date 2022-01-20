# Multi-Dimension-Topic-Mining-Based-on-Hierarchical-Semantic-Graph-Model

## Introduction

Topic mining of scientiﬁc literature can accurately capture the contextual structure of a topic, 
track research hotspots within a ﬁeld, and improve the availability of information about the literature. 
This paper introduces a multi-dimensional topic mining method based on a hierarchical semantic graph 
model. 

The main innovations include 

(1) the hierarchical extraction of feature terms and construction of a corresponding semantic graph and

(2) multi-dimensional topic mining based on graph segmentation and structure analysis. The process of semantic graph construction is based primarily on hierarchical feature term extraction, which can effectively reveal the hierarchical structural distribution of feature terms within documents. Our graph model also takes into account the complementarity of content- and context-related feature terms in documents while avoiding the loss of textual information. In addition, the multi-dimensional features of the topic can be mined effectively via an in-depth analysis of the constructed graph, resulting in a quantitative visualization of the many-to-many association between the topic and feature terms. A variety of experiments on existing document datasets demonstrate that the proposed approach is able to outperform state-of-the-art methods in terms of accuracy and efﬁcacy.


<img width="523" alt="image" src="https://user-images.githubusercontent.com/65884897/150322993-25eb961f-d846-439b-b1f4-9fe6f30cdc12.png">


## SEMANTIC GRAPH CONSTRUCTION

First, the content correlation between feature terms is calculated based on co-occurrence. Second, the hierarchical extraction of feature terms is carried out to construct a semantic graph based on content correlation. Finally, the contextual correlation between feature terms is calculated based on word2vec, and the previously constructed graph is refined to generate the final semantic graph.

### A. TERM CORRELATION BASED ON CO-OCCURRENCE

The correlations between terms are represented by similarities P(Ti|Tj) and P(Tj|Ti) via the distribution of term frequencies in each paragraph. We use the symbol r(Ti, Tj) to represent the association between term Ti and term Tj:

<img width="289" alt="image" src="https://user-images.githubusercontent.com/65884897/150323773-f06f4243-efea-44fe-9b5c-5bfee6cade0b.png">


### B. SEMANTIC GRAPH CONSTRUCTION

Representing the document as a graph allows the retention of some important information, such as semantic relationships and internal structures.


### C. SEMANTIC GRAPH REFINEMENT

We use the word2vec model to refine the semanticterm graph by considering word embedding information. The essence of this procedure is to combine content correlation and contextual correlation in graph analysis for topic modelling.



