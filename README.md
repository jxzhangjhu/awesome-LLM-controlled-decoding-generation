# Awesome-LLM-Controlled-Decoding-Generation
<!-- Awesome-LLM-controlled-constrained-generation -->

\
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/hee9joon/Awesome-Diffusion-Models) 
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Made With Love](https://img.shields.io/badge/Made%20With-Love-red.svg)](https://github.com/chetanraj/awesome-github-badges)



This repo aims to record advanced papers of controllable and decoding generation in LLMs.

We strongly encourage the researchers who want to promote their fantastic work in this area to make pull requests to update their paper's information!


## Contents

- [Review](#review)
- [Papers](#papers)
  - [Decoding-time Alignment](#decoding-time-alignment)
  - [Controlled Decoding](#controlled-decoding)
  - [Tractable Probabilistic Models](#tractable-probabilistic-models)
  - [Instruction Tuning](#instruction-tuning)
  - [Non-autoregressive Language Model](#Non-autoregressive-Language-Model)
  - [NeuroLogic Decoding](#NeuroLogic-Decoding)
  - [Evaluation and Understanding](#Evaluation-and-Understanding)
  - [Application](#application)


--- 

# Review & Survey 

- **Controllable Neural Text Generation** \
*Lilian Weng* \
Lil'Log, 2021. [[Link]](https://lilianweng.github.io/posts/2021-01-02-controllable-text-generation/)

- **A Survey of Controllable Text Generation using Transformer-based Pre-trained Language Models** \
*Hanqing Zhang, Haolin Song, Shaoyu Li, Ming Zhou, Dawei Song* \
ACM Computing Surveys, 2023. [[Paper]](https://arxiv.org/abs/2201.05337)

- **From Decoding to Meta-Generation: Inference-time Algorithms for Large Language Models** \
*Sean Welleck, Amanda Bertsch, Matthew Finlayson, Hailey Schoelkopf, Alex Xie, Graham Neubig, Ilia Kulikov, Zaid Harchaoui* \
arXiv 2024. [[Paper]](https://arxiv.org/abs/2406.16838)


# Benchmark 

- **Controllable Text Generation with Language Constraints** \
*Howard Chen, Huihan Li, Danqi Chen, Karthik Narasimhan* \
arXiv 2022. [[Paper]](https://arxiv.org/abs/2212.10466) [[Github]](https://github.com/princeton-nlp/Cognac) 

# Technical Report

- **LLM Critics Help Catch LLM Bugs** \
*Nat McAleese, Rai Michael Pokorny, Juan Felipe Ceron Uribe, Evgenia Nitishinskaya, Maja Trebacz, Jan Leike* \
Jun 28, 2024. OpenAI. [[Paper]](https://arxiv.org/pdf/2407.00215) [[Link]](https://openai.com/index/finding-gpt4s-mistakes-with-gpt-4/?utm_source=www.dailyzaps.com&utm_medium=newsletter&utm_campaign=criticgpt-fixing-ai-with-ai)


# Papers

## Decoding-time Alignment

- **Decoding-time Realignment of Language Models** \
*Tianlin Liu, Shangmin Guo, Leonardo Bianco, Daniele Calandriello, Quentin Berthet, Felipe Llinares, Jessica Hoffmann, Lucas Dixon, Michal Valko, Mathieu Blondel* \
ICML 2024. [[Paper]](https://arxiv.org/abs/2402.02992) 
<!-- [[Github]] -->

- **DeAL: Decoding-time Alignment for Large Language Models** \
*James Y. Huang, Sailik Sengupta, Daniele Bonadiman, Yi-an Lai, Arshit Gupta, Nikolaos Pappas, Saab Mansour, Katrin Kirchhoff, Dan Roth* \
arXiv 2024. [[Paper]](https://arxiv.org/abs/2402.06147)

- **Decoding-Time Language Model Alignment with Multiple Objectives** \
*Ruizhe Shi, Yifang Chen, Yushi Hu, Alisa Liu, Hannaneh Hajishirzi, Noah A. Smith, Simon Du* \
arXiv 2024. [[Paper]](https://arxiv.org/abs/2406.18853) [[Github]](https://github.com/srzer/mod) 

- **Cascade Reward Sampling for Efficient Decoding-Time Alignment** \
*Bolian Li, Yifan Wang, Ananth Grama, Ruqi Zhang* \
arXiv 2024. [[Paper]](https://arxiv.org/abs/2406.16306) [[Github]](https://github.com/lblaoke/CARDS)

- **Reward Steering with Evolutionary Heuristics for Decoding-time Alignment** \
*Anonymous ACL submission* \
arXiv 2024. [[Paper]](https://openreview.net/pdf?id=lBPk1LEq0b)

<!-- Added papers discussed to mitigate hallucination during the inference, by leveraging data-free representation editing or decoding -->

- **DOLA: DECODING BY CONTRASTING LAYERS IMPROVES FACTUALITY IN LARGE LANGUAGE MODELS**\
*Yung-Sung Chuang, Yujia Xie, Hongyin Luo, Yoon Kim, James Glass, Pengcheng He*\
ICLR 2024. [[Paper]](https://arxiv.org/abs/2309.03883) [[Github]](https://github.com/voidism/DoLa)
 
- **Inference-Time Intervention: Eliciting Truthful Answers from a Language Model** \
*Kenneth Li, Oam Patel, Fernanda Viégas, Hanspeter Pfister, Martin Wattenberg* \
NeurIPS 2023. [[Paper]](https://arxiv.org/abs/2306.03341) [[Github]](https://github.com/likenneth/honest_llama) 
<!-- hallucination -->

 
- **TruthX: Alleviating Hallucinations by Editing Large Language Models in Truthful Space** \
*Shaolei Zhang, Tian Yu, Yang Feng* \
ACL 2024. [[Paper]](https://arxiv.org/pdf/2402.17811v2) [[Github]](https://ictnlp.github.io/TruthX-site/) 
<!-- Following up work of ITI and currently the SOTA on TruthfulQA as of July 2024 -->

- **Truth Forest: Toward Multi-Scale Truthfulness in Large Language Models through Intervention without Tuning** \
*Zhongzhi Chen, Xingwu Sun, Xianfeng Jiao, Fengzong Lian, Zhanhui Kang, Di Wang, Cheng-Zhong Xu* \
AAAI 2024. [[Paper]](https://arxiv.org/abs/2312.17484) [[Github]](https://github.com/jongjyh/TrFr) 
<!-- Related work following ITI, earlier than TruthX -->



- **Lookback Lens: Detecting and Mitigating Contextual Hallucinations in Large Language Models Using Only Attention Maps** \
*Yung-Sung Chuang, Linlu Qiu, Cheng-Yu Hsieh, Ranjay Krishna, Yoon Kim, James Glass* \
Arxiv 2024. [[Paper]](https://arxiv.org/abs/2407.07071) [[Github]](https://github.com/voidism/Lookback-Lens)
<!-- Targetting on contextual hallucination -->


- **Trusting Your Evidence: Hallucinate Less with Context-aware Decoding**\
*Weijia Shi, Xiaochuang Han, Mike Lewis, Yulia Tsvetkov, Luke Zettlemoyer, Scott Wen-tau Yih*\
NAACL 2024. [[Paper]](https://arxiv.org/pdf/2305.14739) [[Github]](https://github.com/hongshi97/CAD)

- **Mutual Information Alleviates Hallucinations in Abstractive Summarization**\
*Liam van der Poel, Ryan Cotterell, Clara Meister*\
EMNLP 2022. [[Paper]](https://arxiv.org/pdf/2210.13210) [[Github]](https://github.com/VanderpoelLiam/CPMI)

- **Locating and Editing Factual Associations in GPT**\
*Kevin Meng, David Bau, Alex Andonian, Yonatan Belinkov*\
NeurIPS 2022. [[Paper]](https://arxiv.org/abs/2202.05262) [[Website]](https://rome.baulab.info/)



## Controlled Decoding


- **Aligning Large Language Models with Representation Editing: A Control Perspective**\
*Lingkai Kong, Haorui Wang, Wenhao Mu, Yuanqi Du, Yuchen Zhuang, Yifei Zhou, Yue Song, Rongzhi Zhang, Kai Wang, Chao Zhang*\
Arxiv 2024. [[Paper]](https://arxiv.org/pdf/2406.05954) 
<!-- 11 June 2024 -->


- **PaCE: Parsimonious Concept Engineering for Large Language Models** \
*Jinqi Luo, Tianjiao Ding, Kwan Ho Ryan Chan, Darshan Thaker, Aditya Chattopadhyay, Chris Callison-Burch, René Vidal* \
arXiv 2024. [[Paper]](https://arxiv.org/abs/2406.04331) [[Github]](https://github.com/peterljq/parsimonious-concept-engineering) 


- **Controlled Decoding from Language Models**\
*Sidharth Mudgal, Jong Lee, Harish Ganapathy, YaGuang Li, Tao Wang, Yanping Huang, Zhifeng Chen, Heng-Tze Cheng, Michael Collins, Trevor Strohman, Jilin Chen, Alex Beutel, Ahmad Beirami*\
ICML 2024. [[Paper]](https://arxiv.org/pdf/2310.17022) 
<!-- 3 June 2024 -->

- **Weak-to-Strong Search: Align Large Language Models via Searching over Small Language Models** \
*Zhanhui Zhou, Zhixuan Liu, Jie Liu, Zhichen Dong, Chao Yang, Yu Qiao* \
arXiv 2024 [[Paper]](https://arxiv.org/abs/2405.19262) [[Github]](https://github.com/zhziszz/weak-to-strong-search)
<!-- 29 May 2024  -->
<!-- greedy search and test-time alignment -->

- **BWArea Model: Learning World Model, Inverse Dynamics, and Policy for Controllable Language Generation**\
*Chengxing Jia, Pengyuan Wang, Ziniu Li, Yi-Chen Li, Zhilong Zhang, Nan Tang, Yang Yu*\
Arxiv 2024. [[Paper]](https://arxiv.org/pdf/2405.17039)
<!-- 27 May 2024 -->

- **COLD-Attack: Jailbreaking LLMs with Stealthiness and Controllability** \
*Xingang Guo, Fangxu Yu, Huan Zhang, Lianhui Qin, Bin Hu* \
ICML 2024. [[Paper]](https://arxiv.org/abs/2402.08679) [[Github]](https://github.com/yu-fangxu/cold-attack) 
<!-- 13 Feb 2024  -->

- **Controlled Text Generation for Large Language Model with Dynamic Attribute Graphs** \
*Xun Liang, Hanyu Wang, Shichao Song, Mengting Hu, Xunzhi Wang, Zhiyu Li, Feiyu Xiong, Bo Tang* \
ACL 2024. [[Ppaer]](https://arxiv.org/abs/2402.11218) [[Github]](https://github.com/iaar-shanghai/datg)

- **Controlled Text Generation via Language Model Arithmetic** \
*Jasper Dekoninck, Marc Fischer, Luca Beurer-Kellner, Martin Vechev* \
ICLR 2024. [[Paper]](https://arxiv.org/abs/2311.14479) [[Github]](https://github.com/eth-sri/language-model-arithmetic)


- **Guiding LLMs The Right Way: Fast, Non-Invasive Constrained Generation** \
*Luca Beurer-Kellner, Marc Fischer, Martin Vechev* \
arXiv 2024. [[Paper]](https://arxiv.org/abs/2403.06988) 
<!-- similar as the above one from same time in ETH -->

- **Controllable Text Generation with Neurally-Decomposed Oracle** \
*Tao Meng, Sidi Lu, Nanyun Peng, Kai-Wei Chang* \
NeurIPS 2022. [[Paper]](https://arxiv.org/abs/2205.14219) [[Github]](https://github.com/mtsomethree/constrdecoding)

- **BOLT: Fast Energy-based Controlled Text Generation with Tunable Biases** \
*Xin Liu, Muhammad Khalifa, Lu Wang* \
ACL 2023. [[Paper]](https://arxiv.org/abs/2305.12018) [[Github]](https://github.com/launchnlp/bolt) 

- **Controllable Text Generation with Neurally-Decomposed Oracle** \
*Xin Liu, Muhammad Khalifa, Lu Wang* \
NeurIPS 2022. [[Paper]](https://arxiv.org/abs/2305.12018) [[Github]](https://github.com/launchnlp/bolt) 


- **COLD Decoding: Energy-based Constrained Text Generation with Langevin Dynamics**\
*Lianhui Qin, Sean Welleck, Daniel Khashabi, Yejin Choi*\
NeurIPS 2022 [[Paper]](https://arxiv.org/pdf/2202.11705) [[Github]](https://github.com/qkaren/COLD_decoding) 
<!-- 13 Oct 2022 -->

- **Gradient-Based Constrained Sampling from Language Models** \
*Sachin Kumar, Biswajit Paria, Yulia Tsvetkov* \
EMNLP 2022. [[Paper]](https://arxiv.org/abs/2205.12558) [[Github]](https://github.com/Sachin19/mucoco/tree/sampling)


- **FUDGE: Controlled Text Generation With Future Discriminators**\
*Kevin Yang, Dan Klein*\
NAACL 2021 [[Paper]](https://arxiv.org/pdf/2202.11705) [[Github]](https://github.com/yangkevin2/naacl-2021-fudge-controlled-generation) 
<!-- 15 Aug 2021 -->

- **A Distributional Approach to Controlled Text Generation** \
*Muhammad Khalifa, Hady Elsahar, Marc Dymetman* \
ICLR 2021. [[Paper]](https://arxiv.org/abs/2012.11635) [[Github]](https://github.com/naver/gdc) 

- **Plug and Play Language Models: A Simple Approach to Controlled Text Generation**\
*Sumanth Dathathri, Andrea Madotto, Janice Lan, Jane Hung, Eric Frank, Piero Molino, Jason Yosinski, Rosanne Liu*\
ICLR 2020 [[Paper]](https://arxiv.org/pdf/1912.02164) [[Github]](https://github.com/uber-research/PPLM) 
<!-- 3 Mar 2020 -->

- **Controlled Text Generation as Continuous Optimization with Multiple Constraints** \
*Sachin Kumar, Eric Malmi, Aliaksei Severyn, Yulia Tsvetkov* \
NeurIPS 2020. [[Paper]](https://arxiv.org/abs/2108.01850) [[Github]](https://github.com/Sachin19/mucoco)
<!-- MUCOCO -->

## Tractable Probabilistic Models

- **Tractable Control for Autoregressive Language Generation**\
*Honghua Zhang, Meihua Dang, Nanyun Peng, Guy Van den Broeck*\
ICML 2023 [[Paper]](https://arxiv.org/pdf/2304.07438) [[Github]](https://github.com/UCLA-StarAI/GeLaTo) 
<!-- 15 Nov 2023 -->

## Multi-aspect Controllabled Text Generation

- **An Extensible Plug-and-Play Method for Multi-Aspect Controllable Text Generation**
- *Xuancheng Huang, Zijun Liu, Peng Li, Tao Li, Maosong Sun, Yang Liu* \
ACL 2023. [[Paper]](https://arxiv.org/abs/2212.09387) [[Github]](https://github.com/thunlp-mt/promptgating4mctg)

- **A Distributional Lens for Multi-Aspect Controllable Text Generation** \
*Yuxuan Gu, Xiaocheng Feng, Sicheng Ma, Lingyuan Zhang, Heng Gong, Bing Qin* \
EMNLP 2022. [[Paper]](https://arxiv.org/abs/2210.02889) [[Github]](https://github.com/happygu0524/multicontrol)

## Hallucination Mitigation

<!-- ## Papers focusing on the hallucination mitigation. Methods unlimited: Prompt optimization, Alignment, Controlled Decoding, Representation Editing -->

- **Teaching Language Models to Hallucinate Less with Synthetic Tasks** \
*Erik Jones, Hamid Palangi, Clarisse Simões, Varun Chandrasekaran, Subhabrata Mukherjee, Arindam Mitra, Ahmed Awadallah, Ece Kamar* \
ICLR 2024. [[Paper]](https://arxiv.org/abs/2310.06827)

- **Knowledge Overshadowing Causes Amalgamated Hallucination in Large Language Models** \
*Yuji Zhang, Sha Li, Jiateng Liu, Pengfei Yu, Yi R. Fung, Jing Li, Manling Li, Heng Ji* \
arXiv 2024. [[Paper]](https://arxiv.org/abs/2407.08039) 



<!-- ## Conditional Language Models -->

## Reinforcement Learning

- **Critic-Guided Decoding for Controlled Text Generation** \
*Minbeom Kim, Hwanhee Lee, Kang Min Yoo, Joonsuk Park, Hwaran Lee, Kyomin Jung* \
ACL 2023. [[Paper]](https://arxiv.org/abs/2212.10938) [[Github]](https://github.com/minbeomkim/CriticControl)


## Instruction Tuning 

- **COLLIE: Systematic Construction of Constrained Text Generation Tasks** \
*Shunyu Yao, Howard Chen, Austin W. Hanjie, Runzhe Yang, Karthik Narasimhan* \
ICLR 2024. [[Paper]](https://arxiv.org/abs/2307.08689) [[Github]](https://github.com/princeton-nlp/Collie)

- **Controlled Text Generation with Natural Language Instructions** \
*Wangchunshu Zhou, Yuchen Eleanor Jiang, Ethan Wilcox, Ryan Cotterell, Mrinmaya Sachan* \
ICML 2023. [[Paper]](https://arxiv.org/abs/2304.14293) [[Github]](https://github.com/michaelzhouwang/instructctg) 

- **Toward Unified Controllable Text Generation via Regular Expression Instruction** \
*Xin Zheng, Hongyu Lin, Xianpei Han, Le Sun* \
IJCNLP-AACL 2023. [[Paper]](https://arxiv.org/abs/2309.10447) [[Github]](https://github.com/mrzhengxin/ctg-regex-instruction) 


## Non-autoregressive Language Model

- **Xiang Lisa Li, John Thickstun, Ishaan Gulrajani, Percy Liang, Tatsunori B. Hashimoto** \
*Diffusion-LM Improves Controllable Text Generation* \
NeurIPS 2022. [[Paper]](https://arxiv.org/abs/2205.14217) [[Github]](https://github.com/xiangli1999/diffusion-lm) 




## NeuroLogic Decoding 


- **NeuroComparatives: Neuro-Symbolic Distillation of Comparative Knowledge** \
*Phillip Howard, Junlin Wang, Vasudev Lal, Gadi Singer, Yejin Choi, Swabha Swayamdipta* \
NACCL 2024. [[Paper]](https://arxiv.org/abs/2305.04978) [[Github]](https://github.com/intellabs/multimodal_cognitive_ai)

- **NeuroLogic Decoding: (Un)supervised Neural Text Generation with Predicate Logic Constraints** \
*Ximing Lu, Peter West, Rowan Zellers, Ronan Le Bras, Chandra Bhagavatula, Yejin Choi* \
NAACL 2021. [[Paper]](https://arxiv.org/abs/2010.12884) [[Github]](https://github.com/GXimingLu/neurologic_decoding)





## Evaluation and Understanding 

- **"We Need Structured Output": Towards User-centered Constraints on Large Language Model Output** \
*Michael Xieyang Liu, Frederick Liu, Alexander J. Fiannaca, Terry Koo, Lucas Dixon, Michael Terry, Carrie J. Cai* \
CHI EA 2024. [[Paper]](https://arxiv.org/abs/2404.07362)
<!-- 10 Apr 2024  -->

- **Evaluating, Understanding, and Improving Constrained Text Generation for Large Language Models** \
*Xiang Chen, Xiaojun Wan* \
Arxiv 2023. [[Paper]](https://arxiv.org/abs/2310.16343)
<!-- 25 Oct 2023  -->

- **Evaluating Large Language Models on Controlled Generation Tasks** \
*Jiao Sun, Yufei Tian, Wangchunshu Zhou, Nan Xu, Qian Hu, Rahul Gupta, John Frederick Wieting, Nanyun Peng, Xuezhe Ma* \
EMNLP 2023. [[Paper]](https://arxiv.org/abs/2310.14542) [[Github]](https://github.com/sunjiao123sun/llm-controlgen) 


## Application 

- **JAMDEC: Unsupervised Authorship Obfuscation using Constrained Decoding over Small Language Models** \
*Jillian Fisher, Ximing Lu, Jaehun Jung, Liwei Jiang, Zaid Harchaoui, Yejin Choi* \
NAACL 2024. [[Paper]](https://arxiv.org/abs/2402.08761) [[Github]](https://github.com/jfisher52/jamdecoding)
<!-- unsupervised  -->

- **Semantically-Aware Constrained Decoding for Code Generation** \
*Kristian Muñiz* \
March 2024.  [[Link]](https://krismuniz.com/posts/constrained-decoding) 
<!-- code generation  -->


- **Discrete Prompt Optimization via Constrained Generation for Zero-shot Re-ranker** \
*Sukmin Cho, Soyeong Jeong, Jeongyeon Seo, Jong C. Park* \
ACL 2023. [[Paper]](https://arxiv.org/abs/2305.13729) [[Github]](https://github.com/zomss/co-prompt)


- **Synchromesh: Reliable code generation from pre-trained language models** \
*Gabriel Poesia, Oleksandr Polozov, Vu Le, Ashish Tiwari, Gustavo Soares, Christopher Meek, Sumit Gulwani* \
ICLR 2022. [[Paper]](https://arxiv.org/abs/2201.11227) [[Github]](https://github.com/kanishkg/synchromesh) 
<!-- code generation  -->
 
