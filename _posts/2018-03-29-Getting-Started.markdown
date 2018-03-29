---
layout: post
title:  "Getting Started with a blog"
date:   2018-03-29 12:17:22 +0530
categories: blog
---

Over the years i had experimented with a lot of technologies which were never documented anywhere nor shared anywhere. As time flew i even forgot the basic of these technologies.So this is a place for me to document the technologies i try out. Since this is my first attempt in writting blogs please do excuse the naive mistakes i am bound to produce

Road to Jekyll
--------------

So, as I came to the decision of making blogs, now the question was how the hell do I make a blog and wondering about it bought a thought to my mind my mind why not just use Github pages to host the site. 

I was introduced to Github pages during my college days. Then I had no clue that Github could be used to host static pages. One of my classmates showed me that such a marvel is possible. Idea was soo simple and truly amazing. 

To host in Github.io i first had to get clear with the idea for that i started looking into https://guides.github.com/features/pages/. So now the next step was to put up a site where i could post with ease. One of my collegues here had already made me aware of Jekyll which provides the ease of posting which i was searching for and here I am posting my first post.

Setting Up Jekyll
-----------------

**System Specs**
  - OS:    Ubuntu 16.04 LTS
  - RAM: 8GB

As jekyll needs ruby which i didn't have in the system I began the steps for the installation from there

{% highlight bash %}
  sudo apt-get install ruby-full
  gem install jekyll
  jekyll new my-blog
  # Produced warning Could not load Bundler. Bundle install skipped.
  # Then i realized we need something called bundler which i installed with the below commands
  bundle exec jekyll serve
  gem install bundler
  rm -rf my-blog
  jekyll new my-blog
  # That created the blog
{% endhighlight %}
