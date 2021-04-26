---
layout: page
permalink: /publications/index.html
title: Publications

pubs:
  - author: "Yan, X, Wang, H, Wang, et al."
    title: "Optimal model averaging forecasting in high-dimensional survival analysis"
    journal: "International Journal of Forecasting"
    month: "Jan"
    year: "2021"
 
---


{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}.{% endif %}
    {{pub.journal}}{{pub.author}}.<br> {% if pub.code %}[Code]({{pub.code}}).
    {% endif %}{% if pub.supplement %}[Code]({{pub.supplement}}).
    {% endif %}
    
{% endunless %}
{% endfor %}


