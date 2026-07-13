---
layout: default
title: Start
permalink: /
---

# Living Game Repository

Das Living Game Repository ist eine wachsende Sammlung psychologischer Spielanalysen. Es verbindet psychologische Theoriearbeit, digitale Medienanalyse, wissenschaftliches Schreiben und studentische Wissensproduktion.

In der Proof-of-Concept-Phase wird das Repository zunächst durch Studierendeninput getragen. Ziel ist es, zu erproben, ob aus theoriegeleiteten Spielanalysen wiederverwendbare Materialien für Lehre, Forschung, Transfer und Wissenschaftskommunikation entstehen können.

## Was findet sich hier?

<div class="card-grid">

  <div class="card">
    <h3>Spielanalysen</h3>
    <p>Theoriegeleitete Analysen einzelner Spiele, Spielmechaniken, Tutorials, Figuren oder Spielerfahrungen.</p>
    <p>
      <a href="{{ "/analyses/" | relative_url }}">Zu den Analysen</a>
    </p>
  </div>

  <div class="card">
    <h3>Theorien</h3>
    <p>Psychologische Konzepte wie Selbstwirksamkeit, Flow, Selbstbestimmungstheorie, Presence, Eudaimonia oder CTML.</p>
    <p>
      <!-- Adjust href when you have a theory overview page -->
      <a href="{{ "/theories/" | relative_url }}">Theorieübersicht</a>
    </p>
  </div>

  <div class="card">
    <h3>Für Studierende</h3>
    <p>Anleitungen, Templates und Hinweise zur Erstellung eigener Beiträge.</p>
    <p>
      <a href="{{ "/contribute/" | relative_url }}">Beitrag erstellen</a>
    </p>
  </div>

</div>

## Aktuelle Beispielanalysen

{% if site.analyses %}
  {% assign items = site.analyses | sort: "title" %}

  <ul>
    {% for item in items %}
      <li>
        <a href="{{ item.url | relative_url }}">
          {{ item.title }}
        </a>
        {% if item.theory %}
          – <em>{{ item.theory }}</em>
        {% endif %}
      </li>
    {% endfor %}
  </ul>
{% else %}
  <p>Derzeit sind keine Beispielanalysen verfügbar.</p>
{% endif %}

## Entwicklungslogik

Das Repository ist „living“, weil es semesterweise erweitert, überarbeitet und strukturell weiterentwickelt wird. Die erste Phase ist bewusst niedrigschwellig. Perspektivisch kann daraus eine professionellere Infrastruktur mit Qualitätsstufen, redaktioneller Kuratierung, öffentlicher Showcase-Ebene und stärkerer technischer Such- und Filterfunktion entstehen.
