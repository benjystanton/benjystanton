---
layout: page
title: Blog
permalink: /blog/
---

  <p class="margin-bottom--m"><a href="category">View all categories →</a></p>

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
        <span class="post-meta">{{ post.date | date: "%d %b %Y" }}</span>

      </li>
    {% endfor %}
  </ul>

  <p class="margin-top--m"><a href="{{ "/feed.xml" | prepend: site.baseurl }}">Subscribe via RSS</a></p>