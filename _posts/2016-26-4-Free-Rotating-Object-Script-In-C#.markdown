---
layout: post
title:  "Free Rotating Object Script in C#"
date: 2016-05-13
categories: jekyll update
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

  using UnityEngine;
  using System.Collections;

  public class RotatingObject : MonoBehaviour {

  	public float myRotationSpeed = 100.0f;

  	public bool isRotateX = false;
  	public bool isRotateY = false;
  	public bool isRotateZ = false;

  	// CHANGE TO ROTATE IN OPPOSITE DIRECTION
  	private bool positiveRotation = false;
  	private int posOrNeg = 1;

  	// Use this for initialization
  	void Start (){
  		collider.isTrigger = true;
  		if(positiveRotation == false){
  			posOrNeg = -1;
  		}
  	}

  	// Update is called once per frame
  	void Update (){
  		//  Toggles X Rotation
  		if(isRotateX){
  			transform.Rotate(myRotationSpeed * Time.deltaTime * posOrNeg, 0, 0);//rotates coin on X axis
  		}
  		//  Toggles Y Rotation
  		if(isRotateY){
  			transform.Rotate(0, myRotationSpeed * Time.deltaTime * posOrNeg, 0);//rotates coin on Y axis
  		}
  		//  Toggles Z Rotation
  		if(isRotateZ){
  			transform.Rotate(0, 0, myRotationSpeed * Time.deltaTime * posOrNeg);//rotates coin on Z axis
  		}
  	}

  }

  }
{% endhighlight %}

<p>
Here's a demonstration on how to use the script :
</p>

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/-ZujPUORn94" frameborder="0" allowfullscreen></iframe>
</p>
