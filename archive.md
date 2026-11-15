---
layout: default
title: Archive
description: An archive of writings by SV Chhangte.
permalink: /archive/
---

<section class="page-heading">
  <p class="eyebrow">THE WRITING</p>
  <h1>Archive</h1>
  <p class="page-intro">A collection of notes, essays, and reflections.</p>
</section>

{% assign visible_posts = site.posts | where_exp: "post", "post.hidden != true" %}
{% assign grouped_posts = visible_posts | group_by_exp: "post", "post.date | date: '%Y'" %}
{% for year in grouped_posts %}
  <section class="archive-year">
    <h2>{{ year.name }}</h2>
    <div class="post-list">
      {% for post in year.items %}
        <a href="{{ post.url | relative_url }}" style="text-decoration:none;"><article class="post-list-item compact">
          <div class="post-meta"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%b %-d" }}</time></div>
          <h3>{{ post.title | escape }}</h3>
        </article></a>
      {% endfor %}
    </div>
  </section>
{% else %}
  <p class="empty-state">No articles published yet.</p>
{% endfor %}
