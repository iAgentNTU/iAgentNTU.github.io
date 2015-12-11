---
layout: page
title: Research
header: true
permalink: /research/
---

<div class="home">

  <h1 class="page-heading">Posts</h1>

  <ul class="news-list">
    {% for news in site.news %}
      <li>
        <span class="news-meta">{{ news.date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="news-link" href="{{ news.url | prepend: site.baseurl }}">{{ news.title }}</a>
        </h2>
      </li>
    {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

</div>
