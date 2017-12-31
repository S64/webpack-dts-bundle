# webpack-dts-bundle

Webpack plugin of dts-bundle wrapper.

## Install

```sh
npm install --save-dev webpack-dts-bundle
```

## Usage

```ts
// in `webpack.config.ts`
import * as webpack from 'webpack';
import * as path from 'path';
import DtsBundlePlugin from 'webpack-dts-bundle';

const configuration: webpack.Configuration = {
  plugins: [
    new DtsBundlePlugin({
      name: 'your-awesome-module-name',
      main: path.resolve(__dirname, './src/index.d.ts'),
      out: path.resolve(__dirname, './dist/index.d.ts'),
      verbose: true,
    }),
  ]
};
```
