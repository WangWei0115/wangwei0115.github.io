---
layout: page
permalink: /publications/index.html
title: Publications

pubs:
  - author: "Yan, X, Wang, H, Wang, W, Xie, J, Ren, Y, & Wang, X"
    title: "Optimal model averaging forecasting in high-dimensional survival analysis"
    month: "Jan"
    year: "2021"
 
---


{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}.
    {% endif %}{% if pub.type %}({{pub.type}})
    {% endif %}{{pub.journal}}{{pub.author}}.
    {{pub.month}}, {{pub.year}}.<br> {% if pub.code %}[Code]({{pub.code}}).
    {% endif %}
{% endunless %}
{% endfor %}


