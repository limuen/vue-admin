## 简介

[vue-element-admin-express](https://github.com/limuen/vue-element-admin-express) 是一个后台前端解决方案，它基于 [vue](https://github.com/vuejs/vue) 和 [element-ui](https://github.com/ElemeFE/element)以及[express](https://www.expressjs.com.cn/)实现。它使用了最新的前端技术栈，内置了动态路由，权限验证，并提供了简单的后端API服务，开箱即用，帮助你快速构建前后端分离动态路由和权限模型。

本项目通过[vue-element-admin](https://github.com/PanJiaChen/vue-element-admin)精简改造，移除了大部分组件，如需要其他组件，可前往搬运。


- [github仓库](https://github.com/limuen/vue-element-admin-express)


## 前序准备

你需要在本地安装 [node](http://nodejs.org/) 、[git](https://git-scm.com/) 和 [mysql](https://www.mysql.com/)。本项目技术栈基于 [ES2015+](http://es6.ruanyifeng.com/)、[vue](https://cn.vuejs.org/index.html)、[vuex](https://vuex.vuejs.org/zh-cn/)、[vue-router](https://router.vuejs.org/zh-cn/) 、[vue-cli](https://github.com/vuejs/vue-cli) 、[axios](https://github.com/axios/axios) 、 [element-ui](https://github.com/ElemeFE/element) 和 [express](https://www.expressjs.com.cn/)，提前了解和学习这些知识会对使用本项目有很大的帮助。


## 功能

```
- 登录 / 注销

- 系统管理
  - 用户管理
  - 菜单管理
  - 角色管理
  - 登录日志
```

## 服务端

```bash
# 进入server端目录
cd vue-element-admin-express/server

# 安装依赖
npm install

# 建议不要直接使用 cnpm 安装依赖，会有各种诡异的 bug。可以通过如下操作解决 npm 下载速度慢的问题
npm install --registry=https://registry.npm.taobao.org

# vue-element-admin-express/server/mysql.sql 导入数据表到mysql数据库
# vue-element-admin-express/server/model/init.js 配置数据库信息:数据库名，登录账号，登录密码，ip,端口

# 启动 默认绑定ip：127.0.0.1 端口：3001, 可以在app.js指定你需要的ip和端口
npm run start

```

接口地址：http://127.0.0.1:3001

## 前台

```bash
# 克隆项目
git clone https://github.com/limuen/vue-element-admin-express.git

# 进入项目目录
cd vue-element-admin-express

# 安装依赖
npm install

# 建议不要直接使用 cnpm 安装依赖，会有各种诡异的 bug。可以通过如下操作解决 npm 下载速度慢的问题
npm install --registry=https://registry.npm.taobao.org

# 启动服务
npm run dev
```

浏览器访问 http://localhost:9527

## 发布

```bash
# 构建测试环境
npm run build:stage

# 构建生产环境
npm run build:prod
```

## 其它

```bash
# 预览发布环境效果
npm run preview

# 预览发布环境效果 + 静态资源分析
npm run preview -- --report

# 代码格式检查
npm run lint

# 代码格式检查并自动修复
npm run lint -- --fix
```


## 支持浏览器版本

Modern browsers and Internet Explorer 10+.

| IE / Edge | Firefox | Chrome | Safari |
| --------- | --------- | --------- | --------- |
| IE10, IE11, Edge| last 2 versions| last 2 versions| last 2 versions

