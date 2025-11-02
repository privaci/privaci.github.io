---
layout: default
title: All Events
sidebar: none
header: no
permalink: /events.html
---

# All Events

<div class="events-grid">
  {% for event in site.data.events %}
  <div class="event-card">
    <div class="event-header">
      <h3>{{ event.title }}</h3>
    </div>
    <p class="event-location">📍 {{ event.location }}</p>
    {% if event.dates %}
    <p class="event-dates">🗓 {{ event.dates }}</p>
    {% endif %}
    {% if event.link %}
    <a href="{{ event.link }}" class="event-link" target="_blank">Learn More →</a>
    {% endif %}
  </div>
  {% endfor %}
</div>
