---
layout: about
inline: true
title: ALfaLFas
description: Automatic Learning of Procedural Language from Natural Language Instructions for Intelligent Assistance

img: assets/img/projects/alfalfas.webp
img_contains_title: true
publications: 'projects^=*ALfaLFas'

profile:
    name: ALfaLFas
    image: projects/alfalfas.webp
    align: left
    address: >
---

## Automatic Learning oF ProcedurAl Language From NAtural Language InStructions for Intelligent Assistance 

<br>

### Motivation
Despite the number of studies that report exceptionally high scores (Devlin et. al., 2019) for downstream natural language processing (NLP) tasks, a growing number of studies discuss the gap between their performance on such tasks and on real-world tasks that require “understanding” ([Bender & Koller, 2020](https://aclanthology.org/2020.acl-main.463.pdf)). Some of the major causes for this are (i) neural models not being able to generalize to out-of-domain data, (ii) downstream tasks not containing the challenges of real-world scenarios and iii) not having suitable evaluation measures.

In order to bring the performance on real-life and downstream tasks closer, this project proposes a novel task for understanding natural language utterances within a more realistic and challenging scope: **understanding human-written instructions**. Giving step-by-step instructions is one of the primary way of human communication to teach someone a new topic or a task. The research plan envisions a future, where people would also be able to instruct machines with such step-by-step instructions, and this research project aims to take the first step towards that goal by developing necessary tools to parse natural language utterances into a sequence of procedures. The advantage of having such a representation would be having the ability to reduce the statements automatically by using an off-the-shelf interpreter and enrich the final model with domain-specific knowledge/rules which cannot be easily learned from data.

A subfield of lingustics, semantics—the study of meaning—has researched how to *best represent meaning* for decades. The number of theorems that are introduced are too many to list here, however most theorems underline some common challenges such as *quantifiers, negation scope* and propose a way to address them in their representation scheme. However most of these representations are designed for sentences, ignoring the *inter-sentential connections* (e.g., After, then, because) and *co-referring with pronouns* (e.g., Sue is sick. She (Sue) won’t work tomorrow). Another prominent problem that occurs specifically in instruction text is *zero anaphora*. Imagine the 2-step procedure: “Mix the macaroni and cheese. Bake for 10 minutes.”. Here what to bake and where to bake are not explicitly stated but inferred from the context. Finally, referring is mostly done to an implicit (non-existing in text) object. For instance if we said “Bake it for 10 minutes”, it would refer to the product of the mixing action.Therefore, the first central research question is: “What is the best way to represent the meaning of step-by-step instructions?”.

Another major challenge arises when we want build models to *parse instructions from various domains into executable procedures*. We want a model trained with car repair instructions that contains some mixing actions (e.g., mixing paints) to be able to parse a cooking instruction that contains a mixing action correctly. Even though this is fairly easy for humans—thanks to our conceptual reasoning abilities— machines tend to overfit and not generalize to unseen domains, and similarly to unseen instructions. One way to tackle this challenge is to develop models, or improve existing models, with conceptual reasoning abilities. Extraction of concepts, however, requires the ability to identify and remember the reoccurring, important patterns and abstracting them from their surface forms, i.e., symbolize them. Hence the second central research question we pose in this project is: “How can we build generalizable models for processing raw text into well-defined procedures?”.

Final obstacle that stands on the way is the *right evaluation measures* to track the progress in the direction of generalizable natural language processing models. The task we define already sets up a realistic measure, however, measuring the progress with one single score has been shown to be problematic. The reasons are as follows. First of all, neural models are not interpretable. Hence their strengths and weaknesses can not be analyzed simply by looking at a single score. Second, a single score only shows how good a model performs on this specific test set, rather than how good a model is by means of the skills required by the task (e.g., logical deduction, mathematical reasoning). As mentioned, this project hypothesizes that improving the ability of long-range reasoning would yield more generalizable models. That brings us to the final research question: “Which reasoning/logical skills are required for processing instructions?” and “How can we measure these skills adequately?”

### Goals

The project will investigate three major research directions to answer the aforementioned RQs:

 - Large, Structured Dataset of Procedural Information Spanning Multiple Domains: In order to
conduct research on data-driven and generalizable models for procedural language understanding, the
field requires large amounts of annotated corpora of goal-oriented instructions and procedures from
variety of domains.
 - Evaluation Benchmark for Distinct Cognitive Abilities: The task of interpreting procedures
encloses various linguistic and reasoning challenges. Nonetheless, the researchers are inclined to
evaluate only on the end result using a single score. 
- Neural/Hybrid Models with Long-Range Reasoning Abilities for Procedural Text: We will contribute with i) investigating the generalizability of existing techniques on the procedural text, and ii) developing novel models inspired from existing cognitive architectures. 

### Team

 - Asst. Prof. Gözde Gül Şahin
 - Abdalfatah Rashid Safa, MSc, Müge Kural, MSc

### Funding

This project (ID:1109B322100424) is funded within the scope of Tübitak 2232B International Fellowship for Outstanding Researchers funding scheme. (Funding Period: 09.2022-09.2025)

### Credit
<a href="https://www.freepik.com/free-photo/3d-render-robot-with-books_1166338.htm#query=robot%20reading%20instruction&position=0&from_view=search&track=ais">Image by kjpargeter</a> on Freepik