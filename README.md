## Voyager

Just another jekyll theme. Demo: <http://redvi.github.io/voyager>

### Feathures:

All HTML files are compressed (see `_layouts/compress.html`).

**Post**

All post settings can be changed. Example:

```
---
layout: post
bg: '2016/background.jpg'
title: "Post Heading"
crawlertitle: "page title"
summary: "post description"
date: 2016-06-29
tags : ['front-end']
slug: post-url
author: "Author"
categories: posts
---
```

`bg` is a path to background of your article. By default backgrounds are placed in the `assets/images` directory.

**Page**

If page contains `active` tag, it will be show on site menu.

```
---
layout: page
title: "About"
permalink: /about/
active: about
---
```

**Archive**

Archive page is sorting posts by tags. No more than one tag in one post.

Good:

```
tags : ['front-end']
```

Bad:

```
tags : ['front-end', 'jekyll']
```

Don't forget to change `_config.yml`.

**Relative paths**

If your blog is not in the root directory, you can include images with a relative path. For example:

```
![my_image]({{ site.images | relative_url }}/image.jpg)
```

## Production environment

Build for production:

`JEKYLL_ENV=production jekyll build`
