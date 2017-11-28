---
layout: post
title: Link your Social Media profiles from the Sidebar Menu
excerpt: Link hydeX to social media profiles through simple modifications to hydeX Jekyll configuration file.
comments: true
tags:
  - hydeX
  - Features
  - Social Media
  - Sidebar Menu
---

hydeX provides the capability to easily link to your profile on multiple social media platforms. The links show up as [Font Awesome icons][1] in the sidebar menu.

To enable integration with social media platforms update the `author` section of hydeX's Jekyll configuration file. Currently, the below-listed platforms are supported. Atom feed for hydeX is enabled by default. 

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

`null` configuration value causes the corresponding social media icon to be hidden in the sidebar menu. Any value other than `null` will be used to create the link to your profile page on the corresponding social media platform as explained below.

1. Navigate to your profile page on the supported social media platform.
2. Compare your profile page URL with the profile page URL pattern mentioned below.
3. Identify the value on your profile page that matches with `{{ site.author.platform }}` in the sample URLs.
4. Update the config file with the determined value.

```yaml
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
In the sample configuration at the start of this post, I have enabled `email`, `github` and `linkedin` integrations for which the icons show up as below for the desktop and responsive mobile interfaces

<img src="/hydeX/assets/images/followme-desktop2.png" alt="Desktop interface showing Social Media icons" height="399px" width="340px">

On the responsive mobile interface, the sidebar menu changes to the top navigation menu which includes page navigation and social media links.


<img src="/hydeX/assets/images/followme-mobile2.png" alt="Mobile interface showing Social Media icons" height="567px" width="340px">

[1]: http://fontawesome.io/