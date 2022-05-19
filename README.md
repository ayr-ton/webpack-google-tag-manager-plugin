<div align="center">
  <a href="https://github.com/webpack/webpack">
    <img width="200" height="200"
      src="https://webpack.js.org/assets/icon-square-big.svg">
  </a>
  <h1>Webpack Google Tag Manager Plugin</h1>
  <p>A clean and easy way to add Google Tag Manager support to your web project.</p>
</div>

![npm](https://img.shields.io/npm/v/webpack5-google-tag-manager-plugin)
![npm](https://img.shields.io/npm/dw/webpack5-google-tag-manager-plugin)

## Installation

```bash
  npm i --save-dev webpack5-google-tag-manager-plugin
```

```bash
  yarn add --dev webpack5-google-tag-manager-plugin
```

## Examples
Webpack basic configuration for setting up the plugin
```Javascript
import webpack from 'webpack'
import HtmlWebpackPlugin from 'html-webpack-plugin'
import GoogleTagManagerPlugin from 'webpack5-google-tag-manager-plugin'

module.exports = {
    ...
    plugins: [
        new HtmlWebpackPlugin({
          ...
        }),
        new GoogleTagManagerPlugin({
            id: 'your-container-id',
        }),
    ],
}

```

Webpack configuration for making use of your environments
```Javascript
import webpack from 'webpack'
import HtmlWebpackPlugin from 'html-webpack-plugin'
import GoogleTagManagerPlugin from 'webpack5-google-tag-manager-plugin'

module.exports = {
    ...
    plugins: [
        new HtmlWebpackPlugin({
          ...
        }),
        new GoogleTagManagerPlugin({
            id: 'your-container-id',
            auth: 'your-auth-value',
            preview: 'your-environment-value',
        }),
    ],
}

```

## [License](https://github.com/timjorjev/webpack-google-tag-manager-plugin/blob/master/LICENSE)

Webpack Google Tag Manager Plugin is published under [MIT License](https://github.com/timjorjev/webpack-google-tag-manager-plugin/blob/master/LICENSE).

## Collaboration

If you have any questions, please contact me via [e-mail](mailto:ayrton@duck.com). For [issues](https://github.com/ayr-ton/webpack-google-tag-manager-plugin/issues), please [open an issue](https://github.com/ayr-ton/webpack-google-tag-manager-plugin/issues/new)!
