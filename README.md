# anikethreddy.dev

Hugo + [PaperMod](https://github.com/adityatelange/hugo-PaperMod) source for my blog, deployed via GitHub Actions to GitHub Pages at https://anikethreddy.dev/.

## Run locally

```
git clone --recurse-submodules <this repo>
hugo server -D
```

## Publishing a post

1. Draft in `ai-career-log/blog-drafts/NN-slug.md` (private) until it's done.
2. Copy the finished post to `anikethreddy.dev/content/posts/slug.md` and add the front matter from the archetype — `hugo new posts/slug.md` creates the file with it already filled in.
3. Preview with `hugo server -D`.
4. Set `draft: false`, commit, push. It goes live in about a minute via GitHub Actions.
5. Cross-post: Hashnode (set canonical URL to the anikethreddy.dev post), dev.to (`canonical_url` front matter field), and a short LinkedIn/X summary linking back.
