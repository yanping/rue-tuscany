---
layout  : name
title   : Home
section : Home
feed    : /atom.xml
---

<img class='inset right' src='/images/dandelion.jpg' title='Train of Thoughts to Tuscany' alt='ruetuscany' width='220px' />

Thank you for visiting. I am a graduate student in my late 20s studying computer science in Ottawa, Canada. I created this site with the intention of becoming a more productive outlet for sharing and learning. I was born and grew up in Indonesia. I am currently working towards completion of my master thesis, focusing on Privacy Preserving Data Mining and Privacy in Data Publishing.  

From the outset, I have always wondered how to find balance between the things I do and the person I would love to become. I believe there is so much to learn from every encounter in this life, regardless of the duration they last. As soon as one door closes, another door opens. It may seem so much easier to embrace security by staying at the same place at times. But understanding the very essence of our individuality requires the courage to step outside one's comfort zone, because the method we know won't always work out in every situation, and we will eventually recognize our inner strength by repeatedly trying. This learning journey has always been a challenge to me.

The same people will not always be there for us. Our good times with them can be likened to oil floating on the surface of an open sea, while the things they do, but do not meet our expectations can be likened to rocks drowning steadily to the bottom of the sea. When they are no longer with us, we can still feel their presence and remember fondly their impact in our life. I can say I have grown to be self-sufficient, within the comfort of a teddy bear companion in her twenties, hot tea, sweet potatoes, herbal oil, the Book of Change and a new appreciation of the Milky Way.


+-- {.section}
Most Recent Entries 
===================

{% for post in site.posts limit:3 %}
<div class="section list">
  <h1>{{ post.date | date_to_string }}</h1>
  <p class="line">
    <a class="title" href="{{ post.url }}">{{ post.title }}</a>
  </p>
  <p class="excerpt">
	{% if post.excerpt %}
	  {{ post.excerpt }}
    {% else %}
      {{ post.content | html_truncate }}
    {% endif %}
  </p>
</div>
{% endfor %}

<p>
<a href="/archives/">Older Posts &rarr;</a>
</p>
=--

