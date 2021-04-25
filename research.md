---
layout: page
permalink: /research/index.html
title: research 

# Publications:
pubs:
  - key: "ansel:pldi:2011"
    title: "Language-Independent Sandboxing of Just-In-Time Compilation, Self-Modifying Code"
    author: "Jason Ansel"
    month: "Jun"
    year: "2011"
    keywords: "SFI"
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
pubs:
  - key: "ansel:pldi:2011"
    title: "Language-Independent Sandboxing of Just-In-Time Compilation, Self-Modifying Code"
    author: "Jason Ansel"
    month: "Jun"
    year: "2011"
    keywords: "SFI"
    url: "http://groups.csail.mit.edu/commit/papers/2011/ansel-pldi11-nacljit.pdf"

  - title: Adaptive Checkpointing for Master-Worker Style Parallelism
    author: "Gene Cooperman, Jason Ansel, Xiaoqin Ma"
    month: Sep
    year: 2005
    url: 2005cluster.pdf
    bibtex: 2005cluster.bib

---

# Working Papers:

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