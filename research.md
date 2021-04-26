---
layout: page
permalink: /research/index.html
title: research

pubs:
  - author: "Yan, X, Wang, H, Wang W, et al."
    title: "Optimal model averaging forecasting in high-dimensional survival analysis"
    journal: "International Journal of Forecasting"
    month: "Jan"
    year: "2021"
    url: "https://www.sciencedirect.com/science/article/abs/pii/S0169207020301904"
 
---
# Publications 

{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).{% else %} {{pub.title}}.{% endif %}
    {{pub.journal}}.
    {{pub.author}}.
    {{pub.month}},
    {{pub.year}}.
    {% if pub.code %}[Code]({{pub.code}}).{% endif %}
    {% if pub.supplement %}[Supplement]({{pub.supplement}}).{% endif %}
{% endunless %}
{% endfor %}


# Working Papers

- Wang W., Xiao Z., Ren Y., Yan X., 2021, "A Bi-integrative analysis of two-dimensional heterogeneous panel data models with group and group and cohort structure recovery"
    
- Feng Q., Wang W., 2021, "Nonstationary Heterogeneous Panels with Structural Breaks"