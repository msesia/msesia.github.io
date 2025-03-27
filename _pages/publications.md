---
layout: single
title: "Publications"
permalink: /publications/
author_profile: true
classes: wide custom-font
---

{% assign pubs = site.publications | sort: "year" | reverse %}
{% assign current_year = nil %}

<div class="publication-list">
  {% for pub in pubs %}
    {% unless pub.year == current_year %}
      {% assign current_year = pub.year %}
      <h2>{{ current_year }}</h2>
    {% endunless %}

    <div class="pub-item">
      <div class="pub-title">
        <strong>{{ pub.title }}
        {% if pub.icon %}
          <span class="pub-icon">{{ pub.icon }}</span>
        {% endif %}
        </strong>
      </div>
      <div class="pub-authors">{{ pub.authors | strip }}</div>
      <div class="pub-venue"><em>{{ pub.venue }}</em>, {{ pub.year }}</div>
      <div class="pub-links">
        {% if pub.preprint %}
          <a href="{{ pub.preprint }}" target="_blank" rel="noopener noreferrer">[Preprint]</a>
        {% endif %}
        {% if pub.published %}
          <a href="{{ pub.published }}" target="_blank" rel="noopener noreferrer">[Published]</a>
        {% endif %}
        {% if pub.bibtex %}
          <a href="{{ pub.bibtex }}" target="_blank" rel="noopener noreferrer">[BibTeX]</a>
        {% endif %}
      </div>
      <br>
    </div>
  {% endfor %}
</div>
