---
layout: default
title: Analysen
permalink: /analyses/
---

# Spielanalysen

Diese Seite listet alle bisher aufgenommenen Beiträge des Living Game Repository. In der Proof-of-Concept-Phase handelt es sich um interne oder kuratierte studentische Beiträge.

{% assign items = site.analyses | sort: "title" %}

<div class="card-grid">
{% for item in items %}
<div class="card">
  <h3>{{ item.url | relative_url }}{{ item.title }}</a></h3>
  <p><strong>Spiel/Medium:</strong> {{ item.game }}</p>
  <p><strong>Theorie:</strong> {{ item.theory }}</p>
  <p><strong>Schwerpunkt:</strong> {{ item.focus }}</p>
  <p><strong>Status:</strong> {{ item.status }}</p>
</div>
{% endfor %}
</div>