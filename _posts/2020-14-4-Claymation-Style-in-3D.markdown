---
layout: post
title:  "Claymation Style in 3D"
date: 2020-04-16
categories: [blog,]
# tags: [hot, summer]
---

<H3>Intro</H3>
<p>
I've always been interested in the claymation/stopmotion look ever since I was a kid. I would watch movies such as
<a href="https://www.wallaceandgromit.com/">Wallace and Grommit</a> in the car during long road-trips. Way back when, when flash games were a thing, there was a website similar
to today's youtube where I would watch all sorts of indie claymation films and play crazy flash games when flash was still alive... This website some of you might have heard of before;
It's called <a href="https://www.newgrounds.com/">NewGrounds</a>. I have some good memories from there. There were a few animations and games that really stuck in my memory though.
<a href="https://www.youtube.com/watch?v=jwFivfiLxQY">DoodieMan</a> being one of them. It's about a superhero, who's super-power is the ability to poop on command... I'll let you watch the video instead of getting into
the details of that shit.

<p>
Butt... onto the flash games that I used to play that I suppose had a big influence on my life since I got into making games years later. The flash game was one by
<a href="https://joecartoon.com/">JoeCartoon</a> Where there's a shit-talking frog stuck in a blender(funny bc now the 3D program I use), slowly spinning around and your job is to taunt him by slowly pressing the buttons of the blender
increasing the taunts and threats from the frog until eventually the frog goes Bye-Bye. I was a young child at the time so gore for me was some-what taboo so it made it even more interesting. -don't ask me why I like to play Gears of War now...
</p>

<p>
You might be asking yourself what any of that has to do with claymation, well it doesn't! But thinking about claymation got me cruisin' down memory lane on how those early animations and flash games really
set the stage for my future in Art, Animation, and GameDevelopment.
</p>

</p>

<p>
The way the characters have subtle jitters and movements in the clay where the animators
positioned the character differently from the last frame, the squash and stretch of the
clay bringing immense life into an inanimate objects that you can't necessarily get with traditional 3D animation.
</p>

<H3>Claymation Is Expensive</H3>
<p>
To make a claymation you need a lot of resources.
You have to have a decent camera to take the single framed shots of your clay characters. And although I do own a Canon t2i and a tripod, there's other resources that I couldn't afford.

You will have to build sets (scenes) for your characters to be animated in. These sets can be made from an assortment of goods from balsawood, cardboards, to foamboard and more.
You can really build the sets out of anything. Although depending on how long you want your film to be and how many different scenes you want, this can end up being quite expensive.
Then even after you've built your scenes you still need to light those scenes, and the lights aren't cheap either.

Once you've got your camera, your scenes & props, and lighting setup, you'll obviously need some Characters which guess what? Are made from clay!
The characters have metal bones which are made from twisting wire together into a skeletal system called an armature. Once you have your armature built, you then mould the clay
around the armature to create the form of your character.
Now It seems like you are finally ready to start filming.
-Did I tell you that to make a single second of film for a stop-motion film you are going to have to take 24 pictures on your camera?
That's 1,440 pictures for a single minute of film.
So it's also very time consuming making a stop motion film and you have to buy a lot of resources, So I set out to figure out how to make the process faster & cheaper.

<H3>Claymation Style on a Budget</H3>
I noticed while doing 3D work that people would sculpt their characters with a clay looking matcap on their model. I figured if they are able to do this live while sculpting, then
the effect could only be recreated and improved upon in a full render. So I set out to find a way to achieve a good looking claymation style in 3D.
That's when I came upon <a href="https://mindbender.com/#/home"> Meindbender Animation Studio</a> work. They have a lot of very cool and inspiring work that looks very claymation esc.
A lot of what makes meindbender so amazing are their very <a href="https://vimeo.com/278691057"> complex rigs</a> for their characters.

I tried to make a similar rig or atleast incorporate some aspects of their rig in <a href="https://www.blender.org/"> Blender</a> (A free 3D program) You can find my test <a href="https://youtu.be/g2VJK93KcHs"> here</a>. I wanted the face to stretch out with the eye-ball to mimic that the clay-material was being pulled with the eye. I did this with a Cast modifier at first, but this wasn't giving me the fidelity I wanted and was hard to predict/control. I then later found that the hook modifier was a better choice and that with the hook modifier I could select a specific amount of vetices on the face that would be controlled by an empty object and that the hook modifier had a strength attribute that I could change depending on how severe I wanted to make the control. With the hook modifier you are even able to weight paint the vertex group that the empty controls for even finer control.
</p>

<p>
Now you might be wondering what is that clay looking material I am using in Blender? It's a downloadable shader made by DoubleGum with tons of features which you can download <a href="https://blendermarket.com/products/claydoh"> here</a>. It is well worth the money as it has tons of controls which you can change in the shader editor. It even has an automatic texture movement when you animate that mimics the movement of fingerprints and claymovement as it would if you were moulding the clay every frame. If you can't afford this though, then don't fret. There's a nice blog post <a href="https://blenderartists.org/t/realistic-clay-material-in-cycles/576258"> here</a> that will show you how to create a basic clay material from scratch.
</p>

<H3>Claymation in games</H3>
<p>
I've also tried to make claymation for games as well. I made some bones in my characters feet that would mimic the squashing effect of clay which you can see <a href="https://www.facebook.com/Slamatron/videos/1849785161972836/"> here</a>. I was looking into how to get the clay-mation type material in Unity3D as well, but the version of Unity I was using at the time didn't have PBR materials so everything looked very bad. I'm sure if you wanted to do it now It'd be a lot easier specially with Unity's HDRP and the shader graph. I will definately update this post if I get something working in Engine.
</p>

<p>
I'm hoping that this post has been somewhat informative for you or atleast beneficial in helping you achieve a claymation style in 3D. If not I'm hoping that you at least found a nice assortment of resources in this post to aid you.
</p>

<p>
I will be updating this post more and more as I find out new techniques to achieve the claymation/stop-motion style/look in Blender. Please contact us using the email in the footer if you have any insight to help. Thank you!
</p>



<!-- <h2>Clay Experiments 1</h2> -->

<h3>Resources:</h3>

<a href="https://blenderartists.org/t/realistic-clay-material-in-cycles/576258">(Tutorial) Basic Blender Clay Material</a>

<a href="https://www.pedroconti.com/"> (Website) Pedro Conti</a>

<a href="http://olovburman.com/"> (Website) Olav Burman</a>

<a href="https://nki.tv/#!/fr/works/">(Animation Company) NKI </a>

<a href="https://www.youtube.com/user/PatrickBoivin/videos">(Stop-Motion Animator) Patrick Boivin</a>

<a href="https://www.youtube.com/user/leehardcastle/videos">(Stop-Motion Animator) Lee Hardcastle</a>

<a href="https://blendermarket.com/products/claydoh">(Purchasable) Advanced Blender Clay Material - By : DoubleGum</a>

<a href="https://www.youtube.com/channel/UCOWrbryuVEPUMSSgayuLURg">(Videos) SouthernShotty youtube channel has videos about creating claymation type visuals in Blender</a>

<a href="https://www.cgbookcase.com/textures/fingerprints-01">(Texture) HD Fingerprint texture - 1k, 2k, and 3k rez</a>

<a href="http://www.williamchild.co.uk/">(Website) William Child Films - Makes music videos/commercials in claymation style</a>






<p>Here's the code :</p>

{% highlight c# %}
	NO CODE TO SHOW HERE.
	JUST A TEST!
{% endhighlight %}

<p></p>
<p></p>
