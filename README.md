# PAT-ADN
Paper: Unsupervised disentanglement strategy for mitigating artifact in photoacoustic tomography under extremely sparse view      
Authors: Wenhua Zhong, Tianle Li, Shangkun Hou, Hongyu Zhang, Qiegen Liu, Xianlin Song
https://doi.org/10.1016/j.pacs.2024.100613

Date : May-1-2024     
Version : 1.0       
The code and the algorithm are for non-comercial use only.      
Copyright 2024, Department of Electronic Information Engineering, Nanchang University.  

Traditional methods under sparse view for reconstruction of photoacoustic tomography (PAT) often result in significant artifacts. Here, a novel image to image transformation method based on unsupervised learning artifact disentanglement network (ADN), named PAT-ADN, was proposed to address the issue. This network is equipped with specialized encoders and decoders that are responsible for encoding and decoding the artifacts and content components of unpaired images, respectively. The performance of the proposed PAT-ADN was evaluated using circular phantom data and the animal in vivo experimental data. The results demonstrate that PAT-ADN exhibits excellent performance in effectively removing artifacts. In particular, under extremely sparse view (e.g., 16 projections), structural similarity index and peak signal-to-noise ratio are improved by ~200% and ~90% in in vivo experimental data using the proposed method compared to traditional reconstruction methods. PAT-ADN improves the imaging performance of PAT, opening up possibilities for its application in multiple domains.

## Method
<div align="center"><img src="https://github.com/yqx7150/PAT-ADN/blob/main/Figs/Fig2.jpg"> </div>

Fig. 1. Architecture of the proposed PAT-ADN.

## Results on circular phantom data
<div align="center"><img src="https://github.com/yqx7150/PAT-ADN/blob/main/Figs/Fig5.jpg"> </div>

Fig. 2. Comparison of artifact removal capabilities of U-Net, CycleGAN and PAT-ADN in circular phantom under different projections.

## Results on in vivo data
<div align="center"><img src="https://github.com/yqx7150/PAT-ADN/blob/main/Figs/Fig8.jpg"> </div>

Fig. 3. Comparison of artifact removal capabilities of U-Net and PAT-ADN in in vivo data under different projections.

## Other Related Projects

*  Accelerated model-based iterative reconstruction strategy for sparse-view photoacoustic tomography aided by multi-channel autoencoder priors  
[<font size=5>**[Paper]**</font>](https://onlinelibrary.wiley.com/doi/10.1002/jbio.202300281)         [<font size=5>**[Code]**</font>](https://github.com/yqx7150/PAT-MDAE)     

* Sparse-view reconstruction for photoacoustic tomography combining diffusion model with model-based iteration      
[<font size=5>**[Paper]**</font>](https://www.sciencedirect.com/science/article/pii/S2213597923001118)       [<font size=5>**[Code]**</font>](https://github.com/yqx7150/PAT-Diffusion)

* Score-based generative model-assisted information compensation for high-quality limited-view reconstruction in photoacoustic tomography      
[<font size=5>**[Paper]**</font>](https://www.sciencedirect.com/science/article/pii/S2213597924000405)       [<font size=5>**[Code]**</font>](https://github.com/yqx7150/Limited-view-PAT-Diffusion)

* Mean-reverting diffusion model-enhanced acoustic-resolution photoacoustic microscopy for resolution enhancement: Toward optical resolution      
[<font size=5>**[Paper]**</font>](https://doi.org/10.1142/S1793545824500238)       [<font size=5>**[Code]**</font>](https://github.com/yqx7150/https://github.com/yqx7150/PAM-AR2OR)

* Generative model for sparse photoacoustic tomography artifact removal      
[<font size=5>**[Paper]**</font>](https://www.spiedigitallibrary.org/conference-proceedings-of-spie/12745/1274503/Generative-model-for-sparse-photoacoustic-tomography-artifact-removal/10.1117/12.2683128.short?SSO=1)   

* PAT-public-data from NCU [<font size=5>**[Code]**</font>](https://github.com/yqx7150/PAT-public-data)
