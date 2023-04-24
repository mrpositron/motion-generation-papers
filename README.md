# Awesome Motion Generation Papers

Last updated on: 18.04.2023

### Modeling motion with ...
1. [Variational Auto Encoders (VAEs)](#vaes)   
    - [T2M-GPT: Generating Human Motion from Textual Descriptions with Discrete Representations](#t2m-gpt-generating-human-motion-from-textual-descriptions-with-discrete-representations)
    - [Generating Diverse and Natural 3D Human Motions from Text](#generating-diverse-and-natural-3d-human-motions-from-text )
    
2. [Diffusion Processes](#diffusion-processes)

<!-- [[website]()][[arXiv]()][[code]()][[video]()] -->
<!-- date -->

## VAEs

### T2M-GPT: Generating Human Motion from Textual Descriptions with Discrete Representations
*Jianrong Zhang, Yangsong Zhang, Xiaodong Cun, Shaoli Huang, Yong Zhang, Hongwei Zhao, Hongtao Lu, Xi Shen*   
Venue: CVPR2023   
[[website](https://mael-zys.github.io/T2M-GPT/)][[arXiv](https://arxiv.org/abs/2301.06052)][[code](https://github.com/Mael-zys/T2M-GPT)][no video]   
<!-- 15 Jan 2023 -->  

<details>
<summary><b> tldr </b></summary>

> In this work, the authors use a combination of Vector Quantised-Variational AutoEncoder (VQ-VAE) and Generative Pre-trained Transformer (GPT) for generating human motion from text descriptions. They find that a simple CNN-based VQ-VAE with commonly used training techniques produces high-quality representations, and incorporating a corruption strategy during GPT training improves performance. Their proposed approach, T2M-GPT, outperforms recent diffusion-based approaches on a large dataset, HumanML3D, with better consistency between text and generated motion and lower FID score. However, the authors note that the dataset size is a limitation of their approach, and suggest that VQ-VAE remains a competitive approach for human motion generation.
</details>


---
### Generating Diverse and Natural 3D Human Motions from Text
*Chuan Guo, Shihao Zou, Xinxin Zuo, Sen Wang, Wei Ji, Xingyu Li, Li Cheng*      
Venue: CVPR2022   
[[website](https://ericguo5513.github.io/text-to-motion/)][[thecvf](https://openaccess.thecvf.com/content/CVPR2022/papers/Guo_Generating_Diverse_and_Natural_3D_Human_Motions_From_Text_CVPR_2022_paper.pdf)][[code](https://github.com/EricGuo5513/text-to-motion)][[video](https://youtu.be/085mBtMeZpg)]


> **tldr;** This paper proposes a two-stage approach to address the challenging problem of generating diverse and accurate 3D human motions from text. The first stage involves sampling motion lengths from a learned distribution function conditioned on input text, while the second stage uses a temporal variational autoencoder to synthesize a diverse set of human motions of the sampled lengths using motion snippet code as an internal motion representation.

---
### TEMOS: Generating diverse human motions from textual descriptions   
*Mathis Petrovich, Michael J. Black, Gül Varol*  
Venue: ECCV2022   
[[website](https://mathis.petrovich.fr/temos/)][[arXiv](https://arxiv.org/abs/2204.14109)][[code](https://github.com/Mathux/TEMOS)][[video](https://youtu.be/07dQiKK17aQ)]   
<!-- 25 Apr 2022 --> 

> **tldr;** The paper presents TEMOS, a text-conditioned generative model that addresses the problem of generating diverse 3D human motions from textual descriptions. Unlike previous work that focuses on generating a single, deterministic motion, TEMOS uses a variational approach that produces multiple diverse human motions. The model leverages variational autoencoder training with human motion data and a text encoder that produces distribution parameters compatible with the VAE latent space. The framework can produce skeleton-based animations as well as more expressive SMPL body motions and achieves significant improvements over the state of the art on the KIT Motion-Language benchmark.

---
## Diffusion Processes

### Single Motion Diffusion   
*Sigal Raab, Inbal Leibovitch, Guy Tevet, Moab Arar, Amit H. Bermano, and Daniel Cohen-Or*  
Venue: arXiv preprint.   
[[website](https://sinmdm.github.io/SinMDM-page/)][[arXiv](https://arxiv.org/abs/2302.05905)][[code](https://github.com/SinMDM/SinMDM)][[video](https://youtu.be/dU9WR8rWAJI)]

<!-- 12 Feb 2023 -->

> **tldr;** This work presents Single Motion Diffusion Model that learns internal motifs of a single motion sequence and generates motions of arbitrary length that are faithful to them. The model harnesses the power of diffusion models and includes a denoising network designed specifically for learning from a single input motion. The transformer-based architecture avoids overfitting and encourages motion diversity. SinMDM can be applied in various contexts, including spatial and temporal in-betweening, motion expansion, style transfer, and crowd animation. Results show that SinMDM outperforms existing methods in quality and time-space efficiency and facilitates applications at inference time without additional training.

---
### Executing your Commands via Motion Diffusion in Latent Space
*Xin Chen, Biao Jiang, Wen Liu, Zilong Huang, Bin Fu, Tao Chen, Jingyi Yu, Gang Yu*   
Venue: CVPR2023   
[[website](https://chenxin.tech/mld/)][[arXiv](https://arxiv.org/abs/2212.04048)][[code](https://github.com/ChenFengYe/motion-latent-diffusion)][no video]    
> **tldr;**  The authors tackle the challenging task of conditional human motion generation, where they generate plausible human motion sequences based on conditional inputs like action classes or textual descriptors. They propose a Motion Latent-based Diffusion (MLD) model that uses a Variational AutoEncoder (VAE) to learn a low-dimensional latent code for human motion sequences, and then performs diffusion on the motion latent space to establish connections with conditional inputs. This approach reduces computational overhead and produces vivid motion sequences that outperform state-of-the-art methods on various human motion generation tasks, while being significantly faster than previous diffusion models on raw motion sequences.
   
---


### MoFusion: A Framework for Denoising-Diffusion-based Motion Synthesis
*Rishabh Dabral, Muhammad Hamza Mughal, Vladislav Golyanik, Christian Theobalt.*  
Venue: CVPR2023.  
[[website](https://vcai.mpi-inf.mpg.de/projects/MoFusion/)][[arXiv](https://arxiv.org/abs/2212.04495)][no code][[video](https://youtu.be/DLoB0Xmj84Y)]   


<!-- 8 Dec 2022 -->


> **tldr;** MoFusion is a new framework for high-quality conditional human motion synthesis that can generate long, semantically accurate motions based on a range of conditioning contexts, such as music and text. It introduces a denoising-diffusion-based method that allows for well-known kinematic losses for motion plausibility. The learned latent space can be used for interactive motion editing applications and is demonstrated to be more effective than the state-of-the-art on established benchmarks in the literature.

---


### Human Motion Diffusion Model
*Guy Tevet, Sigal Raab, Brian Gordon, Yonatan Shafir, Daniel Cohen-Or, Amit H. Bermano.*  
Venue: ICLR2023.  
[[website](https://guytevet.github.io/mdm-page/)][[arXiv](https://arxiv.org/abs/2209.14916)][[code](https://github.com/GuyTevet/motion-diffusion-model)][[video](https://youtu.be/rVkIDj5wgjs)]  

<!-- 29 Sep 2022 -->


> **tldr;** This paper introduces the Motion Diffusion Model (MDM), a generative model for human motion that uses diffusion models and transformer-based techniques. MDM predicts the sample in each diffusion step instead of the noise, making it easier to use established geometric losses on the motion. The model is trained with lightweight resources and achieves state-of-the-art results on benchmarks for text-to-motion and action-to-motion.

---

### FLAME: Free-form Language-based Motion Synthesis & Editing
*Jihoon Kim, Jiseob Kim, Sungjoon Choi*   
Venue: AAAI2023.    

[[website](https://kakaobrain.github.io/flame/)][[arXiv](https://arxiv.org/abs/2209.00349)][[code](https://github.com/kakaobrain/flame)][[video](https://youtu.be/LbPNGv0zrto)]
<!-- 1 Sep 2022 -->   
> **tldr**; The paper proposes a text-based motion synthesis and editing model named FLAME that integrates diffusion-based generative models into the motion domain. FLAME can generate high-fidelity motions well aligned with given text and edit motion parts without fine-tuning. It uses a transformer-based architecture to better handle motion data, manage variable-length motions, and attend well to free-form text. FLAME achieves state-of-the-art generation performances on three text-motion datasets and editing capability can be extended to other tasks such as motion prediction or motion in-betweening.
---

### MotionDiffuse: Text-Driven Human Motion Generation with Diffusion Model
*Mingyuan Zhang, Zhongang Cai, Liang Pan, Fangzhou Hong, Xinying Guo, Lei Yang, Ziwei Liu*   
Venue: arXiv preprint.   
[[website](https://mingyuan-zhang.github.io/projects/MotionDiffuse.html)][[arXiv](https://arxiv.org/abs/2208.15001)][[code](https://github.com/mingyuan-zhang/MotionDiffuse)][[video](https://youtu.be/U5PTnw490SA)]  
<!-- 31 Aug 2022 -->

> **tldr**; MotionDiffuse is a text-driven motion generation framework that uses probabilistic mapping and a diffusion model to generate diverse and fine-grained human motions from various text inputs. It excels at modeling complicated data distributions and responds to fine-grained instructions on body parts, allowing for arbitrary-length motion synthesis with time-varied text prompts. MotionDiffuse outperforms existing state-of-the-art methods on text-driven motion generation and action-conditioned motion generation, and it is controllable for comprehensive motion generation.
