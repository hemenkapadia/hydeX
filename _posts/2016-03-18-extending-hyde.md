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

I was looking to migrate my blog from [Blogger][1] to [Jekyll][3] based [GitHub Pages][2]. While researching for a [Jekyll][3] theme to use for the blog I discovered [Hyde][4], an excellent theme made by [Mark Otto][5], the creator of [Bootstrap][6].

[Hyde][4] is a minimalistic and responsive theme, designed with a mobile first approach. It was close to what I was looking for but somehow felt it was missing a persona I wanted in my blog template. Not a problem, I thought, and decided to try and implement that persona myself. Instantaneously, I forked [Hyde][5] to my [GitHub repository][6], and started work on [hydeX][7], the Hyde eXtension.

When I started, I did not have a clear idea of the 'missing persona' I was looking for in the template. I had few pointers to start with (mentioned below) and then decided to iteratively work on it till I was satisfied.

I started working on the below aspects

* Changing blog's main page to display the post listing instead of the full post. Experimenting with an option to display the post excerpt below the post listing.
* Improving Hyde's Jekyll configuration file. Making it more organized and adding additional parameters to control the template experience. 
* Updating the Typography to match the blog listing design I finalized. I also decided to base the Typography on web fonts provided by [Google Fonts][8].
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





