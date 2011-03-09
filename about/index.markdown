---
layout  : name
title   : About
section : About
feed    : /atom.xml
---

About this Site
===============
Thank you for visiting. More information about this site's mechanics or colophon can be found at my [first blog post](/website/first-post.html), as well as at the [update](/website/starting-over.html) for changes so far. The header of this site may appear funny :-). I don't have much experience in CCS and web design, but it's always my hope to add a little touch of originality to the adapted layout. The original site template and CCS design credit goes to [Mark Reid] (http://mark.reid.name).

See the source of this blog at [github](https://github.com/leecarrot/rue-tuscany). Below is an example of the workflow. Assume git has been initialized in the working directory with: `$ git init`, and a heroku application has been created by running: `$ heroku create`. [More...](http://devcenter.heroku.com/articles/quickstart) 

	$ cd rue-tuscany
	$ gedit _posts/2011-02-28-post-title.markdown
	$ jekyll --server --auto --pygments
	$ git add _posts
	$ git commit -m "add new post post title"
	$ git push -u origin
	$ git push heroku
	$ heroku open

The second last command basically pushes updates to Heroku after the initial push of Heroku application (first step: `$ git push ... master`). In the above example, both push to Github and Heroku. It's not necessary to push to Github. The push was only meant to share the structure of the code. To test if the site has been hosted properly on Heroku, the last command will open the address of Heroku application. The Heroku application will reflect the actual site.

A Little About Me
=================
I am a 28 years old graduate student studying computer science at the University of Ottawa, Canada. I created this site with the intention of becoming a more productive outlet for sharing and learning. I was born and grew up in Indonesia. I am currently working towards completion of my master thesis, focusing on Privacy Preserving Data Mining and Privacy in Data Publishing.  

From the outset, I have always wondered how to find balance between the things I do and the person I would love to become. I believe there is so much to learn from every encounter in this life, regardless of the duration they last. As soon as one door closes, another door opens. It may seem so much easier to embrace security by staying at the same place at times. But understanding the very essence of our individuality requires the courage to step outside one's comfort zone, because the method we know won't always work out in every situation, and we will eventually recognize our inner strength by repeatedly trying. This learning journey has always been a challenge to me.

The same people will not always be there for us. Our good times with them are synonymous to oil floating on the surface of an open sea, while the not-so-good moments can be thought as rocks drowning to the bottom of the sea. When they are no longer with us, we can still feel their presence and remember fondly their impact in our life. I can say I have grown to be self-sufficient, within the comfort of a teddy bear companion in her twenties, hot tea, sweet potatoes, herbal oil, the Book of Change and a new appreciation of the Milky Way.

Anyone can get in touch with me by leaving comments, feedback [@jliyi](http://twitter.com/jliyi), or through leecarrot@gmail.com.
