---
layout: archive
permalink: /machine-learning/
title: "Machine Learning Posts by Topics"
author_profile: true
tags: ML

---

{% for post in site.tags.ML  %}

  <ul class="taxonomy__index">
    {% assign postsInYear = site.posts | group_by_exp: 'post', 'post.date | date: "%Y"' %}
    {% for year in postsInYear %}
      <li>
        <a href="#{{ year.name }}">
          <strong>{{ year.name }}</strong> <span class="taxonomy__count">{{ year.items | size }}</span>
        </a>
      </li>
    {% endfor %}
  </ul>

  {% assign postsByYear = site.posts | group_by_exp: 'post', 'post.date | date: "%Y"' %}
  {% for year in postsByYear %}
        {% for post in year.items %}
          {% include archive-single.html type=page.entries_layout %}
        {% endfor %}
  {% endfor %}






{% endfor %}
