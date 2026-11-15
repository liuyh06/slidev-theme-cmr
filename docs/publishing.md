# Publishing

Repository: https://github.com/liuyh06/slidev-theme-cmr
Preview: https://liuyh06.github.io/slidev-theme-cmr/
Package: slidev-theme-cmr

## npm

Run `npm run check`, `npm run build`, `npm run build:starter`, and `npm pack --dry-run` before publishing. Package contents use an explicit allowlist; private reference slides, source-PPT images, cache, local paths and credentials are excluded.

Authenticate interactively with `npm login` in your own terminal. Never paste a password, OTP, or token into a chat or issue. Then run:

```sh
npm publish --access public
```

Version 0.1.0 is the initial release candidate. Check registry availability immediately before publishing. A packed release candidate is not proof that the registry version has been published.

## GitHub Pages

The Pages workflow installs from the lockfile, builds the example with the repository base path, uploads dist, and deploys using GitHub Actions. Repository Settings → Pages must use GitHub Actions as the build source. The package does not need to be published for the source example to build.

## Slidev community gallery

The curated gallery lives in https://github.com/slidevjs/slidev/blob/main/docs/.vitepress/themes.ts . Append an entry to `community` before the placeholder entry. Use the snippet in `docs/gallery-entry.ts` once the repository, preview, screenshots, and npm package are live. Open a pull request against slidevjs/slidev; the maintainers decide whether to merge it.

Official documentation: https://sli.dev/guide/write-theme and https://sli.dev/resources/theme-gallery . npm publication does not automatically add the theme to the curated gallery.
