---
layout: post
title: Customize the layout and theme of your blog
excerpt: hydeX makes customizing the layout and theme of your blog as simple as updating couple of configurations in the config file.
comments: true
tags:
  - Features
  - Theme
  - Layout 
  - Sidebar
  - Sticky Sidebar
  - Reverse Layout
  - hydeX
---

hydeX makes it extremely easy to customize the look and feel of your blog by making minor configuration changes in the `Theme configuration` section of `_config.yml`. To achieve the same customizations in Hyde, you would need to make code changes in the HTML templates.

### Sidebar and Layout customization

By default, hydeX displays the sidebar to left of the main content area. It can be moved to right of the main content area i.e. reversed, using the `layout` configuration. Possible configuration options are `normal` (default) where sidebar is to left of the main content, and `reverse` where sidebar is to right of the main content area.

Sidebar content, by default, floats to the top. It can be configured to stick to the bottom using `sidemenutype` configuration. Possible configuration options are `nonsticky` (default) i.e. content floating to the top, and `sticky` where content sticks to the bottom.

```
# Theme configurations
layout:                         reverse                # [normal | reverse]
sidemenutype:                   sticky                 # [nonsticky | sticky]
```

![Reverse and Sticky Layout](/hydeX/assets/images/reverse-sticky-layout.png)

A site with reverse layout and sticky sidebar content looks good too, however, the defaults are based on my preference.


### Theme customization

In line with hydeX's minimalistic philosophy, and my bias for [Grayscale][2], the default theme for hydeX is set to `theme-base-00`. For those who want to add a bit of color to their blog, hydeX supports 8 additional color themes based on [base16 color palette][1].

![Theme Palette](/hydeX/assets/images/theme-palette.png)

Update the `pooletheme` configuration, in `_config.yml` file, with the value of the theme you want to apply to your blog.

```
# Theme configurations
pooletheme:                     theme-base-08
```

hydeX with the `theme-base-08` theme applied to it. 


![hydeX Base08 Theme](/hydeX/assets/images/base08-theme.png)


[1]: https://github.com/chriskempson/base16
[2]: https://en.wikipedia.org/wiki/Grayscale


