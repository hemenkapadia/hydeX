---
layout: post
title: Community engagement using Disqus 
excerpt: Enable community engagement by integrating Disqus to your blog powered by hydeX. 
comments: true
tags:
  - hydeX
  - Features
  - Disqus 
  - Community Engagement
---

> Communication is a two way street.

[Jekyll][1], out of the box, does not provide capability to capture reader comments for your blog. A blog without capability to foster interaction within the reader community is merely a 'monologue'. An engaged and active reader community is critical for the success of your blog.

[hydeX][2] enables this capability by providing integration with [Disqus][3]. [Disqus][3] is trusted by millions of publishers to engage their audience, retain readers and monetize their engagement.

Enabling Disqus on hydeX is extremely simple. As a first step, you will need to [Register with Disqus][4]. As part of the registration process, you will need to pick a short name for your website. 

![Disqus Registration](/hydeX/assets/images/disqus-register.png)

Once you have the short name for your hydeX based website, all you are required to do is update the same in the configuration file. I provide the below stub in the configuration file. The parameter to be updated is `disqus_src, where `example.disqus.com` be replaced by the short name you created. 

```yaml
# Comments - Disqus Configuration
disqus_enable:                  true 
disqus_src:                     example.disqus.com     # replace this
```
This is the bare minimum configuration needed to get this working. You should now see Disqus panel show up below the [Related Posts][5] section of the blog post.

![Comments powered by Disqus](/hydeX/assets/images/disqus-comments.png)

In case you want to disable Disqus across the entire site then you can change `disqus_enable` to `false` in `_config.yml`. There is also an option to disable comments on a single post. In the post's YAML front matter, change the value of the `comment` property from `true` to `false`. This will cause Disqus comments to be disabled on that post only.

You should not need any additional configuration, however, you can still refer to the [Disqus Installation 101][6] in case such a need arises.


[1]: https://jekyllrb.com/
[2]: https://hemenkapadia.github.io/hydeX/
[3]: https://disqus.com/
[4]: https://disqus.com/profile/signup/
[5]: /hydeX/blog/2016/03/23/tags.html
[6]: https://help.disqus.com/customer/en/portal/articles/1259853-installation-101

