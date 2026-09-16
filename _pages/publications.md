---
layout: portfolio
title: Publications
kicker: Research
permalink: /publications/
intro: Work on learning methods, structured generation, and applications in health and science.
---
<p><a href="https://scholar.google.com/citations?hl=en&amp;user=9IjNO2sAAAAJ">Google Scholar ↗</a></p>
<h2>Preprints &amp; submissions</h2>
<ol class="paper-list">{% for paper in site.data.papers %}{% if paper.status %}<li><span class="venue">{{ paper.status }}</span><h3>{% if paper.url %}<a href="{{ paper.url }}">{{ paper.title }}</a>{% else %}{{ paper.title }}{% endif %}</h3><p>{{ paper.authors | join: ', ' }}</p></li>{% endif %}{% endfor %}</ol>
<h2>Peer-reviewed publications</h2>
<ol class="paper-list">{% for paper in site.data.papers %}{% if paper.venue %}<li><span class="venue">{{ paper.venue }}</span><h3>{% if paper.url %}<a href="{{ paper.url }}">{{ paper.title }}</a>{% else %}{{ paper.title }}{% endif %}</h3><p>{{ paper.authors | join: ', ' }}</p></li>{% endif %}{% endfor %}</ol>
