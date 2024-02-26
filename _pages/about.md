---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am Hongjie Wang (王泓杰), a third-year Ph.D. candidate in the [Department of Electrical and Computer Engineering](https://ece.princeton.edu/) at Princeton University, supervised by Prof. [Niraj K. Jha](https://scholar.google.com/citations?user=R-z1R84AAAAJ&hl=en&oi=ao). Before that, I received my *B.S. degree with honor* from Peking University (June 2021). Mentored by Dr. [Yuchen Liu](https://lychenyoko.github.io/), I worked as a research scientist intern at [Adobe Research](https://research.adobe.com/). I also worked with Prof. [Yingyan Lin](https://eiclab.scs.gatech.edu/pages/team.html) and Prof. [Priyanka Raina](https://priyanka-raina.github.io/) as a research intern at Rice University and Stanford University, respectively. You can find more information in my [CV](https://hongjiew.github.io/files/resume.pdf). 

My research focuses on the efficiency of Machine Learning models, including but not limited to: (1) Vision Transformers, (2) Diffusion Models, (3) Vision-Language Models (Multimodal Generative Models), and (4) State Space Models. My research aims to make their training and inference more efficient and thus enable scaling them up for generation with higher quality. My recent projects focus on the hardware-agnostic efficiency enhancement of them, but I am also interested in the software-hardware co-design to boost their throughputs.

Please feel free to reach out via hongjiewang@princeton.edu if you share interests similar to mine! I am glad to chat and explore opportunities for collaboration.

## Recent News

- 2024-02: Zero-TPrune and AT-EDM are accepted to CVPR 2024!
- 2024-01: Give a Talk to Qualcomm on Zero-TPrune [[slides](https://hongjiew.github.io/files/Talk_Qualcomm.pdf)]

## Publications and Preprints

- AT-EDM: Attention-Driven Training-Free Efficiency Enhancement of Diffusion Models

  **Hongjie Wang**, Difan Liu, Yan Kang, Yijun Li, Zhe Lin, Niraj K. Jha, Yuchen Liu

  ![AT-EDM](https://hongjiew.github.io/files/ATEDM.png)

  **Highlight:** We introduce the Attention-driven Training-free Efficient Diffusion Model (**AT-EDM**), a framework that leverages attention maps to perform run-time pruning of redundant tokens during inference **without fine-tuning** **or** performing GPU-intensive **optimization** on a certain loss function. AT-EDM reduces the FLOPs of the state-of-the-art open-source diffusion model, [SD-XL](https://github.com/Stability-AI/generative-models), by **40%** while keeping its FID and CLIP scores. 

  [[project webpage](https://atedm.github.io/)] The *arXiv* link is coming soon

- Zero-TPrune: Zero-Shot Token Pruning through Leveraging of the Attention Graph in Pre-Trained Transformers

  **Hongjie Wang**, Bhishma Dedhia, Niraj K. Jha

  ![Zero-TPrune](https://hongjiew.github.io/files/zero-tprune.png)

  **Highlight:** We propose Zero-TPrune, the first zero-shot method that considers both the importance and similarity of tokens in performing token pruning. It leverages the attention graph of pre-trained Transformer models to produce an importance distribution for tokens via our proposed Weighted Page Rank (WPR) algorithm. It can be deployed on large Vision Transformers at negligible computational cost. Without any fine-tuning, Zero-TPrune reduces the FLOPs cost of DeiT-S by 34.7% and improves its throughput by 45.3% with only 0.4% accuracy loss.

  *arXiv*:2305.17328 [[paper](https://arxiv.org/abs/2305.17328)] [[project webpage](https://zerotprune.github.io/)]

- SAPIENS: A 64-kb RRAM-Based Non-Volatile Associative Memory for One-Shot Learning and Inference at the Edge

  Haitong Li, Wei-Chen Chen, Akash Levy, Ching-Hua Wang, **Hongjie Wang**, Po-Han Chen, Weier Wan, Win-San Khwa, Harry Chuang, Y.-D. Chih, Meng-Fan Chang, H.-S. Philip Wong, Priyanka Raina.

  ![SAPIENS](https://hongjiew.github.io/files/SAPIENS.png)

  **Highlight:** We present the first chip-level demonstration of one-shot learning with Stanford Associative memory for Programmable, Integrated Edge iNtelligence via life-long learning and Search (SAPIENS), a resistive random access memory (RRAM)-based non-volatile associative memory (AM) chip that serves as the backend for memory-augmented neural networks (MANNs).

  *IEEE Transactions on Electron Devices (2021)* [[paper](https://ieeexplore.ieee.org/abstract/document/9535369)]

- One-Shot Learning with Memory-Augmented Neural Networks Using a 64-kbit, 118 GOPS/W RRAM-Based Non-Volatile Associative Memory

  Haitong Li, Wei-Chen Chen, Akash Levy, Ching-Hua Wang, **Hongjie Wang**, Po-Han Chen, Weier Wan, H.-S. Philip Wong, Priyanka Raina

  <img src="https://hongjiew.github.io/files/one-shot.png" alt="one-shot" width="70%">

  **Highlight:** Using only one example per class for 32 unseen classes during on-chip learning, our AM chip achieves ~72% measured inference accuracy on Omniglot as the first chip accuracy report compared to software accuracy (~82%), while reaching 118 GOPS/W for in-memory L1 distance computation and prediction. 

  *IEEE Symposia on VLSI Technology and Circuits (VLSI) 2021* [[paper](https://ieeexplore.ieee.org/abstract/document/9508761)]

- A New MRAM-based Process In-Memory Accelerator for Efficient Neural Network Training with Floating Point Precision

  **Hongjie Wang**, Yang Zhao, Chaojian Li, Yue Wang, Yingyan Lin

  <img src="https://hongjiew.github.io/files/SOT-MRAM.png" alt="one-shot" width="70%">
  
  **Highlight:** We propose a SOT-MRAM based digital Process In-Memory accelerator that supports floating point precision. It can achieve 3.3×, 1.8×, and 2.5× improvement in terms of energy, latency, and area, respectively, compared with a state-of-the-art PIM based DNN training accelerator.
  
  *IEEE International Symposium on Circuits and Systems (ISCAS) 2020* <span style="color: red;">**(Oral)**</span> [[paper](https://arxiv.org/abs/2003.01551)]

## Academic Service

- Served as a reviewer for
  - IEEE Internet of Things Journal
  - IEEE ISCAS 2021

## Work Experience

- Adobe Research, research scientist intern, May 2023 - present
- Stanford University, research intern, June 2020 - Sep 2020
- Rice University, research intern, June 2019 - Aug 2019

## Selected Awards

- Fellowship in Natural Science and Engineering, Princeton University, 2021
- Excellent Graduate, Peking University, 2021
- Xiaomi Scholarship, Peking University, 2020
- National Scholarship, Peking University, 2019
- May 4th Scholarship, Peking University, 2018
- Student of Merits, Peking University, 2017-2021
- Gold Medal in 33rd Chinese Physics Olympiad, 2016



