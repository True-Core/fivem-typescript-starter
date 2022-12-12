# A TypeScript starter for FiveM


This is a basic boilerplate for creating a FiveM resource using TypeScript. It includes webpack config files, linting (ESlint + prettier) and a directory structure to get you started.

## Usage
1. Clone repository into your `resources` folder.
2. Install the depencies with `yarn`.

### Development
Use `yarn run watch` to watch files during development.

### Production
You can build your production ready code with `yarn run build`.

This will build the client and server script with the `--mode production` flag.

### Automatic Builds (Optional)
The `fxmanifest.lua` is not setup to automatically build upon first FXServer start. If you'd like to setup automatic builds you must add the following to your `fxmanifest.lua`.

```lua
dependency 'yarn'
dependency 'webpack'

webpack_config 'webpack.config.js'
```

However, due to the speed performance of the pre-packaged webpack/yarn of cfx-server-data, we suggest you don't do this and build manually as described previously ("Production").

## License
This product is MIT licensed. Please make sure you give credit and include this license in your product.

## Original Developer
I have taken this project on from here: https://github.com/d0p3t/fivem-ts-boilerplate.

I liked what Remco did and wanted to bring it up date and share with the community.