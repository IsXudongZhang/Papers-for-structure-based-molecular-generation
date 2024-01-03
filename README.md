# Papers for structure-based molecular generation

## Contents

| Date | Journal | Title | Code | Remark |
| ---- | ---- | ---- | ---- | ---- |
| 2023 | arXiv | [PrefixMol: Target- and Chemistry-aware Molecule Design via Prefix Embedding](#1.) |  | Controllable generation | 
| 2023 | ICML | [DECOMPDIFF: Diffusion Models with Decomposed Priors for Structure-Based Drug Design](#2.) | https://github. com/bytedance/DecompDiff  | Diffusion model | 




---

## Papers

### <a id="1."> **arXiv 2023** || PrefixMol: Target- and Chemistry-aware Molecule Design via Prefix Embedding</a>  

**Motivation**:
Is there a unified model for generating molecules considering different conditions, such as binding pockets and chemical properties? Although target-aware generative models have made significant advances in drug design, they **do not consider chemistry conditions and cannot guarantee the desired chemical properties**. Unfortunately, merging the target-aware and chemical-aware models into a unified model to meet customized requirements may lead to the problem of negative transfer.

**Contibution**:
Inspired by the success of multitask learning in the NLP area, authors suggest **prepending learnable conditional feature vectors to the query and key of the attention module**, resulting in the PrefixMol method. The prefix embedding is always on the left side, serving as a task-related contextual prompt to affect the predicted outcomes on its right. These prefix embeddings are learned by auxiliary neural networks, considering the 3D pocket and chemical properties.

**Results**:
Experiments show that our model exhibits good controllability in both single and multi-conditional molecular generation. The controllability enables us to outperform previous structure-based drug design methods. More interestingly, we open up the attention mechanism and reveal coupling relationships between conditions, providing guidance for multi-conditional molecule generation.
<img width="1058" alt="image" src="https://github.com/IsXudongZhang/Papers-for-structure-based-molecular-generation/assets/105139522/f9e2995d-c7ce-4fb5-93b6-f76023ba725e">

[Go To Top](#top)

<br>

---
### <a id="2."> **ICML 2023** || DECOMPDIFF: Diffusion Models with Decomposed Priors for Structure-Based Drug Design</a>  

Designing 3D ligands within a target binding site is a fundamental task in drug discovery. Existing structured-based drug design methods treat all ligand atoms equally, which ignores different roles of atoms in the ligand for drug design and can be less efficient for exploring the large drug-like molecule space. In this paper, inspired by the convention in pharmaceutical practice, we decompose the ligand molecule into two parts, namely arms and scaffold, and propose a new diffusion model, DECOMPDIFF, with decomposed priors over arms and scaffold. In order to facilitate the decomposed generation and improve the properties of the generated molecules, we incorporate both bond diffusion in the model and additional validity guidance in the sampling phase. Extensive experiments on CrossDocked2020 show that our approach achieves state-of-the-art performance in generating high-affinity molecules while maintaining proper molecular properties and conformational stability, with up to −8.39 Avg. Vina Dock score and 24.5% Success Rate. The code is provided at 
**Motivation**:
Is there a unified model for generating molecules considering different conditions, such as binding pockets and chemical properties? Although target-aware generative models have made significant advances in drug design, they **do not consider chemistry conditions and cannot guarantee the desired chemical properties**. Unfortunately, merging the target-aware and chemical-aware models into a unified model to meet customized requirements may lead to the problem of negative transfer.

**Contibution**:
Inspired by the success of multitask learning in the NLP area, authors suggest **prepending learnable conditional feature vectors to the query and key of the attention module**, resulting in the PrefixMol method. The prefix embedding is always on the left side, serving as a task-related contextual prompt to affect the predicted outcomes on its right. These prefix embeddings are learned by auxiliary neural networks, considering the 3D pocket and chemical properties.

**Results**:
Experiments show that our model exhibits good controllability in both single and multi-conditional molecular generation. The controllability enables us to outperform previous structure-based drug design methods. More interestingly, we open up the attention mechanism and reveal coupling relationships between conditions, providing guidance for multi-conditional molecule generation.
<img width="1058" alt="image" src="https://github.com/IsXudongZhang/Papers-for-structure-based-molecular-generation/assets/105139522/f9e2995d-c7ce-4fb5-93b6-f76023ba725e">

[Go To Top](#top)

<br>
