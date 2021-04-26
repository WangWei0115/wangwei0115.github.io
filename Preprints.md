---
layout: page
permalink: /preprints/index.html
title: Preprints
---

pres:
  - title: "A Bi-integrative analysis of two-dimensional heterogeneous panel data models with"
    author: "Wei Wang, Zhijie Xiao, Yanyan Ren, Xiaodong Yan"
    month: "Jan"
    year: "2021"
  - title: "Nonstationary Heterogeneous Panels with Structural Breaks"
    author: "Qu Feng, Wei Wang"
    month: April
    year: 2021
---

{% for pre in page.pres %}
{% unless pre.hidden %}
  - {% if pre.url %} [{{pre.title}}]({{pre.url}}).
    {% else %} {{pre.title}}.
    {% endif %}.
    {{pre.author}}{{pre.journal}}.<br>
    {{pre.month}}, {{pre.year}}. 
{% endfor %}
