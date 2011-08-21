---
layout  : name
title   : About
section : About
---

About this Site
===============
Thank you for visiting. See the source of this blog at [github](https://github.com/leecarrot/rue-tuscany). Below is an example of the workflow. Assume git has been initialized in the working directory with: `$ git init`, and a heroku application has been created by running: `$ heroku create`. [More detailed steps can be found here.](http://devcenter.heroku.com/articles/quickstart) 

	$ cd rue-tuscany
	$ gedit _posts/2011-02-28-post-title.markdown
	$ jekyll --server --auto --pygments
	$ git add _posts
	$ git commit -m "add new post post title"
	$ git push -u origin
	$ git push heroku
	$ heroku open

The second last command basically pushes updates to Heroku after the initial push of Heroku application (first step: `$ git push ... master`). In the above example, both push to Github and Heroku. It's not necessary to push to Github. The push was only meant to share the structure of the code. To test if the site has been hosted properly on Heroku, the last command will open the address of Heroku application. The Heroku application will reflect the actual site.

More information about this site's mechanics or colophon can be found at my [first blog post](/website/first-post.html). The site template is adapted from [Mark Reid] (http://mark.reid.name).

A Little About Me
=================

I am a graduate student studying computer science at the University of Ottawa, Canada. I created this site with the intention of becoming a more productive outlet for sharing and learning. I was born and grew up in Indonesia. I am currently working towards completion of my master thesis, focusing on Privacy Preserving Data Mining and Privacy in Data Publishing. It's a constant learning journey to become self-sufficient, live without expectation within the comfort of a teddy bear companion in her twenties, good music, and the Book of Change.
