---
layout: default
<!-- title: Superhero.me -->
# permalink: /games/superhero.me/
permalink: /games/infiniterunner/
---

<div>
	<header class="post-header">
    	<h1>Infinite-Runner</h1>
  	</header>

	<p>
	<div class="embed-responsive embed-responsive-16by9">
			<iframe width="560" height="315" src="https://www.youtube.com/embed/c_zaRy9eZYw" frameborder="0" allowfullscreen></iframe>
		</div>
	</p>


	<H4>System : IOS</H4>
	<H4>Release Date : Coming Soon</H4>

<h3>Posts</h3>

<h4>Nothing here yet...</h4>

	<ul class="posts">
    {% for post in site.categories.infiniterunner %}
      <li>
        <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </li>
    {% endfor %}
  	</ul>

</div>
