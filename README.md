# Review for structure based drug de novo design

# <a id="top">Molecular Generation</a>  

## 1. Structure-based

[1.  <span style="color: red;">arXiv 2023</span>  PrefixMol: Target- and Chemistry-aware Molecule Design via Prefix Embedding ](#1.)




<br>

### <a id="1."> <span style="color: red;">arXiv 2023</span> PrefixMol: Target- and Chemistry-aware Molecule Design via Prefix Embedding</a>  

**Motivation**: 
<span style="color: red;"> Is there a unified model for generating molecules considering different conditions, such as binding pockets and chemical properties?</span> Although targetaware generative models have made significant advances in drug design, they do not consider chemistry conditions and cannot guarantee the desired chemical properties. Unfortunately, merging the target-aware and chemical-aware models into a unified model to meet customized requirements may lead to the problem of negative transfer.

**Contibution**:
Inspired by the success of multi-task learning in the NLP area, <span style="color: red;">we use prefix embeddings to provide a novel generative model that considers both the targeted pocket’s circumstances and a variety of chemical properties.</span> All conditional information is represented as learnable features, which the generative model subsequently employs as a contextual prompt. 

**Results**:
Experiments show that our model exhibits good controllability in both single and multi-conditional molecular generation. The controllability enables us to outperform previous structure-based drug design methods. More interestingly, we open up the attention mechanism and reveal coupling relationships between conditions, providing guidance for multi-conditional molecule generation.

[Go To Top](#top)

<br>
