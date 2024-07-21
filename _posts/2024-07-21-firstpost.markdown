---
layout: post
title:  "A Jekyll Quickstart Tutorial"
date:   2024-07-21 12:39:36 -0500
categories: jekyll
---

The first of (hopefully) many posts where I record the new things I learn. I figured that this website is probably a good place to start.

I made this site using [Jekyll](https://jekyllrb.com/docs/), a static site generator that takes your markup content and transforms it into a website. If you're like me and don't really like to spend much time on CSS and HTML, but need a website for maintaining a portfolio or a blog, this is a perfect fit. Jekyll is supported by Github pages and there is a lot of [documentation](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll) on Github for setting up a website with Jekyll's [Minima theme](https://github.com/jekyll/minima/tree/master), which is great. However, Github Pages has not updated the version of Jekyll and Minima that it uses, leading to some issues that will be the focus of this post.

### Man, I just want dark mode
![I just want darkmode man](/img/2024_0721/gh_darkskin.png)

You'll quickly find that if you followed Github's documentation to a T, getting darkmode onto your website is not as straight forward as it looks. Choosing between multiple skins is not supported on the latest version of Minima supported by Github pages. 

The solution I found was to add in the latest version of Minima as a [remote theme](https://github.com/benbalter/jekyll-remote-theme). This lets you use all the latest functionality of Minima, as in the github repo online. One warning though, is that this will slightly alter your default page layout from the starter code. For one, the footer layout changes noticeably. I personally prefer the older footer layout, but it's not a big deal as I can just customize the template, which I cover later in this post.

There will also be noticeable variation between the documentation suggested by Github, and the Minima repo documentation. For example, when adding social media links, the default syntax is something like {% highlight ruby %}
github_username: jekyll/jekyll
{% endhighlight %} Whereas on the latest version, the correct syntax is 

{% highlight ruby %}
minima:
  social_links:
    - { platform: github,  user_url: "https://github.com/jekyll/jekyll" }
{% endhighlight %}

Personally I prefer the remote theme as this lets me follow the documentation in the Minima repo, which is more extensive.

### Testing Locally

You should be [testing your site locally](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll?platform=linux) instead of uploading it and waiting 2 minutes to see if the changes you made reflected as intended or not. Sometimes, you might run into the issue of the local server still running, even when you hit `Ctrl-C` to end the local instance.

![](/img/2024_0721/portinusess.png)

The quick fix is to manually kill the previous process, specifically whichever process is still connected to the default port used by Jekyll to locally host your website.

{% highlight ruby %}
$ sudo fuser -k 4000/tcp
{% endhighlight %}

### Customizing your site

If you don't like something in the default template (you prefer the older version of the footer, or you wish to [remove the `subscribe RSS` button](https://github.com/jekyll/minima/issues/553)), you can always change it relatively easily. You have to find the original file in the repository that contains the CSS/HTML description for that element, copy the file into your own repository while making sure to keep the same relative file path, and make your changes accordingly. For example I have a `/_includes/footer.html` file in my repository in order to customize my footer from the default template.

While this means we can't avoid delving into some HTML/CSS, less is better than too much.

![text](/img/2024_0721/css.png)
*[Source](https://i.imgur.com/ajiIIq3.jpg)*

### That's it folks

Till next time. Thanks for reading!






