---
layout: post
date: 2024-03-06
inline: true
---

Our new paper is available on [arXiv](https://arxiv.org/)!

***
Our paper entitled [PARADISE: Evaluating Implicit Planning Skills of Language Models with Procedural Warnings and Tips Dataset]({{ '/assets/pdf/2403.03167.pdf' | relative_url }}) is available on [arXiv](https://arxiv.org/)! Check the [repo](https://github.com/GGLAB-KU/paradise) for more details 📣

> Abstract: Recently, there has been growing interest within the community regarding whether large language models are capable of planning or executing plans. However, most prior studies use LLMs to generate high-level plans for simplified scenarios lacking linguistic complexity and domain diversity, limiting analysis of their planning abilities. These setups constrain evaluation methods (e.g., predefined action space), architectural choices (e.g., only generative models), and overlook the linguistic nuances essential for realistic analysis. To tackle this, we present PARADISE, an abductive reasoning task using Q\&A format on practical procedural text sourced from wikiHow. It involves warning and tip inference tasks directly associated with goals, excluding intermediary steps, with the aim of testing the ability of the models to infer implicit knowledge of the plan solely from the given goal. Our experiments, utilizing fine-tuned language models and zero-shot prompting, reveal the effectiveness of task-specific small models over large language models in most scenarios. Despite advancements, all models fall short of human performance. Notably, our analysis uncovers intriguing insights, such as variations in model behavior with dropped keywords, struggles of BERT-family and GPT-4 with physical and abstract goals, and the proposed tasks offering valuable prior knowledge for other unseen procedural tasks. The PARADISE dataset and associated resources are publicly available for further research exploration with this https URL.