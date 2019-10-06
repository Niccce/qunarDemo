# qunardemo
Vue2.5开发去哪儿网App  从零基础入门到实战项目（慕课网）

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).


# 项目环境准备
* node.js、git
* 安装vue-cli(已安装可忽略))
`npm install --global vue-cli`

1. 在GitHub上新建仓库，克隆到本地
2. 创建一个基于webpack打包工具构建的Vue项目
3. `vue init webpack qunarDemo`，选择各项配置（最后一个是项目放置的位置）
4. `cd qunarDemo`
5. `npm run dev`，帮我们打包
6. 在`http://localhost:8080`查看项目

# 项目代码结构介绍
README.md：项目说明文件
package.json：记录在开发项目时的第三方依赖包
package-lock.json：帮助我们确定安装的第三方包的版本，保持团队编程的统一
index.html：项目默认的首页模版文件
.postcssrc.js：对postcss的配置项
.gitignore：里面记录的文件不会被提交到仓库
.eslintrc.js：配置代码的规范
.eslintignore：里面记录的文件不受eslint检测工具检测
.editorconfig：帮助我们配置编辑器的语法
.babelrc：babel配置

* static目录：放静态资源，例如静态图片，用于模拟数据的json文件
* node_modules：放第三方依赖的包
* src目录：放置整个项目的源代码
    * main.js：整个项目的入口文件
    * App.vue：项目原始的根组件
    * router  ->  index.js：这个项目所有的路由
    * components：放项目里要用的小组件
    * assets：放项目里用到的图片资源
* config目录：放置项目的配置文件
    * index.js：基础配置
    * dev.env.js：开发环境的配置
    * prod.env.js：线上环境的配置（即最后打包—）
* build目录：放置项目打包的webpack的配置内容
    * webpack.base.conf.js：基础webpack配置项
    * webpack.dev.conf.js：开发环境的webpack配置项
    * webpack.prod.conf.js：线上环境的webpack配置项
    * 这是vue-cli自动帮我们构建好的，一般来说不需要怎么修改