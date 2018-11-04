---
layout: default
<!-- title: Superhero.me -->
permalink: /blog/tags/blogposts
---

<div>
	<header class="post-header">
    	<h1>Free Posts</h1>
  </header>
	
	<p></p>
	
<h2>Collection of posts tagged with 'blog' : </h2>

	<ul class="posts">
    {% for post in site.categories.blog %}
      <li>
        <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </li>
    {% endfor %}
  </ul>

</div>
