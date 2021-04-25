---
layout: page
permalink: /research/index.html
title: research 

# Publications:
pubs:
  - key: "ansel:pldi:2011"
    title: "Language-Independent Sandboxing of Just-In-Time Compilation, Self-Modifying Code"
    author: "Jason Ansel, Petr Marchenko, Ulfar Erlingsson, Elijah Taylor, Brad Chen, Derek Schuff, David Sehr, Cliff Biffle, Bennet Yee"
    booktitle: "ACM SIGPLAN Conference on Programming Language Design, Implementation"
    month: "Jun"
    year: "2011"
    address: "San Jose, CA"
    keywords: "SFI"
    url: "http://groups.csail.mit.edu/commit/papers/2011/ansel-pldi11-nacljit.pdf"


  - title: Adaptive Checkpointing for Master-Worker Style Parallelism
    author: "Gene Cooperman, Jason Ansel, Xiaoqin Ma"
    booktitle: "IEEE Computer Society International Conference on Cluster Computing"
    address: "Boston, MA"
    month: Sep
    year: 2005
    type: Extended Abstract
    url: 2005cluster.pdf
    bibtex: 2005cluster.bib

---

# Publications

{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}.
    {% endif %}{% if pub.type %}({{pub.type}})
    {% endif %}<br>
    {{pub.author}}.<br>
    {% if pub.type == 'Technical Report' %}{{pub.number}}
    {% endif %}{{pub.booktitle}}{{pub.school}}{{pub.journal}}.<br>
    {% if pub.address %}{{pub.address}}.
    {% endif %} {{pub.month}}, {{pub.year}}. {% if pub.slides %}[Slides]({{pub.slides}}).
    {% endif %}{% if pub.key %}[Bibtex](http://groups.csail.mit.edu/commit/bibtex.cgi?key={{pub.key}}).
    {% endif %}{% if pub.bibtex %}[Bibtex]({{pub.bibtex}}).
    {% endif %}
{% endunless %}
{% endfor %}

# Working Papers:
