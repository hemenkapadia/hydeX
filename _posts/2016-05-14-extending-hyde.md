---
layout: post
title: Extending Hyde, the start of hydeX development
excerpt: Introducing hydeX - the extended version of Hyde, a popular theme for Jekyll.
comments: true
tags: 
    - hydeX
    - Hyde
    - Jekyll
    - theme
---

I was looking to migrate my blog from [Blogger][1] to [GitHub Pages][2], which is based on [Jekyll][3]. While researching for a [Jekyll][3] theme to use for the blog I discovered [Hyde][4], an excellent theme made by [Mark Otto][5], the creator of [Bootstrap][6].

[Hyde][4] is a very minimalistic and responsive theme, designed with a mobile first approach. I felt it was pretty close to what I was looking for but somehow felt it was missing a persona I was looking for in my blog template. Not a problem, I thought and decided to try and get that persona myself. Instantaneously, I forked [Hyde][5] to my [GitHub repository][6], and started work on [hydeX][7], the Hyde eXtension.

When I started, I did not have a clear idea of the 'missing persona' I was looking for in the template. I had few pointers to start with (mentioned below) and then decided to iteratively work on it till I was satisfied.

I immediately started working on the below aspects

* I did not want the entire blog post on the main page. Instead, I was looking for a post listing. Adding an excerpt of the post below the blog title was something I wanted to experiment with.
* I also realized Hyde's Jekyll configuration file was not well organized nor did it exploit Jekyll's configuration and templating capability to its full potential. I wanted to drive all possible configurable aspects of hydeX via the Jekyll configuration file.
* I wanted to update the Typography to match the blog listing approach I planned to take. Moreover, I wanted to base the Typography on web fonts provided by [Google Fonts][8].
* I wanted the sidebar to be more impactful. Also, I wanted the [stickiness of sidebar content][9] to be controlled from the config file, without requiring any changes to the blog layout templates.
* Similarly, I also wanted the [blog color theme][10] to be controlled by the config file.

This was just the start and I was sure that I would add lot more features once I start working on the extended theme.

Thanks!


[1]: http://www.blogger.com
[2]: https://pages.github.com/
[3]: https://jekyllrb.com/
[4]: http://hyde.getpoole.com/
[5]: https://github.com/poole/hyde 
[6]: https://github.com/hemenkapadia?tab=repositories
[7]: https://hemenkapadia.github.io/hydeX/
[8]: https://fonts.google.com/
[9]: https://github.com/poole/hyde#sticky-sidebar-content
[10]: https://github.com/poole/hyde#themes





