<div align="center">
<h1>AUITestAgent: Natural Language-Driven GUI Functional Bug Tester</h1>
</div>

<div align="center">
<a>arxiv link here</a>
</div>

<div align="center">
Yongxiang Hu<sup>1</sup>, Xuan Wang<sup>1</sup>, Yingchuan Wang<sup>1</sup>, Yu Zhang<sup>2</sup>, Shiyu Guo<sup>2</sup>, Chaoyi Chen<sup>2</sup>, Xin Wang<sup>1,3</sup> and Yangfan Zhou<sup>1,3</sup>

<br>

<sup>1</sup>School of Computer Science, Fudan University  
<sup>2</sup>Meituan, China  
<sup>3</sup>Shanghai Key Laboratory of Intelligent Information Processing, Shanghai, China
</div>

<!-- <div style="display: flex; justify-content: center; align-items: center;">
  <img src="assets/fudan.png" alt="Fudan University Logo" width="100" style="margin-right: 50px"/>
  <img src="assets/meituan.png" alt="Meituan Logo" width="100"/>
</div> -->

## 🌟 Introduction

AUITestAgent is a LLM-based multi-agent framework for automatically perform natural language-driven GUI functional bug testing. It takes test requirements written in natural language as input, generates and conducts UI interactions, and verifies whether the UI response aligns with the expectations outlined in the requirements.

<center><img src="assets/overview.png" width="90%" height="90%" /></center>

To enhance the performance of LLM-based agents in the domain-specific area of UI testing, AUITestAgent decouples GUI interaction and function verification into two separate modules, performing verification after interaction.

 In terms of implementation, AUITestAgent extracts GUI interactions from test requirements using dynamically organized agents to tackle the diversity of requirement expressions. Then, a multi-dimensional data extraction strategy is employed to retrieve data relevant to the test requirements from the interaction trace and performs verification.

## 📺 Demo

### Using AUITestAgent in Meituan 

todo: video

![demo1](assets/demo1.png)


### Using AUITestAgent in Facebook

todo: video

![demo2](assets/demo2.png)


## 📝 Evaluation

We evaluate AUITestAgent’s performance with two customized benchmark, [interaction benchmark](interaction.md) and [verification benchmark](verification.md), including 8 widely used commercial apps (*i.e.,* Meituan, Little Reb Book, Douban, Facebook, Gmail, linkedIn, Google play and YouTube Music). 

Our experiments show that AUITestAgent accurately completes 77% of interaction tasks, **significantly outperforms existing methods in natrual language commands to GUI interactions translation.** Additionally, it can detect 91% of injected GUI functional bugs with a false positive rate of just 3%.
Furthermore, unseen bugs detected from Meituan show the practical benefits of using AUITestAgent to conduct GUI testing for complex commercial apps.

For detail information, please refer to the [evalution results](evaluation_results/evaluation.md).

### GUI Interactions translation

![interaction result](assets/interaction.png)

Baseline: 
* [MobileAgent](https://github.com/X-PLUG/MobileAgent)
* [AppAgent](https://github.com/mnotgod96/AppAgent)


### Function Verification

![verification result](assets/verification.png)

## 📚 Citation
```bib
todo
```