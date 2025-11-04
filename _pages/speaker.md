---
layout: single
permalink: /speakers/
titles: 演讲嘉宾
key: page-speaker
toc: false
classes: wide
---

<div class="grid__wrapper">
  {% for speaker in site.speakers %}
    <div class="grid__item" style="text-align: center; margin-bottom: 2rem;">
      <a href="{{ speaker.url | relative_url }}" style="text-decoration: none;">

        {% if speaker.image %}
          <img src="{{ speaker.image | relative_url }}" alt="{{ speaker.title | escape }}" style="width: 150px; height: 150px; border-radius: 50%; object-fit: cover;">
        {% endif %}

        <h3 style="margin-top: 0.5rem; margin-bottom: 0.2rem;">{{ speaker.title }}</h3>
      </a>

      <p style="font-size: 0.9rem; color: #777;">{{ speaker.bio }}</p>
    </div>
  {% endfor %}
</div>