# Webpack 4 Configuration

This is `webpack v4` configuration forked and simplified from Nenad Novaković, that I am using for small static projects.
Feel free to contribute, improve or use it for your projects.

### What does this configuration handles?

> Common for development & production environment

- it accepts one entry point; one for the `app` 
- it compiles everything with relative paths, rather than absolute
- it compiles `sass/scss` to the `css` file
- it compiles `es6` to the syntax that every browser can understand
- it has alias as `~` for importing your `js` files, no more mess with directory back-levels

> Development environment

- it runs webpack-dev-server with browser-sync support
- it builds source-maps

> Production environment

- it minifies `js`
- it minifies multiple image types _(gif, png, jpg, jpeg, svg)_
- it copies all `web fonts`
- it minifies all `json` files from `data` directory
- it has subresource-integrity
- it does not build source-maps, but you may specify it on line `216` if you want them


### Commands?

It's pretty easy... You do not have a bunch of commands, just two of them:

- `npm run serve` – to start with development
- `npm run build` - to make it ready for production use
