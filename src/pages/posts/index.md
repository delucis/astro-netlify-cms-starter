---
title: Using Netlify CMS with an Astro site
publishDate: 16 May 2022
author: Chris Swithinbank
authorURL: https://twitter.com/swithinbank
description: How to get started using Netlify CMS to manage your Astro site’s content
layout: ../../layouts/BlogPost.astro
---
![Astro + Netlify CMS logos](/assets/blog/header.png)

[Netlify CMS](https://www.netlifycms.org/) is an open-source, Git-based content management system. It provides a single-page app for editing content and can publish that content by committing it to a hosted Git repo (for example on GitHub or GitLab).

Adding Netlify CMS to an [Astro](https://astro.build/) site would usually involve creating a number of files in different parts of your project directory and then keeping all those moving parts in sync. With the [`astro-netlify-cms`](https://github.com/delucis/astro-netlify-cms/) integration, you configure the integration in your `astro.config.mjs` file and the integration takes care of the rest.

```javascript
import { defineConfig } from 'astro/config';
import NetlifyCMS from 'astro-netlify-cms';

export default defineConfig({
  integrations: [
    NetlifyCMS({
      config: {
        backend: {
          name: 'git-gateway',
          branch: 'main',
        },
        collections: [
          // Content collections
        ],
      },
    }),
  ],
});
```