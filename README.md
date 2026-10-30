# orellut.net

Sources for orellut.net website, built with [Hugo](https://gohugo.io/) and the
[PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme.

## Setup

Requires Hugo extended (same version as `HUGO_VERSION` in
`.github/workflows/hugo.yaml`).

```bash
git clone --recurse-submodules git@github.com:j-sp/orellut.net.git
```

## Writing

```bash
hugo new content posts/my-new-post.md   # creates a draft
hugo server -D                          # preview at http://localhost:1313, drafts included
```

Set `draft = false` in a post's front matter to publish it.

## Deployment

Every push to `main` is built and deployed to GitHub Pages by
`.github/workflows/hugo.yaml`. The base URL comes from the repository's Pages
settings, so it is not set in `hugo.toml`.

## Updating the theme

```bash
git submodule update --remote themes/PaperMod
```
