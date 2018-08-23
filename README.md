### 目录结构介绍

<!--more-->

- 首页
  - 完整布局
  - 换肤(全局功能，暂时只实现了顶部导航的换肤，后续加上其他模块)
- 导航菜单
  - 顶部导航(菜单伸缩，全屏功能)
  - 左边菜单(增加滚动条以及适配路由的 active 操作)
- UI 模块
  - 按钮(antd 组件)
  - 图标(antd 组件并增加彩色表情符)
  - 加载中(antd 组件并增加顶部加载条)
  - 通知提醒框(antd 组件)
  - 标签页(antd 组件)
  - 轮播图(ant 动效组件)
  - 富文本
  - 拖拽
  - 画廊
- 动画
  - 基础动画(animate.css 所有动画)
  - 动画案例
- 表格
  - 基础表格(antd 组件)
  - 高级表格(antd 组件)
  - 异步表格(数据来自掘金酱的接口)
- 表单
  - 基础表单(antd 组件)
- 图表
  - echarts 图表
  - recharts 图表
- 页面
  - 登录页面(包括 GitHub 第三方登录)
  - 404 页面

### 代码目录

```js
+-- build/                                  ---打包的文件目录
+-- config/                                 ---npm run eject 后的配置文件目录
+-- node_modules/                           ---npm下载文件目录
+-- public/
|   --- index.html							---首页入口html文件
|   --- npm.json							---echarts测试数据
|   --- weibo.json							---echarts测试数据
+-- src/                                    ---核心代码目录
|   +-- axios                               ---http请求存放目录
|   |    --- index.js
|   +-- components                          ---各式各样的组件存放目录
|   |    +-- animation                      ---动画组件
|   |    |    --- ...
|   |    +-- charts                         ---图表组件
|   |    |    --- ...
|   |    +-- dashboard                      ---首页组件
|   |    |    --- ...
|   |    +-- forms                          ---表单组件
|   |    |    --- ...
|   |    +-- pages                          ---页面组件
|   |    |    --- ...
|   |    +-- tables                         ---表格组件
|   |    |    --- ...
|   |    +-- ui                             ---ui组件
|   |    |    --- ...
|   |    --- BreadcrumbCustom.jsx           ---面包屑组件
|   |    --- HeaderCustom.jsx               ---顶部导航组件
|   |    --- Page.jsx                       ---页面容器
|   |    --- SiderCustom.jsx                ---左边菜单组件
|   +-- style                               ---项目的样式存放目录，主要采用less编写
|   +-- utils                               ---工具文件存放目录
|   --- App.js                              ---组件入口文件
|   --- index.js                            ---项目的整体js入口文件，包括路由配置等
--- .env                                    ---启动项目自定义端口配置文件
--- .eslintrc                               ---自定义eslint配置文件，包括增加的react jsx语法限制
--- package.json
```

### 安装运行

##### 1.下载或克隆项目源码

##### 2.yarn 或者 npm 安装相关包文件(首先推荐使用 yarn，国内建议增加淘宝镜像源，不然很慢)

```js
yarn or npm i
```

##### 3.启动项目

```js
yarn start or npm start
```

##### 4.打包项目

```js
yarn build or npm run build
```
