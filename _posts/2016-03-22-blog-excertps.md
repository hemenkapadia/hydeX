---
layout: post
title: Display post excerpts on the blog main page
excerpt: Configure hydeX's main page to optionally show excerpts in the post listing.  
comments: true
tags:
  - hydeX
  - Features
  - Post Excerpts
  - Main Page
---

Unlike [Hyde][1], hydeX's main page does not display complete blog post content. Instead, it displays a listing of posts published on the blog. 

By default, the post listing includes the excerpt of the post below the blog title as shown in the below screen-shots.

### Desktop Interface (with excerpts)
![Desktop interface with post excerpts](/hydeX/assets/images/excerpt-desktop.png)

### Mobile Interface (with excerpts)
<img src="/hydeX/assets/images/excerpt-mobile.png" alt="Desktop interface with post excerpts" height="480px" width="320px">


The display of post excerpts can be disabled using the `showexcerpt` property in hydeX configuration file. By default, it is configured to display the excerpt in post listing.


```yaml
# Theme configurations
pooletheme:                     theme-base-00
layout:                         normal                 # [normal | reverse]
sidemenutype:                   nonsticky              # [nonsticky | sticky]
showexcerpt:                    true                   # [true | false]
rel_post_count:                 3
```

Configuring hydeX to not display the excerpts has effect across Desktop as well as Mobile interfaces as shown in the screen-shots below.

### Desktop Interface (without excerpts)
![Desktop interface without post excerpts](/hydeX/assets/images/excerpt-no-desktop.png)

### Mobile Interface (without excerpts)
<img src="/hydeX/assets/images/excerpt-no-mobile.png" alt="Desktop interface with post excerpts" height="480px" width="320px">

Thanks, hope this clarification helps.

[1]: http://hyde.getpoole.io