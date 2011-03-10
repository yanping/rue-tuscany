---
layout  : name
title   : Blog
section : Past
---

<div class="category">
<span class="cat">
    <a href="/well-being.html">well-being ({{ site.categories.well-being | size }})</a>
    <a href="/random.html">random ({{ site.categories.random | size }})</a>     
    <a href="/website.html">website ({{ site.categories.website | size }})</a>
    <a href="/privacy.html">privacy ({{ site.categories.privacy | size }})</a>
    <!--a href="/books.html">books ({{ site.categories.books | size }})</a>
    <a href="/facts.html">facts ({{ site.categories.facts | size }})</a>
    <a href="/astrology.html">astrology ({{ site.categories.astrology | size }})</a-->
</span>
</div>

Blog Posts
==========

{% for post in site.posts %}
<div class="section list">
  <h1>{{ post.date | date_to_string }}</h1>
  <p class="line">
    <a class="title" href="{{ post.url }}">&raquo; {{ post.title }}</a>
    <a class="comments" href="{{ post.url }}#disqus_thread">View Comments</a>
  </p>
  <p class="excerpt">{% if post.excerpt %}
	{{ post.excerpt }}
  {% else %}
    {{ post.content | html_truncate }}
  {% endif %}</p>
</div>
{% endfor %}

<script type="text/javascript">
    /* * * CONFIGURATION VARIABLES: EDIT BEFORE PASTING INTO YOUR WEBPAGE * * */
    var disqus_shortname = 'rosebery'; // required: replace example with your forum shortname

    /* * * DON'T EDIT BELOW THIS LINE * * */
    (function () {
        var s = document.createElement('script'); s.async = true;
        s.type = 'text/javascript';
        s.src = 'http://' + disqus_shortname + '.disqus.com/count.js';
        (document.getElementsByTagName('HEAD')[0] || document.getElementsByTagName('BODY')[0]).appendChild(s);
    }());
</script>
