---
layout: post
title:  "Getting Started with a blog"
date:   2018-03-29 12:17:22 +0530
categories: blog
---

Over the years i had experimented with a lot of technologies which was never documented anywhere nor shared anywhere. As time flew i even forgot the basic of these technologies.So this is a place for me to document the technologies i try out. Since this is my first attempt in writting blogs please do excuse the naive mistakes i am bound to produce

Road to Jekyll
--------------

So i come to the decision of making blogs, now the question is how the hell i make a blog? I have literally no clue as to where would i make a blog or how to host it? 

In my college days i have come across this amazing way to host static sites in gihub.io. So here i am having confusions on how to host a blog and i just had a thought why not use github.io to host the blog.
For this first i have brush up on Github.io which i did from the site https://guides.github.com/features/pages/ and there it was Jekyll which would produce basic template for the blog and sounded cool and here i am posting my first post.

Setting Up Jekyll
-----------------

**System Specs**
  - OS:    Ubuntu 16.04 LTS
  - RAM: 8GB

As jekyll needs ruby which i didn't have in the system i began the steps for the installation from there

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
