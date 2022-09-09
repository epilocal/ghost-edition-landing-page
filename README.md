# Landing Page Based on Edition Theme

Landing page theme for [Ghost](https://github.com/TryGhost/Ghost) based on [Ghost Edition Theme](https://github.com/TryGhost/Edition) by [Epilocal](https://www.epilocal.com/).

Accompanying guide: [How to Use Ghost as a Landing Page](https://www.epilocal.com/blog/ghost-landing-page/)

![Ghost Edition Landing Page](https://user-images.githubusercontent.com/9167731/189374899-b7b51f7c-2554-41d3-b0b6-8f4c5383ce41.png)

# Instructions

1. [Download this theme](https://github.com/epilocal/ghost-edition-landing-page/dist/edition-landing-page.zip)
2. Log into Ghost, and go to the `Design` settings area to upload the zip file
3. In the Settings > Lab > Routes area, upload the ``routes.yaml`` file

# Development

Edition styles are compiled using Gulp/PostCSS to polyfill future CSS spec. You'll need [Node](https://nodejs.org/), [Yarn](https://yarnpkg.com/) and [Gulp](https://gulpjs.com) installed globally. After that, from the theme's root directory:

```bash
# Install
yarn

# Run build & watch for changes
yarn dev
```

Now you can edit `/assets/css/` files, which will be compiled to `/assets/built/` automatically.

The `zip` Gulp task packages the theme files into `dist/edition.zip`, which you can then upload to your site.

```bash
yarn zip
```
