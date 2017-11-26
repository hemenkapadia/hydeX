---
layout: post
title: Engage your blog's audience by enabling community discussions
excerpt: hydeX provides built-in integration with Disqus, enabling your audience to comment on your blog posts as well as interact as a community. 
comments: true
tags:
  - Features
  - Disqus 
  - Community Engagement
  - hydeX
---

> Communication is a two way street.

An engaged and active reader community is critical for the success of your blog.  A blog where the audience cannot share their views on the topic, is merely a 'monologue'. 

[Jekyll][1], out of the box, does not provide capability to capture reader comments for your blog. [hydeX][2] enables this capability by providing integration with [Disqus][3]. [Disqus][3] is trusted by millions of publishers to engage their audience, retain readers and monetize their engagement.

Integrating your blog, based on [hydeX][2], with [Disqus][3] is extremely simple. Follow the steps outlined below. 

### Create a new Disqus site

As a first step, you will need to [Register with Disqus][4]. As part of the registration process, you will proceed to [Create a new Disqus Site][7]. 

Based on the Website Name you share while [creating a new site][7], Disqus will generate a unique Disqus URL for your website. You can see that the unique Disqus URL generated in the below screen-shot is `my-amazing-blog.disqus.com`. Make note of this URL, you will need it later to configure hydeX for your blog.

![Disqus Registration](/hydeX/assets/images/disqus-register.png)

### Integrate hydeX with Disqus

Once you have the unique Disqus URL for your hydeX based website/blog, you need to update the same in hydeX configuration file. 

In the `Disqus configuration` section, update the parameter `disqus_src` to the value of the unique Disqus URL you created above. 

```yaml
# Disqus Configuration
disqus_enable:                  true 
disqus_src:                     my-amazing-blog.disqus.com   # update this line
```
That's it! This is the absolute minimum configuration required to get Disqus integrated with your hydeX based blog. 

Once you publish the above configuration changes, Disqus comments will show up below the [Related Posts][5] section of the blog post, provided the Jekyll Environment is `production`.

![Comments powered by Disqus](/hydeX/assets/images/disqus-comments.png)

### Jekyll Environments

In case you are composing your posts locally and reviewing them in a local [Jekyll environment][10] before you publish it, you will notice that comments do not load in your local environment. Instead you get a message as below

![Comments enabled only in Production](/hydeX/assets/images/comments-production.png)

This is expected behavior as hydeX enables comments only in production environment. Once you publish the post on [GitHub Pages][9], comments will load as expected. [GitHub Pages][9] sets the value for `JEKYLL_ENV` environment variable to `production` enabling comments in your published blog.

I strongly recommend reading about [Jekyll Environments][10] if you are interested to know more about this.

### Additional Configuration parameters

While hydeX makes it simple to enable audience interaction on your blog, there can be moments where you may want to disable this feature temporarily across your entire blog, or on specific posts.

To temporarily disable Disqus across the entire site, but still keep the integration intact, change `disqus_enable` to `false` in `Disqus Configuration` section of `_config.yml`. 

To disable comments on a single post change the value of `comment` property, in the post's [YAML front matter][8], from `true` to `false`. Publish your post once again.

You should not need any additional configuration, however, you can still refer to the [Disqus Installation 101][6] in case such a need arises.


[1]: https://jekyllrb.com/
[2]: https://hemenkapadia.github.io/hydeX/
[3]: https://disqus.com/
[4]: https://disqus.com/profile/signup/
[5]: /hydeX/blog/2016/03/23/tags.html
[6]: https://help.disqus.com/customer/en/portal/articles/1259853-installation-101
[7]: https://disqus.com/admin/create/
[8]: https://jekyllrb.com/docs/frontmatter/
[9]: https://pages.github.com/
[10]: http://www.petethompson.net/blog/web/2015/02/28/environments-in-jekyll/