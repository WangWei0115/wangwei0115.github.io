---
layout: page
permalink: /publications/index.html
title: Publications


pubs:
  - key: "IJOC"
    title: "Optimal model averaging forecasting in high-dimensional survival analysis"
    author: "Yan, X., Wang, H., Wang, W., Xie, J., Ren, Y., & Wang, X."
    month: "Jan"
    year: "2021"
    url: "https://www.sciencedirect.com/science/article/abs/pii/S0169207020301904"
    code: IJOC.bib
---


{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}.
    {% endif %}.
    {{pub.author}}{{pub.journal}}.<br>
    {{pub.month}}, {{pub.year}}. 
{% endunless %}
{% endfor %}


