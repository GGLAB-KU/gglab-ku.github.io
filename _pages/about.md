---
layout: about
title: Home
permalink: /
nav: true
nav_rank: 1
sitetitle: true
description: Welcome to the GGLab at Koç University. Team. Projects.

profile:
  name: GGLab, NLP Research Group at Koç University
  align: left
  image: new_group.webp
  image_circular: false # crops the image to make it circular
  image_caption: Group Members (2023)
  email: gosahin@ku.edu.tr


news: true  # includes a list of news items
projects: true
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false  # includes social icons at the bottom of the page
---


GGLab (pronounced as "cici" in Turkish) is a Natural Language Processing (NLP) research lab led by [Asst. Prof. Gözde Gül Şahin](https://gozdesahin.github.io/). We have a keen interest in conducting fundamental research in core methodologies, including but not limited to areas such as learning/performing under low-resource settings and incorporating expert knowledge in language technologies. Additionally, we explore how these methodologies can be applied to various tasks, such as text simplification, linguistic structure analysis, grammatical error correction, dialogue understanding and question answering. We are part of [Computer Science Department](https://cs.ku.edu.tr/) at [Koç University](https://www.ku.edu.tr/) and affiliated with [KUIS AI Lab](https://ai.ku.edu.tr/), located in the north of Istanbul, Türkiye. GGLab is partly funded by [Scientific and Technological Research Council of Türkiye](https://www.tubitak.gov.tr/) via Tübitak 2232B International Fellowship for Outstanding Researchers program, and [Wikimedia Foundation](https://wikimediafoundation.org/) via [Wikimedia Research Fund](https://meta.wikimedia.org/wiki/Grants:Programs/Wikimedia_Research_%26_Technology_Fund/Wikimedia_Research_Fund).   

[Talk to us](mailto:gosahin@ku.edu.tr) or
[join our group]({{ '/open-positions' | relative_url }})
when you are interested in these topics or our work.

{% assign members = site.members | where: "team_frontpage", true | sort: "lastname" %}
<div class="d-flex flex-wrap align-content-stretch justify-content-center m-n2 pt-5 no-gutters">
    {% for member in members %}
        {% assign colsMod6 = forloop.length | modulo: 6 %}
        {% assign colIdMod4 = forloop.index | modulo: 4 %}
        {% if colsMod6 == 1 and colIdMod4 == 1 %}<div class="col-md-2 w-100"></div>{% endif %}
        <div class="col-6 col-sm-3 col-md-2 mb-3">
            <a href="{{ member.url | relative_url }}" class="no-decoration">
                <div class="card hoverable h-100 m-2">
                    <img src="{{ '/assets/img/' | append: member.profile.image | relative_url }}" class="card-img-top" alt="{{ member.profile.name }}" />
                    <div class="card-body p-2">
                        <div class="card-title m-0">{{ member.title }}</div>
                    </div>
                </div>
            </a>
        </div>
    {% endfor %}
</div>


