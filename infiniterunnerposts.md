---
layout: default
<!-- title: Superhero.me -->
# permalink: /games/superhero.me/
# permalink: /games/infiniterunner/
# permalink: /blog/tags/freeposts
permalink: /blog/tags/infiniterunnerposts
---

<div>
	<header class="post-header">
    	<h1>Free Posts</h1>
  </header>
	
	<p></p>
	
<h2>Collection of posts tagged with 'infiniterunner' : </h2>

	<ul class="posts">
    {% for post in site.categories.infiniterunner %}
      <li>
        <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </li>
    {% endfor %}
  </ul>

</div>
