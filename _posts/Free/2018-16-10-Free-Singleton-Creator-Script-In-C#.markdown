---
layout: post
title:  "Free Singleton Creator Script in C#"
date: 2016-05-13
categories: [blog, free]
tags: [hot, summer]
---
<!--
You'll find this post in your `_posts` directory - edit this post and re-build (or run with the `-w` switch) to see your changes!
To add new posts, simply add a file in the `_posts` directory that follows the convention: YYYY-MM-DD-name-of-post.ext.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll's GitHub repo][jekyll-gh].

[jekyll-gh]: https://github.com/jekyll/jekyll
[jekyll]:    http://jekyllrb.com

-->

<p>
Here's the code :
</p>

<!-- <img
src = "http://localhost:4000/assets/screenshot.jpg"
alt = "my helpful screenshot"
style="width:300px;height:300px;"
/> -->

{% highlight c# %}

using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Singleton : MonoBehaviour {

	public static Singleton instance;

	public void Awake(){

		if (instance == null){
			instance = this;
			DontDestroyOnLoad(gameObject);
		}else{
			Destroy(gameObject);
		}

	}
}

{% endhighlight %}

<p>
	Attach this script to any object in your scene to have it persist between scenes as a singleton.
</p>
<p>
	This script helps you follow the MonoBehavior 'component' principal, where one script will do one simple task.
	This helps you manage code easier and find bugs faster.
</p>
