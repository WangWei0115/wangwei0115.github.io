---
layout: page
permalink: /research/index.html
title: research 


pubs:
  - key: "ansel:pldi:2011"
    title: "Language-Independent Sandboxing of Just-In-Time Compilation, Self-Modifying Code"
    author: "Jason Ansel"
    month: "Jun"
    year: "2011"
    url: "http://groups.csail.mit.edu/commit/papers/2011/ansel-pldi11-nacljit.pdf"

  - title: Adaptive Checkpointing for Master-Worker Style Parallelism
    author: "Gene Cooperman, Jason Ansel, Xiaoqin Ma"
    month: Sep
    year: 2005
    url: 2005cluster.pdf
    bibtex: 2005cluster.bib
---

works:
  - key: "ansel:pldi:2011"
    title: "Language-Independent Sandboxing of Just-In-Time Compilation, Self-Modifying Code"
    author: "Jason Ansel"
    month: "Jun"
    year: "2011"
    url: "http://groups.csail.mit.edu/commit/papers/2011/ansel-pldi11-nacljit.pdf"

  - title: Adaptive Checkpointing for Master-Worker Style Parallelism
    author: "Gene Cooperman, Jason Ansel, Xiaoqin Ma"
    month: Sep
    year: 2005
    url: 2005cluster.pdf
    bibtex: 2005cluster.bib
---


# Publications 

{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}.
    {% endif %}.
    {{pub.author}}.
    {{pub.booktitle}}{{pub.school}}{{pub.journal}}.<br>
    {{pub.month}}, {{pub.year}}. {% if pub.slides %}[Slides]({{pub.slides}}).
    {% endif %}{% if pub.key %}[Bibtex](http://groups.csail.mit.edu/commit/bibtex.cgi?key={{pub.key}}).
    {% endif %}{% if pub.bibtex %}[Bibtex]({{pub.bibtex}}).
    {% endif %}
{% endunless %}
{% endfor %}

# Working Papers:

{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}.
    {% endif %}.
    {{pub.author}}.
    {{pub.booktitle}}{{pub.school}}{{pub.journal}}.<br>
    {{pub.month}}, {{pub.year}}. {% if pub.slides %}[Slides]({{pub.slides}}).
    {% endif %}{% if pub.key %}[Bibtex](http://groups.csail.mit.edu/commit/bibtex.cgi?key={{pub.key}}).
    {% endif %}{% if pub.bibtex %}[Bibtex]({{pub.bibtex}}).
    {% endif %}
{% endunless %}
{% endfor %}