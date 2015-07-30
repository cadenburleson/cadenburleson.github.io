---
layout: page
title: Blog
permalink: blog/
---

<!-- <div class="page-content">

<!-- Trailer For Spinball
	<iframe width="560" height="315" src="//www.youtube.com/embed/_xe3Q6DTj8s?list=UU7FK4Y_Eu4Cwf3uATBHj09A" frameborder="0" allowfullscreen></iframe>

	<p><h5>Current Version:</h5>1.0</p>

</div>

 -->

<div class="home">

  <h1>Posts</h1>

  <ul class="posts">
    {% for post in site.posts %}
      <li>
        <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </li>
    {% endfor %}
  </ul>

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

</div>