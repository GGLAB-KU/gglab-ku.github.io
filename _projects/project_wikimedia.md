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

This project addresses the gap between the growing volume of English-to-Turkish Wikipedia translations and the limited number of contributors, particularly in technical domains. By leveraging the collaborative efforts of academics in building terminology dictionaries, we propose a pipeline system to improve translation quality. Our focus is on fostering collaboration between academic and Wikipedia communities, creating datasets, and developing NLP models for terminology identification, retrieval, and terminology-aware translation. The goal is to encourage sustained contributions and enhance the overall quality of Turkish Wikipedia articles.

### Project Goals

The project will focus on the following tasks:

- **High-Quality Parallel Corpora for Terminology-Aware Translation:** We aim to generate 3,000 parallel English-Turkish sentences that include: 
    1. English text annotated with technical terms,
    2. Links to the correct terminology entries in the database,
    3. Edited translations using the correct Turkish terminology.

- **Term Identification:** Develop models to identify technical terms in a multilingual setup.

- **Term Linking:** Build models to link identified terms to a terminology database. If the term is not present in the database, a notification system will alert domain experts to add it.

- **Terminology-Aware Translation:** Develop post-editing and translation systems that adhere to the terminology database to ensure consistent and accurate translations.


### Project Team

- **Asst. Prof. Gözde Gül Şahin** (Principal Investigator)  
- **Ali Gebeşçe** (Master's Student)  
- **Ege Uğur Amasya** (Intern)  

#### Former Team Members
- **Mina Durhasan** (Intern)


### Funding

This project is funded by the Wikimedia Research Fund. The official project page can be found [here](https://meta.wikimedia.org/wiki/Grants:Programs/Wikimedia_Research_Fund/Bridging_the_Gap_Between_Wikipedians_and_Scientists_with_Terminology-Aware_Translation:_A_Case_Study_in_Turkish).

### Publications

<div class="publications">
  {% bibliography -f papers -q @*[projects^=*terminology]* %}
</div>
