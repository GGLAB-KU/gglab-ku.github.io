---
layout: page
title: ALfaLFas
img: assets/img/projects/alfalfas.webp
importance: 1
related_publications: true
img_contains_title: true
publications: 'projects^=*ALfaLFas'
---

## Automatic Learning oF ProcedurAl Language From NAtural Language InStructions for Intelligent Assistance

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/alfalfas.webp" title="ALfaLFas" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Giving step-by-step instructions is one of the primary ways humans teach a new task; this project asks whether machines can be taught the same way. Understanding natural language instructions requires tackling challenges unique to procedural text: *zero anaphora* ("Mix the macaroni and cheese. Bake for 10 minutes.": what to bake, and where, goes unstated), implicit co-references, and inter-sentential dependencies that go beyond sentence-level semantics. Three research questions drive the project: *What is the best way to represent the meaning of step-by-step instructions? How can we build generalizable models for parsing raw instructions into executable procedures? And which reasoning skills does this require, and how do we measure them adequately?* To answer these, the project pursued a comprehensive survey of the field, built evaluation benchmarks for procedural language understanding, and ultimately advanced toward a multi-agent cognitive architecture capable of learning new procedural tasks at inference time, enabling personal assistants that users can genuinely teach.

### Project Outcomes and Key Findings

- **Instructional Text Survey:** We authored a comprehensive survey, "Instructional Text Across Disciplines: A Survey of Representations, Downstream Tasks, and Open Challenges Toward Capable AI Agents," covering representation formats, datasets, and downstream tasks across the full landscape of procedural language understanding, examining 181 papers. Published in *Computational Linguistics* (2026).

- **PARADISE: Procedural Planning Benchmark:** We introduced PARADISE, an abductive reasoning benchmark using a Q&A format on practical procedural text sourced from wikiHow. The task evaluates whether language models can infer implicit warnings and tips from a procedure goal alone, without intermediary steps, testing implicit planning skills. Published at *ACL 2024 Findings*.

- **Turkish Procedural Language Understanding Benchmarks:** We expanded Turkish wikiHow from 2,000 to 52,000 tutorials and generated downstream tasks including action linking, goal inference, and summarization, providing the first large-scale benchmark suite for procedural language understanding in a low-resource, morphologically rich language. Published at *IJCNLP-AACL 2023*.

- **Multi-Agent Cognitive Architecture for Inference-Time Learning:** We designed a novel multi-agent architecture featuring a four-layer cognitive memory system (Working, Episodic, Semantic, Procedural) augmented with Meta-Memory for confidence tracking. This architecture enables intelligent assistants to acquire new procedural workflows and personalize behavior directly during live interactions, without gradient-based retraining, through a seven-step adaptive execution flow.

- **Dataset and Longitudinal Evaluation Framework:** We designed a novel three-phase dataset capturing realistic user-AI teaching interactions, including procedural demonstrations and correction cycles, using fictional API schemas to prevent data contamination. We also proposed a longitudinal evaluation framework to measure learning effectiveness and personalization quality across extended interaction periods.

- **Public Resources:** Project-related resources and code are available under our [GitHub organization](https://github.com/GGLAB-KU).

### Project Team

- **Prof. Dr. Gözde Gül Şahin**
- **Abdulfattah Rashid Safa**
- **Tamta Kapanadze**
- **Ali Gebeşçe**
- **Hulki Ciray**

#### Former Team Members
- **Betül Özateş**
- **Müge Kural**
- **Gürkan Soykan**
- **Tilek Chubakov**
- **Atakan Kara**
- **Farrin Marouf Sofian**
- **Andrew Bond**
- **Subha Vadlamannati**
- **Arda Uzunoğlu**

### Project Date
September 2022 - September 2025

### Funding

This project (121C132) is funded within the scope of TÜBİTAK 2232 International Fellowship for Outstanding Researchers.

### Publications

<div class="publications">
  {% bibliography -f papers -q @*[projects^=*ALfaLFas]* %}
</div>

#### Credit
<a href="https://www.freepik.com/free-photo/3d-render-robot-with-books_1166338.htm#query=robot%20reading%20instruction&position=0&from_view=search&track=ais">Image by kjpargeter</a> on Freepik

<!--
#### Motivation
Despite the number of studies that report exceptionally high scores (Devlin et. al., 2019) for downstream natural language processing (NLP) tasks, a growing number of studies discuss the gap between their performance on such tasks and on real-world tasks that require "understanding" ([Bender & Koller, 2020](https://aclanthology.org/2020.acl-main.463.pdf)). Some of the major causes for this are (i) neural models not being able to generalize to out-of-domain data, (ii) downstream tasks not containing the challenges of real-world scenarios and iii) not having suitable evaluation measures.

In order to bring the performance on real-life and downstream tasks closer, this project proposes a novel task for understanding natural language utterances within a more realistic and challenging scope: **understanding human-written instructions**. Giving step-by-step instructions is one of the primary way of human communication to teach someone a new topic or a task. The research plan envisions a future, where people would also be able to instruct machines with such step-by-step instructions, and this research project aims to take the first step towards that goal by developing necessary tools to parse natural language utterances into a sequence of procedures. The advantage of having such a representation would be having the ability to reduce the statements automatically by using an off-the-shelf interpreter and enrich the final model with domain-specific knowledge/rules which cannot be easily learned from data.

A subfield of lingustics, semantics—the study of meaning—has researched how to *best represent meaning* for decades. The number of theorems that are introduced are too many to list here, however most theorems underline some common challenges such as *quantifiers, negation scope* and propose a way to address them in their representation scheme. However most of these representations are designed for sentences, ignoring the *inter-sentential connections* (e.g., After, then, because) and *co-referring with pronouns* (e.g., Sue is sick. She (Sue) won't work tomorrow). Another prominent problem that occurs specifically in instruction text is *zero anaphora*. Imagine the 2-step procedure: "Mix the macaroni and cheese. Bake for 10 minutes.". Here what to bake and where to bake are not explicitly stated but inferred from the context. Finally, referring is mostly done to an implicit (non-existing in text) object. For instance if we said "Bake it for 10 minutes", it would refer to the product of the mixing action.Therefore, the first central research question is: "What is the best way to represent the meaning of step-by-step instructions?".

Another major challenge arises when we want build models to *parse instructions from various domains into executable procedures*. We want a model trained with car repair instructions that contains some mixing actions (e.g., mixing paints) to be able to parse a cooking instruction that contains a mixing action correctly. Even though this is fairly easy for humans—thanks to our conceptual reasoning abilities— machines tend to overfit and not generalize to unseen domains, and similarly to unseen instructions. One way to tackle this challenge is to develop models, or improve existing models, with conceptual reasoning abilities. Extraction of concepts, however, requires the ability to identify and remember the reoccurring, important patterns and abstracting them from their surface forms, i.e., symbolize them. Hence the second central research question we pose in this project is: "How can we build generalizable models for processing raw text into well-defined procedures?".

Final obstacle that stands on the way is the *right evaluation measures* to track the progress in the direction of generalizable natural language processing models. The task we define already sets up a realistic measure, however, measuring the progress with one single score has been shown to be problematic. The reasons are as follows. First of all, neural models are not interpretable. Hence their strengths and weaknesses can not be analyzed simply by looking at a single score. Second, a single score only shows how good a model performs on this specific test set, rather than how good a model is by means of the skills required by the task (e.g., logical deduction, mathematical reasoning). As mentioned, this project hypothesizes that improving the ability of long-range reasoning would yield more generalizable models. That brings us to the final research question: "Which reasoning/logical skills are required for processing instructions?" and "How can we measure these skills adequately?"

#### Goals

The project investigates three major research directions to answer the aforementioned RQs:

 - Large, Structured Dataset of Procedural Information Spanning Multiple Domains: In order to
conduct research on data-driven and generalizable models for procedural language understanding, the
field requires large amounts of annotated corpora of goal-oriented instructions and procedures from
variety of domains.
 - Evaluation Benchmark for Distinct Cognitive Abilities: The task of interpreting procedures
encloses various linguistic and reasoning challenges. Nonetheless, the researchers are inclined to
evaluate only on the end result using a single score.
- Neural/Hybrid Models with Long-Range Reasoning Abilities for Procedural Text: We will contribute with i) investigating the generalizability of existing techniques on the procedural text, and ii) developing novel models inspired from existing cognitive architectures.
-->
