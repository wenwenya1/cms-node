### node介绍

简单的说 Node.js 就是运行在服务端的 JavaScript。

Node.js 是一个基于Chrome JavaScript 运行时建立的一个平台。

Node.js是一个事件驱动I/O服务端JavaScript环境，基于Google的V8引擎，V8引擎执行Javascript的速度非常快，性能非常好。


### Express是什么
Express是一个开放，快速，简单的node.js Web开发框架。通过它。可以快速搭建node应用

### Express 特性
- 简单易学
- 丰富的基础API支持
- 强大的路由功能
- 灵活的中间件
- 高性能
- 非常稳定
- 视图支持非常多的模板引擎

安装命令
npm install -g express-generator

创建项目
express --view=hjs myapp

### 什么是MVC

MVC 模式代表 Model-View-Controller(模型-视图-控制器) 模式。这种模式用于应用程序的分层开发。

Model(模型)- 业务流程/状态的处理以及业务规则的制定。业务流程的处理过程对其它层来说是黒箱操作，模型接受视图请求的数据，并返回最终的处理结果。业务模型的设计可以说是HVC最主要的核心

View(视图)- 视图代表模型包含的数据的可视化。

Controller(控制器)- 控制器作用于模型和视图上。它控制数据流向模型对象，并在教据变化时更新脚图。它使视图与机型分离开。

### 数据库表结构设计

#### 应用 【application】

id   | name  | application_string
-----|------- | --------

#### 页面 【page】

id   | application_id(外键) | name |cover(封面) | page_type(页面类型) | is_abled （是否启用）| page_string |update_time |create_time| creator（创建人）| share_desc（微信分享文案）| share_image （微信分享图片）|
---- | --------- | ---------|----------| -----|-----|------|-----|----|----|---|---

#### 组件详情 【components】

id | page_id(外键) | component_string | sort | name （组件名称）
------ | -------------|-----| ----------|--------------|-----|----

#### 用户【user】

id | user_name(用户名) | password(密码)
-----|-----|----

