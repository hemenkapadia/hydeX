---
layout: post
title: Get insights about your blog's audience using Google Analytics
excerpt: hydeX provides built-in integration with Google Analytics to help you get a deeper understanding of your blog's audience and performance. 
comments: true
tags:
  - hydeX
  - Features
  - Google Analytics
  - Web Analytics
---

A critical aspect of having your web presence is to be able to understand and gain insights about how your audience is interacting with your blog. [Google Analytics][1] is the defacto standard to enable analytics on your website and for mobile applications. 

hydeX provides built-in integration with [Google Analytics][1]. To enable web analytics for your hydeX based blog you only need to update your Google Analytics Property ID, hereafter called `ga_id`, in the `_config.yml` file. 

Before you delve deeper, I strongly recommend you understand the [hierarchy of accounts, properties, and views][4] by which Google Analytics organizes the data it collects. For our purpose, we need a Google Analytics Property Id created.

### Create Google Analytics Property ID 

If you are new to Google Analytics, then the first step is to [sign up for Google Analytics][2]. Note that before you land on the [Sign Up][2] page you will be required to authenticate with Google using your regular Google credentials i.e. the same credentials you use for other Google services like Gmail etc.

The [Sign up][2] page will lead you to [Create a New Account and Property][3] page where you can provide the required details about your blog.

![Create a New Google Analytics Account and Property](/hydeX/assets/images/ga-create.png)

Submitting this form should get you a Google Analytics Property ID. 

The Property ID would be of the format `UA-AccountID-PropertyNumber`, where `AccountID` is numeric and `PropertyNumber` starts with 1 and increments by 1 for each new property you create.

### Integrate hydeX with Google Analytics

Now that you have the Google Analytics Property ID created, next step is to update the same in hydeX configuration file `_config.yml`. Update the value of `ga_id` parameter to the property ID obtained in the step above. 

Also ensure that `ga_enable` is set to `true` or else Google Analytics will not be enabled for your blog.

```yaml
# Google Analytics Configuration
ga_enable:      true
ga_id:          UA-00000000-0   # replace this
```
Push the updated config changes to GitHub and you will notice web traffic in your Google Analytics dashboard, after about 5 to 6 hours of publishing the changes.


[1]: https://www.google.com/analytics/analytics/features/ 
[2]: https://analytics.google.com/analytics/web/provision/?authuser=0#provision/SignUp/
[3]: https://analytics.google.com/analytics/web/provision/?authuser=0#provision/CreateAccount/ 
[4]: https://support.google.com/analytics/answer/1009618?hl=en&ref_topic=3544906
