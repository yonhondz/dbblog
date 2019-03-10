## 简介
这是一个基于Springboot2.x，vue2.x的前后端分离的开源博客系统，提供 前端界面+管理界面+后台服务 的整套系统源码。响应式设计，手机、平板、PC，都有良好的视觉效果！

- 你可以拿它作为前端Vue2.0学习的练手教程；
- 你也可以把它作为springboot技术的学习项目；
- 你还可以将其视为一个前后端分离的项目实践；
- ...

## 站点演示
[www.dblearn.cn](www.dblearn.cn)

## 模块分层
### 后端模块
```shell
dbblog
├── dbblog-auth   # 鉴权模块：shiro
│   ├── pom.xml
│   └── src
├── dbblog-core   # 核心模块：配置文件，Entity类，mapper类，工具类，异常过滤等
│   ├── pom.xml
│   └── src
├── dbblog-manage # 后台管理界面Service
│   ├── pom.xml
│   └── src
├── dbblog-portal # 前端界面Service
│   ├── pom.xml
└── └── src
```
### 前端模块
#### 后台管理页面
```shell
├── assets
├── components # 公共组件
├── element-ui
├── element-ui-theme # elementUI主题
├── icons   
├── router  # 路由
├── store   # vuex
├── utils   # js工具类
└── views   
    ├── common # 公共模块
    └── modules
        ├── article    # 文章模块
        ├── book       # 阅读模块
        ├── comment    # 评论模块
        ├── operation  # 运维模块
        └── sys        # 系统模块


```
#### 前台页面
```shell
├── assets
├── common
├── components
│   ├── content # 页面
│   │   ├── ArticleContent.vue      # 文章详情页
│   │   ├── ArticleListContent.vue  # 文章列表页
│   │   ├── BookContent.vue         # 图书详情页
│   │   ├── BookListContent.vue     # 图书列表页
│   │   ├── BookNoteContent.vue     # 笔记详情页
│   │   ├── BookNoteListContent.vue # 笔记列表页
│   │   ├── HomeContent.vue         # 首页
│   │   └── TimeLineContent.vue     # 归档页
│   ├── footer
│   ├── header
│   ├── index
│   ├── utils
│   └── views # 页面组件库
│       ├── Archive 
│       ├── Article
│       ├── Book
│       ├── BookNote
│       ├── Classify
│       └── TimeLine
├── router # 路由
├── store  # Vuex
└── utils  # js工具类

```
## 项目部署
### 服务端
项目后端环境
- JDK1.8
- Mysql5.7
- Redis
- IDEA编译器
- Lombox插件（百度一下）

部署步骤：
1. 创建数据库dbblog，并导入dbblog-backend -> db里的所有sql文件
2. 修改dbblog-backend -> dbblog-> dbblog-core里的application-*.yml的数据库连接和redis连接
3. 导入项目，并且运行dbblog-backend -> dbblog-portal -> BlogApplication里的main方法

### 前端
前端环境：
- Node.js 8.0+
- WebStorm编辑器

部署步骤：
1. 导入项目，运行 npm install（如果失败，清空包后试试cnpm install）
2. 启动项目：npm run dev

## 界面预览


## 碎碎念
上大学的时候做过博客，技术选型也从一开始的SSM+JSP [博客1](https://github.com/llldddbbb/Blog) 

--> 过渡到分模块的SpringBoot [博客2](https://github.com/llldddbbb/Blog2) 

-->  到现在的前后端分离博客 [博客3](https://github.com/llldddbbb/dbblog) 

如果是初学Java的朋友也可以跟着流程借鉴借鉴这些代码，试着实现一个自己的博客，相信能对你的成长有所帮助！

如果有心，不妨请博主喝杯茶::laughing::

![支付.jpg](http://oss.dblearn.cn/dbblog/20190310/7517419c57e14d548ec13f4a550edbc0.jpg)

最后的最后，我的github地址是[https://github.com/llldddbbb/dbblog](https://github.com/llldddbbb/dbblog)，开源不易，一定要给我==Star==哦！！
