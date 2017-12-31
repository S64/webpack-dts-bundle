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

## License

```
Copyright 2017 Shuma Yoshioka

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
