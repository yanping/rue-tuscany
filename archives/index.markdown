---
layout  : name2
title   : Blog
section : Past
feed    : /atom.xml
---

Blog Posts
==========

This is the complete archive of posts at *[Rue Tuscany](/)* in reverse chronological order.

{% assign year = "none" %}
{% assign month = "none" %}

{% for post in site.posts %}
{% capture curryear %}{{post.date | date:'%Y'}}{% endcapture %}
{% capture currmonth %}{{post.date | date:'%Y-%m'}}{% endcapture %}
<div class="section list">
  <h1>{% if currmonth != month %}<a name="{{ currmonth }}">{% endif %}
	{% if curryear != year %}<a name="{{ curryear }}">{% endif %}
	{{ post.date | date_to_string }}
	{% if currmonth != month %}</a>{% endif %}
	{% if curryear != year %}</a>{% endif %}
  </h1>
  <p class="line">
    <a class="title" href="{{ post.url }}">{{ post.title }}</a>
    <a class="comments" href="{{ post.url }}#disqus_thread">View Comments</a>
  </p>
  <p class="excerpt">{% if post.excerpt %}
	{{ post.excerpt }}
  {% else %}
    {{ post.content | html_truncate }}
  {% endif %}</p>
</div>
{% assign year = curryear %}{% assign month = currmonth %}{% endfor %}

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


