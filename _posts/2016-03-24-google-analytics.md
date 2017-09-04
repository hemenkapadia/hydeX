---
layout: post
title: Web analytics using Google Analytics
excerpt: hydeX provides built-in integration with Google Analytics to help gain insights on how your blog is performing. 
comments: true
tags:
  - hydeX
  - Features
  - Google Analytics
  - Web Analytics
---

A critical aspect of having your web presence is to be able to understand and gain insights about how your audience is interacting with your website/blog. 

It is super easy to setup your own blog by forking hydeX. Enabling [Google Analytics][1] on your blog is even easier.

Before you start, I recommend you understand the [hierarcy of accounts, properties, and views][4]

Next, [get a Google Analytics tracking code][2] generated for your website. If you do not have a Google Analytics account already, then start by [getting a Google Analytics account][3] first.

Google Analytics tracking code is of the format `UA-AccountID-PropertyNumber`, where `Account ID` is numeric and `Property Number` starts with 1 and increments by 1 for each new property you create.

Next, update hydeX config file with your tracking code. By default, I include a dummy tracking code in the config file. Update the value of `ga_id` with your tracking code.

```yaml
# Comments - Google Analytics Configuration
ga_enable:                      true
ga_id:                          UA-00000000-0          # replace this
```
Push the config changes to GitHub and you will notice web traffic in your Google Analytics dashboard.


[1]: https://www.google.com/analytics/
[2]: https://support.google.com/analytics/answer/1042508
[3]: https://support.google.com/analytics/answer/1008015
[4]: https://support.google.com/analytics/answer/1009618

