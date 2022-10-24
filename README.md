![Astro + Netlify CMS](https://raw.githubusercontent.com/delucis/astro-netlify-cms/HEAD/header.png)

<h1 align="center">Astro Blog Starter with Netlify CMS</h1>

This example is based on [the basic Astro blog starter kit][starter], and
adds [the Astro Netlify CMS integration][integration].

## Quick deploy

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)][deploy]

☝️ Click this button to copy this project to your own GitHub (or GitLab)
account and set up continuous deployment with Netlify as if by magic. ✨

Once you’ve got the project set up, you do need to
[activate Netlify Identity in the Netlify UI][identity] and then enable
[“Git Gateway”][gateway] to allow e-mail/password authentication.

## Commands

All commands are run from the root of the project, from a terminal:

| Command            | Action                                             |
| :----------------- | :------------------------------------------------- |
| `pnpm install`     | Installs dependencies                              |
| `pnpm run dev`     | Starts local dev & Netlify CMS proxy servers       |
| `pnpm run build`   | Build your production site to `./dist/`            |
| `pnpm run preview` | Serve `./dist/` & run the Netlify CMS proxy server |

> **Note**
> These commands are using [`pnpm`][pnpm], a fast and efficient package manager.
> You can choose to use `npm` or `yarn` instead if you prefer, but remember to update the config in [`netlify.toml`](netlify.toml) to match.

[starter]: https://astro.new/blog?on=github
[integration]: https://github.com/delucis/astro-netlify-cms
[deploy]: https://app.netlify.com/start/deploy?repository=https://github.com/delucis/astro-netlify-cms-starter
[identity]: https://docs.netlify.com/visitor-access/identity/
[gateway]: https://docs.netlify.com/visitor-access/git-gateway/
[pnpm]: https://pnpm.io/
