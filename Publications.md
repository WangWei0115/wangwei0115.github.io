---
layout: page
permalink: /publications/index.html
title: Publications

pubs:
  - author: "Yan, X, Wang, H, Wang W, et al."
    title: "Optimal model averaging forecasting in high-dimensional survival analysis"
    journal: "International Journal of Forecasting"
    month: "Jan"
    year: "2021"
    url: "https://www.sciencedirect.com/science/article/abs/pii/S0169207020301904"
 
---

{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}.
    {% endif %}{% if pub.type %}({{pub.type}})
    {% endif %}{{pub.journal}}.
    {{pub.author}}.
    {% if pub.type == 'Technical Report' %}{{pub.number}}
    {% endif %}{{pub.booktitle}}{{pub.school}}.
    {% if pub.address %}{{pub.address}}.
    {% endif %} {{pub.month}}, {{pub.year}}.<br>{% if pub.key %}[Bibtex](http://groups.csail.mit.edu/commit/bibtex.cgi?key={{pub.key}}).
    {% endif %}{% if pub.bibtex %}[Bibtex]({{pub.bibtex}}).
    {% endif %}
{% endunless %}
{% endfor %}


