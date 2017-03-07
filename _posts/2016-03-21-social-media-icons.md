---
layout: post
title: Social Media icons in Sidebar Menu
excerpt: Linking hydeX to your social media profiles is a simple modification to Jekyll's configuration file. This post explains how easy it is to enable various social media icons in the sidebar menu. 
comments: true
tags:
  - hydeX
  - Features
  - Social Media
  - Sidebar Menu
---

hydeX provides capability to easily link to one's profile on multiple social media platforms. The link shows up as [Font Awesome icon][1] in the sidebar menu.

hydeX enables social media integration in the `author` section of Jekyll configuration file.

```yaml
# Author information
author:
  name:                         "Hemen Kapadia"
  email:                        hemen.kapadia@gmail.com
  twitter:                      null
  github:                       hemenkapadia
  linkedin:                     kapadiahemen
  facebook:                     null
  instagram:                    null
  googleplus:                   null
  youtube:                      null
  stackoverflow:                null
```

Atom feed for hydeX is enabled by default. Integration with social media platforms listed above are supported. 

 A value of `null` causes the corresponding social media icon to be hidden. To determine configuration value for a social media platform

1. Navigate to your profile page on the supported social media platform.
2. Compare your profile page url with the profile page url pattern mentioned below.
3. Identify the value on your profile page that matches with `{{ site.author.platform }}` in the sample urls.
4. Update the config file with the determined value.

```
# Profile Page URL pattern

twitter:           https://twitter.com/{{ "{{ site.author.twitter " }}}}
github:            https://github.com/{{ "{{ site.author.github " }}}}
linkedin:          https://www.linkedin.com/in/{{ "{{ site.author.linkedin " }}}}
facebook:          https://www.facebook.com/{{ "{{ site.author.facebook " }}}}
instagram:         https://www.instagram.com/{{ "{{ site.author.instagram " }}}}
googleplus:        https://plus.google.com/{{ "{{ site.author.googleplus " }}}}
youtube:           https://www.youtube.com/user/{{ "{{ site.author.youtube " }}}}
stackoverflow:     http://stackoverflow.com/users/{{ "{{ site.author.stackoverflow " }}}}
```

In the above configuration I have enabled `email`, `github` and `linkedin` integrations for which the icons show up as below for the desktop and responsive mobile interfaces

![Social Media icons - desktop interface](/hydeX/assets/images/followme-desktop2.png)

On the responsive mobile interface, the sidebar menu changes to the top navigation menu which includes page navigation and social media links.

![Social Media icons - mobile interface](/hydeX/assets/images/followme-mobile2.png)


[1]: http://fontawesome.io/