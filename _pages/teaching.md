---
layout: single
title: "Teaching"
permalink: /teaching/
author_profile: true
classes: wide custom-font
---

{% assign courses = site.teaching | sort: "date" | reverse %}
{% assign current_year = nil %}

<div class="teaching-list">
{% for course in courses %}
{% assign year = course.date | date: "%Y" %}
{% unless year == current_year %}
{% assign current_year = year %}
<h2>{{ current_year }}</h2>
{% endunless %}

<div class="teaching-item">
<strong>{{ course.title }}</strong><br>
{% if course.type contains "Graduate" %}🎓{% else %}📘{% endif %} {{ course.type }}<br>
{% assign month = course.date | date: "%m" %}
{% if month <= '05' %}
{% assign term = "Spring" %}
{% elsif month <= '07' %}
{% assign term = "Summer" %}
{% else %}
{% assign term = "Fall" %}
{% endif %}
📅 {{ term }} {{ course.date | date: "%Y" }}<br>
📍 {{ course.venue }}, {{ course.location }}
</div>

{% endfor %}
</div>
