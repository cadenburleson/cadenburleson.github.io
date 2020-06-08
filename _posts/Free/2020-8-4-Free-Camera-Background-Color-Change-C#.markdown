---
layout: post
title:  "Fade Camera Background Color Over Time in Unity C# (Free Script)"
date: 2020-06-8
categories: [blog, free]
# tags: [hot, summer]
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
<div>
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

public class FadeColor : MonoBehaviour
{
    private new Camera camera;
    [SerializeField] [Range(0f, 1f)] float lerpTime;
    [SerializeField] Color[] myColors;

    private int colorIndex = 0;
    private float t = 0f;
    private int len;

    private void Start()
    {
        camera = GetComponent<Camera>();
        len = myColors.Length;
    }

    private void Update()
    {
        camera.backgroundColor = Color.Lerp(camera.backgroundColor, myColors[colorIndex], lerpTime * Time.deltaTime);

        t = Mathf.Lerp(t, 1f, lerpTime * Time.deltaTime);
        if (t > 0.9f)
        {
            t = 0f;
            colorIndex++;
            colorIndex = (colorIndex >= len ? 0 : colorIndex);
        }
    }

}

{% endhighlight %}

<H4>The Component</H4>
<img src="/assets/FadeColorComponent.png" alt="FadeColorComponent" style="width:400px; height:300px;">

<p>
Demo Video on how to use this script coming soon!
In the meantime watch a video by : Hamza Herbou that inspired this script.
</p>

<div class="embed-responsive embed-responsive-16by9">
	<iframe width="560" height="315, initial-scale=1" src="https://www.youtube.com/embed/C_f2ChrcSSM" frameborder="0" allowfullscreen></iframe>
    <!-- <iframe width="560" height="315" src="https://www.youtube.com/embed/C_f2ChrcSSM" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> -->
</div>

</div>
