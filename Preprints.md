---
layout: page
permalink: /preprints/index.html
title: Preprints
---


pres:
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

{% for pre in page.pres %}
{% unless pre.hidden %}
  - {% if pre.url %} [{{pre.title}}]({{pre.url}}).
    {% else %} {{pre.title}}.
    {% endif %}.
    {{pre.author}}{{pre.journal}}.<br>
    {{pre.month}}, {{pre.year}}. {% if pre.slides %}[Slides]({{pre.slides}}).
    {% endif %}{% if pre.key %}[Bibtex](http://groups.csail.mit.edu/commit/bibtex.cgi?key={{pre.key}}).
    {% endif %}{% if pre.bibtex %}[Bibtex]({{pre.bibtex}}).
    {% endif %}
{% endunless %}
{% endfor %}
