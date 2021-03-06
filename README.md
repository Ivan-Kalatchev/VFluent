<p align="center">
    <img src="./examples/assert/logo/VFluent.png"/>
</div>

<p align="center">
    <a href="LICENSE">
      <img src="https://img.shields.io/badge/License-MIT-yellow.svg">
    </a>
    <a href="BUILD">
      <img src="https://travis-ci.com/aleversn/VFluent.svg?branch=master">
    </a>
</p>

## 基于 Vue Cli 的 Fluent UI DESIGN

### 目录结构

```bash
- build # 脚手架
  config.js # 组件库配置文件
- examples
  - docs # 在线演示文档(VuePress)
  index.js # Vue Cli Lib 打包入口
- lib # 打包ump文件
- packages
  - common-theme # 通用主题
  - {themeName}-theme
    index.scss # 全局scss 由脚本生成
    {ComponentScss}.scss
  - {ComponentName}
    - src # 组件Source
      index.vue # 组件
    index.js # 组件入口
  index.js # 所有组件入口 由脚本生成
components.json # 组件目录
vue.config.js # Vue cli 配置
```

### 脚本命令(2019-12-16 更新)

```bash
npm run pub # 打包推送到npm
npm run docs:dev # 开发文档模式
npm run bin:new componentName chineseName #新建组件
npm run bin:rm componentName #移除组件并重新定制入口
npm run bin:entry # 定制入口
```

### Fluent Design UI (Vue 2.0+)

#### DOCS

[中文文档](https://aleversn.github.io/VFluent)

#### How to use

1. install via npm

```bash
  yarn add vfluentdesign # recommend
```

```bash
  npm i vfluentdesign
```

2. import (vue entry main.js)

```js
import Vue from "vue";
import VueFluent from "vfluentdesign";
import "vfluentdesign/lib/index.css";

Vue.use(VueFluent);
```

3. sample example

```html
<fv-button>Hello Vue Fluent!</fv-button>
```

4. about Fabric UI

Our project have many using cases contains Microsoft's Fabric UI, such as icons and shadows, for more details you can click <a href="https://developer.microsoft.com/en-us/fabric#/styles">here</a> to get more information.

Here is the icon using sample.

```vue
<i class="ms-Icon ms-Icon--AADLogo"></i>
```

In particular, if you're using a component of Fluent Vue Design and it contains a prop that support icon, you only need to type the icon's name in prop.

### License

MIT License

Copyright (c) 2020 Creator SN™

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
