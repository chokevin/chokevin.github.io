---
layout: default
title: Articles
permalink: /articles/
---

<section class="articles-page">
  <h1 class="articles-title">Articles</h1>
  <p class="articles-intro">All posts and notes from the blog.</p>

  {% if site.posts.size > 0 %}
  <div class="articles-list">
    {% for post in site.posts %}
    <article class="article-row">
      <p class="article-row-meta">
        <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time>
        {% if post.categories and post.categories.size > 0 %}
        · {{ post.categories | join: " · " }}
        {% endif %}
      </p>
      <h2 class="article-row-title"><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
      <p class="article-row-excerpt">{{ post.excerpt | strip_html | truncate: 220 }}</p>
      <a class="article-row-link" href="{{ post.url | relative_url }}">Read article →</a>
    </article>
    {% endfor %}
  </div>
  {% else %}
  <p class="meta">No articles yet.</p>
  {% endif %}
</section>
