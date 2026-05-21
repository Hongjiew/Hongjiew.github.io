---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am Hongjie Wang (王泓杰), a Research Scientist at Google DeepMind, working on the efficiency-focused pre-training and post-training of video generative models and world models (e.g., Veo and Genie models). I obtained my Ph.D. degree in the ECE department at Princeton University, supervised by Prof. [Niraj K. Jha](https://scholar.google.com/citations?user=R-z1R84AAAAJ&hl=en&oi=ao). Before that, I received my *B.S. degree with honor* from Peking University (June 2021). You can find more information in my [CV](https://hongjiew.github.io/files/resume.pdf). 

My research focuses on the efficiency of large vision models, including but not limited to: (1) Vision Transformers, (2) Diffusion Models, and (3) Vision-Language Models (Multimodal Understanding and Generation Models). My research aims to make their training and inference more efficient and thus enable scaling them up for better performance. 

## Recent News

- 2025-12: Started to work as a research scientist at Google DeepMind
- 2025-07: Started to work as a research scientist at Meta Superintelligence Labs
- 2025-06: Selected as the Outstanding Reviewer of CVPR 2025
- 2025-02: LinGen is accepted to CVPR 2025!
- 2025-01: Give a talk to Stability AI on LinGen
- 2024-12: Release our latest work LinGen, which provides linear-complexity for video generation
- 2024-05: Start my internship at Meta GenAI MovieGen Team
- 2024-02: Zero-TPrune and AT-EDM are accepted to CVPR 2024!
- 2024-01: Give a talk to Qualcomm on Zero-TPrune [[slides](https://hongjiew.github.io/files/Talk_Qualcomm.pdf)]
- 2023-05: Start my internship at Adobe Research

## Work Experience

- Google DeepMind, Research Scientist, Dec 2025 - present
  - Team: GenMedia
  - Topic: Efficiency-focused training for video generative models and world models
  
- Meta Superintelligence Labs, Research Scientist, July 2025 - Dec 2025
  - Team: Multimedia Generation
  - Topic: VLM-powered text-to-image and image-to-image hybrid pre-training

- Meta GenAI [MovieGen Team](https://ai.meta.com/research/movie-gen/), Research Scientist Intern, May 2024 - Dec 2024 
  - Topic: Minute-Length Text-to-Video Generation with Linear Computational Complexity
  - Mentor: Dr. [Xiaoliang Dai](https://sites.google.com/view/xiaoliangdai) 
- Adobe Research, Research Scientist Intern, May 2023 - March 2024 
  - Topic: Efficient Text-to-Image Diffusion Models
  - Mentor: Dr. [Yuchen Liu](https://lychenyoko.github.io/)
- Stanford University, Research Assistant, June 2020 - Sep 2020 
  - Topic: One-Shot Learning Accelerator
  - Supervisor: Prof. [Priyanka Raina](https://priyanka-raina.github.io/)
- Rice University, Research Assistant, June 2019 - Aug 2019 
  - Topic: Neural Network Training Accelerator
  - Supervisor: Prof. [Yingyan Lin](https://eiclab.scs.gatech.edu/pages/team.html) (now at Georgia Tech)

## Publications and Preprints

- **LinMU: Multimodal Understanding Made Linear** 

  **Hongjie Wang**, Niraj K. Jha

  *Transactions on Machine Learning Research (TMLR)* [[paper](https://openreview.net/pdf?id=6BYdTSNrab)]

  ![LinMU](https://hongjiew.github.io/files/LinMU.png)

  **Highlight:** We propose a Vision-Language Model (VLM) design that **achieves linear complexity** without using any quadratic-complexity modules while maintaining the performance of global-attention-based VLMs. We further develop a **three-stage distillation framework** that transforms pre-trained VLMs to our proposed linear-complexity design at low cost. LinMU matches the performance of teacher models, yet **reduces Time-To-First-Token (TTFT) by up to 2.7x** and **improves token throughput by up to 9.0x** on minute-length videos. 

- **LinGen: Towards High-Resolution Minute-Length Text-to-Video Generation with Linear Computational Complexity**

  **Hongjie Wang**, Chih-Yao Ma, Yen-Cheng Liu, Ji Hou, Tao Xu, Jialiang Wang, Felix Juefei-Xu, Yaqiao Luo, Peizhao Zhang, Tingbo Hou, Peter Vajda, Niraj K. Jha, Xiaoliang Dai

  *IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2025* [[paper](https://arxiv.org/pdf/2412.09856)] [[project](https://lineargen.github.io/)] [[code](https://github.com/jha-lab/LinGen)]

  *Journal Extension (preprint)* [[paper](https://www.researchsquare.com/article/rs-7159495/v1)]

  ![LinGen](https://lineargen.github.io/static/images/overview.png)

  **Highlight:** For the first time, we demonstrate **high-resolution 68-second video generation at 16fps on a single GPU** — without relying on autoregressive extensions, super-resolution, or frame interpolation. Our approach achieves **linear computational complexity**, offering **up to 15x speed-up** over the standard DiT architecture, while delivering **improved video quality and better text alignment**. We believe this linear complexity provides extraordinary scalability, paving the way to hour-length movie generation. 

- **AT-EDM: Attention-Driven Training-Free Efficiency Enhancement of Diffusion Models**

  **Hongjie Wang**, Difan Liu, Yan Kang, Yijun Li, Zhe Lin, Niraj K. Jha, Yuchen Liu

  *IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024* [[paper](https://arxiv.org/abs/2405.05252)] [[project](https://atedm.github.io/)]

  ![AT-EDM](https://hongjiew.github.io/files/ATEDM.png)

  **Highlight:** We introduce the Attention-driven Training-free Efficient Diffusion Model (**AT-EDM**), a framework that leverages attention maps to perform run-time pruning of redundant tokens during inference **without fine-tuning** **or** performing GPU-intensive **optimization** on a certain loss function. AT-EDM reduces the FLOPs of the state-of-the-art open-source diffusion model, [SD-XL](https://github.com/Stability-AI/generative-models), by **40%** while keeping its FID and CLIP scores. 

- **Zero-TPrune: Zero-Shot Token Pruning through Leveraging of the Attention Graph in Pre-Trained Transformers**

  **Hongjie Wang**, Bhishma Dedhia, Niraj K. Jha

  *IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024* [[paper](https://arxiv.org/abs/2305.17328)] [[project](https://zerotprune.github.io/)]

  ![Zero-TPrune](https://hongjiew.github.io/files/zero-tprune.png)

  **Highlight:** We propose Zero-TPrune, the first zero-shot method that considers both the importance and similarity of tokens in performing token pruning. It leverages the attention graph of pre-trained Transformer models to produce an importance distribution for tokens via our proposed Weighted Page Rank (WPR) algorithm. It can be deployed on large Vision Transformers at negligible computational cost. Without any fine-tuning, Zero-TPrune reduces the FLOPs cost of DeiT-S by 34.7% and improves its throughput by 45.3% with only 0.4% accuracy loss.

### Pre-PhD: Software-and-Hardware Co-Design for ML Acceleration

- **SAPIENS: A 64-kb RRAM-Based Non-Volatile Associative Memory for One-Shot Learning and Inference at the Edge**

  Haitong Li, Wei-Chen Chen, Akash Levy, Ching-Hua Wang, **Hongjie Wang**, Po-Han Chen, Weier Wan, Win-San Khwa, Harry Chuang, Y.-D. Chih, Meng-Fan Chang, H.-S. Philip Wong, Priyanka Raina.

  *IEEE Transactions on Electron Devices (2021)* [[paper](https://ieeexplore.ieee.org/abstract/document/9535369)]

  **Highlight:** We present the first chip-level demonstration of one-shot learning with Stanford Associative memory for Programmable, Integrated Edge iNtelligence via life-long learning and Search (SAPIENS), a resistive random access memory (RRAM)-based non-volatile associative memory (AM) chip that serves as the backend for memory-augmented neural networks (MANNs).

- **One-Shot Learning with Memory-Augmented Neural Networks Using a 64-kbit, 118 GOPS/W RRAM-Based Non-Volatile Associative Memory**

  Haitong Li, Wei-Chen Chen, Akash Levy, Ching-Hua Wang, **Hongjie Wang**, Po-Han Chen, Weier Wan, H.-S. Philip Wong, Priyanka Raina

  *IEEE Symposia on VLSI Technology and Circuits (VLSI) 2021* [[paper](https://ieeexplore.ieee.org/abstract/document/9508761)]

  **Highlight:** Using only one example per class for 32 unseen classes during on-chip learning, our AM chip achieves ~72% measured inference accuracy on Omniglot as the first chip accuracy report compared to software accuracy (~82%), while reaching 118 GOPS/W for in-memory L1 distance computation and prediction. 

- **A New MRAM-based Process In-Memory Accelerator for Efficient Neural Network Training with Floating Point Precision**

  **Hongjie Wang**, Yang Zhao, Chaojian Li, Yue Wang, Yingyan Lin

  *IEEE International Symposium on Circuits and Systems (ISCAS) 2020* <span style="color: red;">**(Oral)**</span> [[paper](https://arxiv.org/abs/2003.01551)]

  **Highlight:** We propose a SOT-MRAM based digital Process In-Memory accelerator that supports floating point precision. It can achieve 3.3×, 1.8×, and 2.5× improvement in terms of energy, latency, and area, respectively, compared with a state-of-the-art PIM based DNN training accelerator.

## Academic Service

- Served (or serving) as a reviewer for
  - NeurIPS 2024, 2025, 2026
  - CVPR 2024, 2025, 2026
  - SIGGRAPH Asia 2025
  - ECCV 2024, 2026
  - ICCV 2025
  - BMVC 2026
  - WACV 2026
  - AISTATS 2025, 2026
  - COCOON 2025
  - IEEE Transactions on Image Processing (TIP)
  - International Journal of Computer Vision (IJCV)
  - IEEE Transactions on Neural Networks and Learning Systems (TNNLS)
  - IEEE Internet of Things Journal (IoT-J)
  - IEEE ISCAS 2021

## Selected Awards

- Outstanding Reviewer of CVPR 2026, IEEE/CVF, 2026
- Outstanding Reviewer of CVPR 2025, IEEE/CVF, 2025
- Fellowship in Natural Science and Engineering, Princeton University, 2021
- Excellent Graduate, Peking University, 2021
- Xiaomi Scholarship, Peking University, 2020
- National Scholarship, Peking University, 2019
- May 4th Scholarship, Peking University, 2018
- Student of Merits, Peking University, 2017-2021
- Gold Medal in 33rd Chinese Physics Olympiad, 2016
