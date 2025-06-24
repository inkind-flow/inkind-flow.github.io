---
layout: page
title: Our Team
---

<h2 style="color: {{ site.colors.primary }}">Meet the Team</h2>

<div class="team-grid">
  {% for member in site.data.team %}
    <div class="member">
      <img src="{{ '/' | append: member.image | relative_url }}" alt="{{ member.name }}" loading="lazy">
      <h3>{{ member.name }}</h3>
      <p>{{ member.role }}</p>
      <p>{{ member.bio }}</p>
      <a href="{{ member.linkedin }}" target="_blank" class="btn-linkedin">LinkedIn</a>
    </div>
  {% endfor %}
</div>