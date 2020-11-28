# 基本资料

| / |  / | / | / |  
| ------ | -------- | ----------  | ------- |  
| 姓名 | 陈雨 | 意向职位 | 前端开发 |
| 状态| 在职，观望 | 相关工作经验 | 四年 | 
|性别 | 男  | 城市 | 上海 |

<br />


- [基本资料](#基本资料)
- [工作经历](#工作经历)
  - [上海众多美网络科技有限公司（人人视频）](#上海众多美网络科技有限公司人人视频)
  - [上海麒谋投资管理有限公司](#上海麒谋投资管理有限公司)
- [相关技能](#相关技能)
- [项目经历](#项目经历)
  - [番茄电影](#番茄电影)
  - [前端组件库](#前端组件库)
  - [资源管理中心](#资源管理中心)
  - [BFF项目](#bff项目)
- [个人项目](#个人项目)
  - [vue-float-action-button](#vue-float-action-button)
  - [vue-dialog-x](#vue-dialog-x)
  - [flutter-danmaku](#flutter-danmaku)
  - [蜻蜓解析助手](#蜻蜓解析助手)



<br />

# 工作经历

## 上海众多美网络科技有限公司（人人视频）
2018.04 - 至今 (前端方向
1. 负责运营类活动、App内页、小程序开发（Vue技术栈）
2. 负责公司基于Eggjs、Typescript、MongoDB的BFF层设计开发。基于APIDOC的相关文档维护。以及运营类活动的接口开发。
3. 前端组件库的设计、开发以及维护
4. 基于VuePress的前端组件库文档的编写以及维护

2020.04 - 至今 (Flutter方向
1. 负责Flutter项目业务需求
2. 负责基于Flutter-Redux技术的状态管理设计与实现
3. 负责页面基类的设计与维护
4. 负责部分公共组件的抽离

## 上海麒谋投资管理有限公司
2016.08 - 2018.02
1. 负责公司基于cordova技术的混合应用开发
2. 负责产品性能的优化 负责产品缓存相关的设计
3. 基于ECharts数据类图表的开发

# 相关技能

1. Typescript Dart JavaScript
2. Vue Flutter Eggjs Nodejs 小程序啥的
3. SQLite MongoDB Redis MySQL
4. Redux Vuex
5. 单元测试 集成测试 GitHub CI Gitlab CI Jenkins
6. VuePress ApiDoc

# 项目经历

## 番茄电影
基于Flutter Flutter-Redux SQLite Dio 等相关技术开发的跨平台应用
1. 设计并实现基于Redux技术的全局状态管理。并应用与用户模块，历史记录模块，下载模块，全局配置开关等相关模块。
2. 使用SQLite技术实现本地历史记录相关功能，设计电影与集表并编写相关语句实现历史记录模块的记录展示与查询功能
3. 基于FutureBuilder优化启动流程，区分启动前必须初始化和启动后初始化。
4. 参与设计Tabbar，结合Redux实现动态底部栏更新
5. 设计开发页面基类。囊括加载状态，Appbar，空态页，埋点，ScrollController，分页数据 等统一维护状态
6. 封装ListView GredView 部分业务组件。
7. 编写iOS Platform的相关event channel
8. 参与业务需求开发

## 前端组件库
发布在公司内搭建的私有NPM仓库，通过VuePress编写相关文档，实现及时预览 && 试用的功能。囊括近30个前端业务组件，大量与客户端交互的JSBridge协议，以及常用的工具类&&函数。

1. 基于VuePress的文档编写，借助VuePress与Vue的完美结合，提供及时预览以及试用。
2. 大量业务组件，囊括海报，评论，up主，徽标等等等等。
3. 大量与客户端通过JSBridge方式交互的函数
4. 部分各项目间通用的js函数

目前各大项目不用重复编写样式，各个部门可以通过VuePress提供的文档来联调协议。大大提升了工作效率以及降低部门间沟通成本

## 资源管理中心
基于腾讯云cos，Mongodb，Eggjs，Vue，Vuex相关技术开发的网盘web应用 实现一个树形结构可无限扩展的文件管理系统
1. 文件模块 文件夹模块 通过关联字段 将每个文件夹 以链表的结构串联起来，再将每个文件关联到各个文件夹 以实现无限扩展的文件管理系统 再以此基础上开发文件移动 重命名等扩展
功能
2. 关键字搜索 通过mongodb模糊匹配查询实现关键字搜索功能
3. 上传模块 使用腾讯云COS SDK 读取上传进度 通过Vuex状态管理实现文件上传队列 通过HTML5拖放标准实现拖拽上传 多图上传
4. 登录模块 使用LDAP协议处理登录 JWT技术实现用户认证鉴权
5. 回收站模块
所有删除都为逻辑删除 删除后的资源都会回到回收站，回收站中的资源删除都为物理删除 即删除记录并且删除COS存储文件
6. 分享模块 通过生成分享ID 用户进入后可查看指定文件夹下的内容

相关优化 使用IntersectionObserver API优化 由于设计成网盘形式所以不可避免的出现单个文件夹内容过多的情况，当单页展示文件数量大于一定值时，由于DOM树过大过深导致的页面卡
顿。 通过使用IntersectionObserver API将屏幕不可见DOM隐藏并使用一个简单的DIV填充，即可解决DOM树带来的卡顿
避免部门间传输文件受到其它云盘或在线传输的带宽限制

## BFF项目
基于Eggjs Mongodb Typescript的BFF项目。 用于承接公司内运营类活动需求 以快速开发为准则 开发了大量可复用的活动模块 包括抽奖模块 模板配置 广告配置等 以及一些活动业务代码 项目使用apidoc作为文档生
成工具 egg-validate作为字段验证 ali-node作为监控手段 使用gitlab-cli作为自动构建发布工具 至今已经上线数个长期业务，数十个短期活动 降低开发成本 减少沟通成本

① H5配置中心 该平台以灵活配置广告位为核心目的，设计了配置广告位的功能，包含按ID获取广告、按广告位以及排序来获取广告列表、配置广告展示时间、分端展示、配置标题 封面 广告位 等功能
让市场部门可以灵活配置H5展示内容

② 通用抽奖模块
用于抽奖活动的通用抽奖模块，包含了
奖项配置、奖品配置、概率配置、奖池配置、库存配置
用于运营部门的抽奖需求

③ CDN图床
内网使用的CDN图床客户端 基于七牛CDN开发 实现拖拽上传 多图上传 图片预览等功能

由服务端通过内网调用的方式提供部分用户资源接口。由前端负责具体业务的实现。


# 个人项目

## vue-float-action-button


<a href="https://www.npmjs.com/package/vue-float-action-button">
		<img src="https://img.shields.io/npm/dm/vue-float-action-button.svg" alt="Monthly downloads">
	</a></a>

  <a href='https://coveralls.io/github/a62527776a/vue-floating-action-button?branch=master'><img src='https://coveralls.io/repos/github/a62527776a/vue-floating-action-button/badge.svg?branch=master' alt='Coverage Status' /></a><a href="https://github.com/a62527776a/vue-floating-action-button/issues">
    <img src="https://img.shields.io/github/issues-closed-raw/a62527776a/vue-floating-action-button.svg" />
  </a><a href="https://github.com/a62527776a/vue-floating-action-button">
    <img src="https://img.shields.io/github/stars/a62527776a/vue-floating-action-button.svg?style=social" />
  </a>
个人开发的vue组件 文档清晰 API设计良好 使用VuePress编写文档
https://github.com/a62527776a/vue-fab

## vue-dialog-x

<hr />

  <a href='https://coveralls.io/github/a62527776a/vue-dialog-x?branch=master'><img src='https://coveralls.io/repos/github/a62527776a/vue-dialog-x/badge.svg?branch=master' alt='Coverage Status' /></a>
  <a href="https://www.npmjs.com/package/vue-dialog-x"><img src="https://img.shields.io/npm/dm/vue-dialog-x.svg" /></a>
  <br>
  </a>
  <img alt="npm type definitions" src="https://img.shields.io/npm/types/vue-dialog-x">
  <img alt="npm" src="https://img.shields.io/npm/v/vue-dialog-x">  
  
支持Promise的iOS样式风格的弹窗提示 基于Typescript开发 已在公司内长期稳定使用
https://github.com/a62527776a/vue-dialog-x


## flutter-danmaku
<hr />
<br />

<img src="https://socialify.git.ci/flutte-danmaku/flutter_danmaku/image?description=1&descriptionEditable=a%20normal%20danmaku%20by%20flutter.%20live%20comment%20hohoho%F0%9F%98%8A%20all%20in%20dart.&font=Source%20Code%20Pro&language=1&pattern=Overlapping%20Hexagons&theme=Light&submit" alt="flutter_danmaku" width="400" />  <br />
[![Coverage Status](https://coveralls.io/repos/github/flutte-danmaku/flutter_danmaku/badge.svg?branch=dev)](https://coveralls.io/github/flutte-danmaku/flutter_danmaku?branch=dev)
![Flutter CI](https://github.com/flutte-danmaku/flutter_danmaku/workflows/Flutter%20CI/badge.svg)
[![pub package](https://img.shields.io/pub/v/flutter_danmaku.svg)](https://pub.dev/packages/flutter_danmaku)

Flutter 弹幕项目， 纯Dart开发，实现市面成熟弹幕所有功能

https://github.com/flutte-danmaku/flutter_danmaku
******

## 蜻蜓解析助手
结合youtube-dl以及you-get的短视频解析网站 前端使用Vue技术栈 后端使用Typescript Eggjs Mongodb Redis Nginx 等相关技术
相关功能:
1. 用户单日限额功能 记录用户每次调用成功记录 调用前通过$gt等条件查询语句查询当日解析次数实现用户单日限额功能。 未登录用户 通过Redis缓存记录每个请求IP的解析次数 实现单
个IP一定时间内最大调用次数限制
2. 用户令牌 使用JWT技术 记录UserId 权限等级等敏感信息 通过Redis记录UserId以及生成的Token 实现用户认证机制 以及其衍生的单点登录 刷新token等操作
3. 权限模块 使用Eggjs中间件为每个接口分配不同的权限调用等级 通过读取token Payload 中的权限标识符 来区分不同接口的可调用等级
4. 收藏夹模块 通过Mongodb数据库的联表查询来实现展示每个收藏夹关联的各个用户 每个收藏关联的各个收藏夹
5. 解析模块 使用shelljs调用you-get 以及 youtube-dl 以及大量的兼容性代码 实现两者的通用调用 为了更好的解析体验 通过异步调用 防止线程阻塞 使用Promise包裹，实现双SDK同时调
用 先完成解析先返回结果
6. 切换节点功能 通过配置Shadowsock客户端，在不同端口启动不同的代理 让用户可以选择不同国家或者地区来解析 实现绕过地域限制
7. 签到 VIP 历史记录 等基于MongoDB数据库的业务功能

相关优化 ① 全站静态资源CDN化 ②首页接口Redis缓存 ③webpack等相关优化

基于以上功能开发web版，小程序版
由于没啥收入 就关站了