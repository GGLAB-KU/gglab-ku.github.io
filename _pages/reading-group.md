---
layout: page
permalink: /reading-group
title: Reading Group
description: Reading Group Meetings in reverse chronological order as the "DD.MM.YYYY" format.
nav: true
nav_rank: 6
---


{% assign groups = site.reading-group | sort: "group_rank" | map: "group" | uniq %}
{% for group in groups %}
&nbsp;
## {{ group }} 


    {% assign papers = site.reading-group | sort: "lastname" | where: "group", group %}
    {% for paper in papers %}
<p>
    <div class="card {% if paper.inline == false %}hoverable{% endif %}">
        <div class="row no-gutters">
            <div class="col-sm-4 col-md-3">
                <img src="{{ '/assets/img/' | append: paper.profile.image | relative_url }}" class="card-img img-fluid" alt="{{ paper.profile.name }}" />
            </div>
            <div class="team col-sm-8 col-md-9">
                <div class="card-body">
                    {% if paper.inline == false %}<a href="{{ paper.url | relative_url }}">{% endif %}
                    <h5 class="card-title">{{ paper.profile.name }}</h5>
                    {% if paper.profile.position %}<h6 class="card-subtitle mb-2 text-muted">{{ paper.profile.position }}</h6>{% endif %}
                    <p class="card-text">
                        {{ paper.teaser | markdownify }}
                    </p>
                    {% if paper.inline == false %}</a>{% endif %}
                    {% if paper.profile.website %}
                        <a href="{{ paper.profile.website }}" class="card-link" target="_blank"><i class="fas fa-globe"></i></a>
                    {% endif %}
                    {% if paper.profile.github %}
                        <a href="https://github.com/{{ paper.profile.github }}" class="card-link" target="_blank"><i class="fab fa-github"></i></a>
                    {% endif %}
                    {% if paper.profile.youtube %}
                        <a href="https://youtube.com/{{ paper.profile.youtube }}" class="card-link" target="_blank"><i class="fab fa-youtube"></i></a>
                    {% endif %}
                </div>
            </div>
        </div>
    </div>
</p>
    {% endfor %}
    
{% endfor %}
