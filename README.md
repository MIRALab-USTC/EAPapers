# Must-read papers on Entity Alignment (EA)

## [Content](#content)
- <a href="#triplet-based-models">Triplet-based Models</a>
- <a href="#path-based-models">Path-based Models</a>
- <a href="#graph-based-models">Graph-based Models</a>

## [Triplet-based Models](#content)

1. **Multilingual Knowledge Graph Embeddings for Cross-lingual Knowledge Alignment**. IJCAI 2017. [[Paper](https://arxiv.org/abs/1611.03954)]  
    *Muhao Chen, Yingtao Tian, Mohan Yang, Carlo Zaniolo*.
    
    > This paper proposes **MTransE**, a translation-based model for multilingual knowledge graph embeddings. By encoding entities and relations 
      of each language in a separated embedding space, MTransE provides transitions for each embedding vector to its cross-lingual counterparts in
      other spaces, while preserving the functionalities of monolingual embeddings.

1. **Cross-lingual Entity Alignment via Joint Attribute-Preserving Embedding**. ISWC 2017. [[Paper](https://arxiv.org/abs/1708.05045)]  
    *Zequn Sun, Wei Hu, Chengkai Li*.
    
    > This paper proposes a joint attribute-preserving embedding (**JAPE**) model for cross-lingual entity alignment. It jointly embeds the structures
      of two KBs into a unified vector space and further refines it by leveraging attribute correlations in the KBs.


## [Path-based Models](#content)

1. **Learning to Exploit Long-term Relational Dependencies in Knowledge Graphs**. ICML 2019. [[Paper](https://arxiv.org/abs/1708.05045)]  
    *Lingbing Guo, Zequn Sun, Wei Hu*.
    
    > This paper proposes recurrent skipping networks (RSNs), which employ a skipping mechanism to bridge the gaps between entities. 
      RSNs integrate recurrent neural networks (RNNs) with residual learning to efficiently capture the long-term relational dependencies within and between KGs.


## [Graph-based Models](#content)

1. **Cross-lingual Knowledge Graph Alignment via Graph Convolutional Networks**. EMNLP 2018. [[Paper](https://www.aclweb.org/anthology/D18-1032/)]  
    *Zhichun Wang, Qingsong Lv, Xiaohan Lan, Yu Zhang*.
    
    > This paper proposes **GCN-Align**, which is the first work to adopt graph convolutional networks (GCNs) for entity alignment.

1. **Relation-Aware Entity Alignment for Heterogeneous Knowledge Graphs**. IJCAI 2019. [[Paper](https://arxiv.org/abs/1908.08210)]  
    *Yuting Wu, Xiao Liu, Yansong Feng, Zheng Wang, Rui Yan, Dongyan Zhao*.
    
    > This paper proposes a novel Relation-aware Dual-Graph Convolutional Network (**RDGCN**) to incorporate relation information via attentive 
      interactions between the knowledge graph and its dual relation counterpart, and further capture neighboring structures to learn better entity representations.


1. **Jointly Learning Entity and Relation Representations for Entity Alignment**. EMNLP 2019. [[Paper](https://arxiv.org/abs/1909.09317)]  
    *Yuting Wu, Xiao Liu, Yansong Feng, Zheng Wang, Dongyan Zhao*.
    
    > This paper proposes **HGCN**. Instead of relying on pre-aligned relation seeds to learn relation representations, it first approximates them 
      using entity embeddings learned by the GCN. It then incorporate the relation approximation into entities to iteratively learn better representations for both.

1. **A Vectorized Relational Graph Convolutional Network for Multi-Relational Network Alignment**. IJCAI 2019. [[Paper](https://www.ijcai.org/Proceedings/2019/0574.pdf)]  
    *Rui Ye, Xin Li, Yujie Fang, Hongyu Zang, Mingzhong Wang*.
    
    > This paper proposes **AVR-GCN**. It first proposes a vectorized relational graph convolutional network (VR-GCN) to learn the embeddings of both graph entities 
      and relations simultaneously for multi-relational networks. AVR-GCN, the alignment framework based on VR-GCN, is then developed for multi-relational network alignment
      tasks. Anchors are used to supervise the objective function which aims at minimizing the distances between anchors, and to generate new cross-network triplets to build 
      a bridge between different knowledge graphs at the level of triplet to improve the performance of alignment.

1. **Multi-Channel Graph Neural Network for Entity Alignment**. ACL 2019. [[Paper](https://arxiv.org/abs/1908.09898)]  
    *Yixin Cao, Zhiyuan Liu, Chengjiang Li, Zhiyuan Liu, Juanzi Li, Tat-Seng Chua*.
    
    > This paper proposes novel Multi-channel Graph Neural Network model (**MuGNN**) to learn alignment-oriented knowledge graph (KG) embeddings by robustly encoding two KGs 
      via multiple channels. Each channel encodes KGs via different relation weighting schemes with respect to self-attention towards KG completion and cross-KG attention for
      pruning exclusive entities respectively, which are further combined via pooling techniques.

1. **Knowledge Graph Alignment Network with Gated Multi-hop Neighborhood Aggregation**. AAAI 2020. [[Paper](https://arxiv.org/abs/1911.08936)]  
    *Zequn Sun, Chengming Wang, Wei Hu, Muhao Chen, Jian Dai, Wei Zhang, Yuzhong Qu*.
    
    > This paper proposes **AliNet**, aiming at mitigating the non-isomorphism of neighborhood structures in an end-to-end manner. As the direct neighbors of counterpart entities 
      are usually dissimilar due to the schema heterogeneity, AliNet introduces distant neighbors to expand the overlap between their neighborhood structures. It employs an attention 
      mechanism to highlight helpful distant neighbors and reduce noises. Then, it controls the aggregation of both direct and distant neighborhood information using a gating mechanism. 

1. **Coordinated Reasoning for Cross-Lingual Knowledge Graph Alignment**. AAAI 2020. [[Paper](https://arxiv.org/abs/2001.08728)]  
    *Kun Xu, Linfeng Song, Yansong Feng, Yan Song, Dong Yu*.
    
    > This paper introduces two coordinated reasoning methods, i.e., the Easy-to-Hard decoding strategy and joint entity alignment algorithm. 
      Specifically, the Easy-to-Hard strategy first retrieves the model-confident alignments from the predicted results and then incorporates them as
      additional knowledge to resolve the remaining model uncertain alignments.  

1. **COTSAE: CO-Training of Structure and Attribute Embeddings for Entity Alignment**. AAAI 2020. [[Paper](https://aaai.org/ojs/index.php/AAAI/article/view/5696)]  
    *Kai Yang, Shaoqin Liu, Junfeng Zhao, Yasha Wang, Bing Xie*.
    
    > This paper proposes **COTSAE** that combines the structure and attribute information of entities by co-training two embedding learning components, respectively. 
      This paper also proposes a joint attention method in our model to learn the attentions of attribute types and values cooperatively.

1. **Deep Graph Matching Consensus**. ICLR 2020. [[Paper](https://arxiv.org/abs/2001.09621)]  
    *Matthias Fey, Jan E. Lenssen, Christopher Morris, Jonathan Masci, Nils M. Kriege*.
    
    > This work presents a two-stage neural architecture for learning and refining structural correspondences between graphs. First, this paper uses localized
      node embeddings computed by a graph neural network to obtain an initial ranking of soft correspondences between nodes. Secondly, this paper employs 
      synchronous message passing networks to iteratively re-rank the soft correspondences to reach a matching consensus in local neighborhoods between graphs.

1. **Deep Graph Matching Consensus**. ICLR 2020. [[Paper](https://arxiv.org/abs/2001.09621)]  
    *Matthias Fey, Jan E. Lenssen, Christopher Morris, Jonathan Masci, Nils M. Kriege*.
    
    > This work presents a two-stage neural architecture for learning and refining structural correspondences between graphs. First, this paper uses localized
      node embeddings computed by a graph neural network to obtain an initial ranking of soft correspondences between nodes. Secondly, this paper employs 
      synchronous message passing networks to iteratively re-rank the soft correspondences to reach a matching consensus in local neighborhoods between graphs.

1. **Neighborhood Matching Network for Entity Alignment**. ACL 2020. [[Paper](https://arxiv.org/abs/2005.05607)]  
    *Yuting Wu, Xiao Liu, Yansong Feng, Zheng Wang, Dongyan Zhao*.
    
    > This paper presents Neighborhood Matching Network (NMN), a novel entity alignment framework for tackling the structural heterogeneity challenge. 
      NMN estimates the similarities between entities to capture both the topological structure and the neighborhood difference. It provides two innovative 
      components for better learning representations for entity alignment. It first uses a novel graph sampling method to distill a discriminative neighborhood 
      for each entity. It then adopts a cross-graph neighborhood matching module to jointly encode the neighborhood difference for a given entity pair.


