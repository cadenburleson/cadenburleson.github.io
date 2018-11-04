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
	<h2>COMING SOON!</h2>
	<p>
		Since Slamatron as a company is currently a one man team.
		This game is Slamatron's sole priority atm. All other Slamatron games will be developed after this game is finished.
	</p>
	<h3>System :</h3>
	<p>
		Set to release on all Apple Mobile devices.
	</p>
	<h3>Release Date :</h3>
	<p>
		Coming Soon!
	</p>

<h2>Posts : </h2>

	<ul class="posts">
    {% for post in site.categories.infiniterunner %}
      <li>
        <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </li>
    {% endfor %}
  	</ul>

</div>
