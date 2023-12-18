---
layout: about
inline: false
group: 11.12.2023
group_rank: 1


title: In-Context Learning for Few-Shot Dialogue State Tracking
description: Paper - 1 description

teaser: This paper presents an in-context learning framework for dialogue state tracking that reformulates the task into a text-to-SQL problem, enabling zero-shot and few-shot learning without parameter updates and achieving superior performance in both settings.
   
profile:
    name: In-Context Learning for Few-Shot Dialogue State Tracking <br />
    align: middle
    image: readinggroup/2203.08568.webp
    website: https://arxiv.org/abs/2203.08568
    github: Yushi-Hu/IC-DST/
---

#####  **In-Context Learning for Few-Shot Dialogue State Tracking**
###### **Resources**: [Paper](https://arxiv.org/abs/2203.08568), [Code](https://github.com/Yushi-Hu/IC-DST/)
###### **Authors**: Yushi Hu, Chia-Hsuan Lee, Tianbao Xie, Tao Yu, Noah A. Smith, Mari Ostendorf
###### **Year**: 2022
###### **Venue**: Findings of the Association for Computational Linguistics: EMNLP 2022
###### **Abstract**: "Collecting and annotating task-oriented dialogues is time-consuming and costly; thus, zero and few shot learning could greatly benefit dialogue state tracking (DST). In this work, we propose an in-context learning (ICL) framework for zero-shot and few-shot learning DST, where a large pre-trained language model (LM) takes a test instance and a few exemplars as input, and directly decodes the dialogue state without any parameter updates. To better leverage a tabular domain description in the LM prompt, we reformulate DST into a text-to-SQL problem. We also propose a novel approach to retrieve annotated dialogues as exemplars. Empirical results on MultiWOZ show that our method IC-DST substantially outperforms previous fine-tuned state-of-the- art models in few-shot settings. In addition, we test IC-DST in zero-shot settings, in which the model only takes a fixed task instruction as input, finding that it outperforms previous zero-shot methods by a large margin."
 ![IC-DST](/assets/img/readinggroup/fig1.png)
###### **Conclusion**: "We successfully apply in-context learning for dialogue state tracking by introducing a new approach to representing dialogue context, a novel objective for retriever training, and by reformulating DST into a text-to-SQL task. On MultiWOZ, our system achieves a new state of the art in both few-shot and zero-shot settings. Our analyses show that each innovation benefits performance. We also study in detail the contribution of each design decision. Future work may apply this in-context learning framework to a wider range of dialogue tasks."

### **Group Meeting Notes**
##### **Date**: December 11, 2023
##### **Participants**: Gürkan Soykan, Tamta Kapanadze, Abdulfattah Safa



