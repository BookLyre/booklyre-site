# booklyre.com

The website for **BookLyre** and **BookLyre Studio**: the home page, support page, privacy policies and terms of use, served at [booklyre.com](https://booklyre.com) by GitHub Pages.

| Page | URL |
|------|-----|
| Home | https://booklyre.com/ |
| Guides | https://booklyre.com/guides/ |
| Support | https://booklyre.com/support/ |
| BookLyre privacy policy | https://booklyre.com/privacy/booklyre/ |
| BookLyre Studio privacy policy | https://booklyre.com/privacy/booklyre-studio/ |
| BookLyre terms of use | https://booklyre.com/terms/booklyre/ |
| BookLyre Studio terms of use | https://booklyre.com/terms/booklyre-studio/ |

These are the URLs used in App Store Connect, so keep the paths stable.

## Updating

This repo holds generated HTML. Don't edit the legal pages by hand: they're built from the same Markdown the apps bundle, so the website and the in-app text always match. To change them, edit the source and rebuild:

```sh
pip install markdown
python3 build.py --domain booklyre.com   # writes ./public
```

Then copy the contents of `public/` here and push. Pages redeploys within a minute or two.

## Contact

support@booklyre.com
