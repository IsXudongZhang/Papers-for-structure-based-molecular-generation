# Papers for structure-based molecular generation

## Contents

| Date | Journal | Title | Link | Remark |
| ---- | ---- | ---- | ---- | ---- |
| 2023 | arXiv | [PrefixMol: Target- and Chemistry-aware Molecule Design via Prefix Embedding](#1.) | [[paper]](https://arxiv.org/abs/2302.07120) | Controllable generation | 
| 2023 | ICML | [DECOMPDIFF: Diffusion Models with Decomposed Priors for Structure-Based Drug Design](#2.) | [[paper]](https://openreview.net/forum?id=9qy9DizMlr) [[github]](https://github.com/bytedance/DecompDiff)  | Diffusion model | 




---

## Papers

### <a id="1."> **arXiv 2023** || PrefixMol: Target- and Chemistry-aware Molecule Design via Prefix Embedding</a>  

**Motivation**:
Is there a unified model for generating molecules considering different conditions, such as binding pockets and chemical properties? Although target-aware generative models have made significant advances in drug design, they **do not consider chemistry conditions and cannot guarantee the desired chemical properties**. Unfortunately, merging the target-aware and chemical-aware models into a unified model to meet customized requirements may lead to the problem of negative transfer.

**Contibution**:
Inspired by the success of multitask learning in the NLP area, authors suggest **prepending learnable conditional feature vectors to the query and key of the attention module**, resulting in the PrefixMol method. The prefix embedding is always on the left side, serving as a task-related contextual prompt to affect the predicted outcomes on its right. These prefix embeddings are learned by auxiliary neural networks, considering the 3D pocket and chemical properties.

**Results**:
Experiments show that PrefixMol exhibits good controllability in both single and multi-conditional molecular generation. The controllability enables us to outperform previous structure-based drug design methods. More interestingly, authors open up the attention mechanism and reveal coupling relationships between conditions, providing guidance for multi-conditional molecule generation.
<img width="1058" alt="image" src="https://github.com/IsXudongZhang/Papers-for-structure-based-molecular-generation/assets/105139522/f9e2995d-c7ce-4fb5-93b6-f76023ba725e">

[Go To Top](#top)

<br>

---
### <a id="2."> **ICML 2023** || DECOMPDIFF: Diffusion Models with Decomposed Priors for Structure-Based Drug Design</a>  
**Motivation**:
*  **Why is Diffusion**: Autoregressive models suffer from error accumulation and require a generation order, which is nontrivial for molecular graphs. Diffusion model-based methods can model local and global interactions between atoms simultaneously and achieve better performance than autoregressive models.
*  **Why is decomposed priors**:
    - Existing diffusion model-based approaches neglect bonds in the modeling process, which may lead to unreasonable molecular structures.
    - Moreover, diffusion model-based approaches treat the ligand molecule as a whole and learn the overall correspondence between the target binding site and the ligand. However, atoms within the same ligand can be designed for different functions. Therefore, treating all ligand atoms equally may not be the best way for SBDD, especially considering the tremendous drug-like space to explore and the limited amount of high quality target-ligand complexes  for training.



**Contibution**:
* Authors propose a diffusion model with decomposed priors for structure-based drug design, which incorporates the natural decomposition of a ligand molecule into function-related regions.
* Authors consider both atom and bond diffusion processes in the model to simultaneously generate atoms and bonds for improving drug-likeness and synthesizability.
* Authors design and incorporate several guidance terms in the decomposed generation process to improve the molecular validity.

**Results**:
Extensive experiments on CrossDocked2020 show that DecompDiff achieves SOTA performance in generating high-affinity molecules while maintaining proper molecular properties and conformational stability, with up to −8.39 Avg. Vina Dock score and 24.5% Success Rate. 
<img width="1048" alt="image" src="https://github.com/IsXudongZhang/Papers-for-structure-based-molecular-generation/assets/105139522/aac6c35c-7e20-46e6-bca1-e99c59dde24c">

[Go To Top](#top)

<br>
