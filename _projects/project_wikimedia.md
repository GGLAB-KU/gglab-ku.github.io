---
layout: page
title: Terminology-Grounded Translation
img: assets/img/projects/wikimedia.webp
importance: 2
related_publications: true
img_contains_title: true
publications: 'projects^=*terminology'
---

## Bridging the Gap Between Wikipedians and Scientists with Terminology-Aware Translation: A Case Study in Turkish

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/projects/wikimedia.webp" title="Project pipeline" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The pipeline of our proposed project.
</div>

This project addresses the gap between the escalating volume of English-to-Turkish Wikipedia translations and the insufficient number of contributors, particularly in technical domains. Our focus is two folds: 
1. bridging academic/expert and Wikipedia communities,
2. creating datasets, and developing NLP models for terminology identification and linking, and terminology-aware translation

### Project Outcomes and Key Findings

- **TWiST: Turkish-English Wikipedia & Thesis STEM Terminology Dataset:** We compile and annotate a high-quality parallel English to Turkish corpus of size  3,300 sentence pairs evenly split across Mathematics, Physics, and Computer Science. Each sentence pair is annotated with terms, links and their correct translations based on terimler.org. The dataset is available at [Aperta](https://aperta.ulakbim.gov.tr/records/286016)

- **Shared Task at SIGTURK 2026:** We organized a shared task with three subtasks on TWiST. First subtask was "Term detection" where the goal is to find the aligned term spans in both languages. We found that state-of-the-art models can outperform humans in term detection. Second subtask was to change the translation of the term to be consistent with the terminology database and the original morphological process. Even the state-of-the-art models falled back to their preferred translation, failing to follow the expert guidance. Final subtask was the end-to-end translation with the offline glossary, where a small domain adapted model outperformed large generalist models. More information on the participants and the findings can be find in [our paper](https://aclanthology.org/2026.sigturk-1.20/).

- **Wikipedia Technical Translation Guideline:** We develop a guideline for Turkish Wikipedians on how to provide a higher-quality translation for technical documents that contain vast amount of technical terms. We perform a user study where we survey the Wikipedians for the guideline's SUS (System Usability Score), and measure a SUS score of 84/100. The guideline can be accessed through [here](https://tr.wikipedia.org/wiki/Vikipedi:Bilimsel_Terimlere_Duyarl%C4%B1_%C3%87eviri_K%C4%B1lavuzu).

- **Expert-Wikipedian Email Group:** After thorough discussions between the academics and Turkish Wikipedians, we establish an email group to bridge these two communities. The guideline contains detailed instructions on how to reach out to experts in case of difficulties while translating technical terms. There are currently 35 members of the mail group and 19 active, public discussions. The group can be accessed through [here](https://groups.google.com/g/bilimsel-terimler-genel).

- **Public repositories:** All project related resources can be found under our [data git repo](https://github.com/GGLAB-KU/twist), [shared task repo](https://github.com/GGLAB-KU/sigturk2026_sharedtask).  

### Project Team

- **Prof. Dr. Gözde Gül Şahin** (Principal Investigator)  
- **Ali Gebeşçe** 
- **Ege Uğur Amasya**
- **Abdulfattah Rashid Safa**  

#### Former Team Members
- **Mina Durhasan** 
- **Gürkan Soykan** 
- **Gizem Ekiz** 

### Project Date
June 2024 - June 2025

### Funding

This project is funded by the Wikimedia Research Fund. The official project page can be found [here](https://meta.wikimedia.org/wiki/Research:Bridging_the_Gap_Between_Wikipedians_and_Scientists_with_Terminology-Aware_Translation:_A_Case_Study_in_Turkish).

### Publications

<div class="publications">
  {% bibliography -f papers -q @*[projects^=*terminology]* %}
</div>
