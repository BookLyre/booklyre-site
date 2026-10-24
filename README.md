# booklyre-site

The website for **BookLyre** and **BookLyre Studio**, served by GitHub Pages at
**[booklyre.com](https://booklyre.com)**.

BookLyre turns DRM-free ebooks into full-cast audiobooks, with a different AI voice for each
character, generated entirely on your iPhone or iPad. BookLyre Studio does the same for
independent authors working from their own manuscripts.

## Pages

| Path | Page |
| --- | --- |
| [`/`](https://booklyre.com/) | Home |
| [`/support/`](https://booklyre.com/support/) | Support and FAQ (the App Store support URL) |
| [`/privacy/booklyre/`](https://booklyre.com/privacy/booklyre/) | BookLyre privacy policy |
| [`/terms/booklyre/`](https://booklyre.com/terms/booklyre/) | BookLyre terms of use |
| [`/privacy/booklyre-studio/`](https://booklyre.com/privacy/booklyre-studio/) | BookLyre Studio privacy policy |
| [`/terms/booklyre-studio/`](https://booklyre.com/terms/booklyre-studio/) | BookLyre Studio terms of use |

The privacy and terms URLs are linked from the App Store listings and from inside the apps,
so keep them stable. If a page has to move, leave a redirect at the old path.

## How it's built

Plain static HTML and one stylesheet (`style.css`). No build step runs here: the files in
this repo are published exactly as they are.

- `CNAME` sets the custom domain `booklyre.com`. Don't delete it.
- `.nojekyll` turns off Jekyll processing.
- `404.html` is the not-found page.

Pages publishes from the `main` branch, root folder. A push to `main` goes live within a
minute or two.

## Editing

Edit the HTML directly, or regenerate the pages from their source and commit the output.
Before pushing, open `index.html` locally, or run `python3 -m http.server` in this folder,
and check the links.

## DNS

`booklyre.com` is registered at Porkbun. The root has `A` records pointing at GitHub Pages
(`185.199.108.153`–`185.199.111.153`), and `www` is a `CNAME` to `booklyre.github.io`.
Porkbun email forwarding handles `support@booklyre.com`; leave its `MX` records alone.

## Contact

support@booklyre.com

© 2026 Brandon J Conover
