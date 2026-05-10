---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

## Preprints and Under Review

{% assign preprints = site.publications | where: "category", "preprint" | sort: "date" | reverse %}
{% for post in preprints %}
  {% include archive-single.html %}
{% endfor %}

## Peer-Reviewed Publications

{% assign peer_reviewed = site.publications | where: "category", "peer-reviewed" | sort: "date" | reverse %}
{% for post in peer_reviewed %}
  {% include archive-single.html %}
{% endfor %}
