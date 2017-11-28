---
layout: post
title: Extending Hyde, the start of hydeX development
excerpt: I start development on hydeX, the extended version of Hyde, with an initial set of enhancements, adding more as we go along.
comments: true
tags: 
    - hydeX
    - Hyde
    - Jekyll
    - theme
---

I am looking to migrate my blog from [Blogger][1] to [Jekyll][3] based [GitHub Pages][2]. While researching for a [Jekyll][3] theme to use for the blog I discovered [Hyde][4], an excellent theme made by [Mark Otto][5], the creator of [Bootstrap][6].

[Hyde][4] is a minimalistic and responsive theme, designed with a mobile first approach. It is close to what I am looking for but somehow it feels lacking a persona I want in my blog template. Not a problem, I thought and decided to try and implement that persona myself. Instantaneously, I forked [Hyde][5] to my [GitHub repository][6], and started work on [hydeX][7], the Hyde eXtension.

I do not have a crystal clear idea of the 'missing persona' I am looking for in the template. I am starting with the below-mentioned pointers and will iteratively add more features until I am satisfied.

* Change blog's main page to display the post listing instead of the full post. Experiment with an option to display the post excerpt below the post listing.
* Update Typography to match the blog listing design I envision. Base the Typography on web fonts provided by [Google Fonts][8].
* Make the sidebar more impactful. Replace text links with [Font Awesome][11] icons.
* Improve Hyde's Jekyll configuration file organization. Add additional parameters to control the template experience, which currently requires code changes in the template.
    * [stickiness of sidebar content][9] 
    * [blog color theme][10]


This is just the start, would be interesting to see what the final version turns out to be.

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
[11]: http://fontawesome.io/





