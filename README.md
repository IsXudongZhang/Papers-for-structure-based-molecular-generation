# Papers of structure-based molecular generation

## Contents

[1.  **arXiv 2023** PrefixMol: Target- and Chemistry-aware Molecule Design via Prefix Embedding ](#1.)




## Papers
### <a id="1."> **arXiv 2023** PrefixMol: Target- and Chemistry-aware Molecule Design via Prefix Embedding</a>  

**Motivation**:
Is there a unified model for generating molecules considering different conditions, such as binding pockets and chemical properties? Although target-aware generative models have made significant advances in drug design, they **do not consider chemistry conditions and cannot guarantee the desired chemical properties**. Unfortunately, merging the target-aware and chemical-aware models into a unified model to meet customized requirements may lead to the problem of negative transfer.

**Contibution**:
Inspired by the success of multi-task learning in the NLP area, we use prefix embeddings to provide a novel generative model that considers both the targeted pocket’s circumstances and a variety of chemical properties. All conditional information is represented as learnable features, which the generative model subsequently employs as a contextual prompt. 

**Results**:
Experiments show that our model exhibits good controllability in both single and multi-conditional molecular generation. The controllability enables us to outperform previous structure-based drug design methods. More interestingly, we open up the attention mechanism and reveal coupling relationships between conditions, providing guidance for multi-conditional molecule generation.
<img width="1058" alt="image" src="https://github.com/IsXudongZhang/Papers-for-structure-based-molecular-generation/assets/105139522/f9e2995d-c7ce-4fb5-93b6-f76023ba725e">

[Go To Top](#top)

<br>
