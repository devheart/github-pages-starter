# GitHub Pages starter
> Rapid bare minimum GitHub Pages starter

* **Live reload** - Changes are instantly reflected in the browser.
* **Fast rendering** - High performance Gulp tasks compile SASS and minify assets, Jekyll generates HTML.
* **Asset minification** - Images and CSS are losslessly minified.

## Installation
1. Clone/download repo
2. `yarn install`
3. Edit `_config.yml`, set your values for `url`, `repository`, `custom_settings`.

## Development
Open 3 terminals and run the following commands (they need to be run in parallel).

1. `yarn run jekyll-dev` - Generates site on changes (output to `/_site`)
2. `gulp watch` - Ccompile SASS and images on changes to `/_site/assets`.
3. `yarn run browser-sync` - Starts Browsersync, hosting content from `/_site` at `http://localhost:3000` and injects asset changes.

## Production
1. `gulp build` - Cleanup and generates assets to `/assets`.
2. Push changes to `master`.
