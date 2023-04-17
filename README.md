# Motion Diffusion Papers


**Human Motion Diffusion Model**.   
*Guy Tevet, Sigal Raab, Brian Gordon, Yonatan Shafir, Daniel Cohen-Or, Amit H. Bermano.*  
ICLR2023.  
[[website](https://guytevet.github.io/mdm-page/)][[arXiv](https://arxiv.org/abs/2209.14916)][[code](https://github.com/GuyTevet/motion-diffusion-model)]

> tldr; This paper introduces the Motion Diffusion Model (MDM), a generative model for human motion that uses diffusion models and transformer-based techniques. MDM predicts the sample in each diffusion step instead of the noise, making it easier to use established geometric losses on the motion. The model is trained with lightweight resources and achieves state-of-the-art results on benchmarks for text-to-motion and action-to-motion.





**MoFusion: A Framework for Denoising-Diffusion-based Motion Synthesis**  
*Rishabh Dabral, Muhammad Hamza Mughal, Vladislav Golyanik, Christian Theobalt.*  
CVPR2023.

> tldr; MoFusion is a new framework for high-quality conditional human motion synthesis, capable of generating diverse and plausible motions based on various conditioning contexts. The framework utilizes denoising diffusion-based techniques and introduces kinematic losses for motion plausibility within the model. The learned latent space enables interactive motion editing applications, providing crucial abilities for virtual character animation and robotics. The effectiveness of MoFusion is demonstrated through comprehensive quantitative evaluations and a perceptual user study, showing superior results compared to the state of the art on established benchmarks in the literature.
