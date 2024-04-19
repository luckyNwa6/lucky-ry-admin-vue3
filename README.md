## 🐶 环境

推荐用nvm来控制node版本，使用pnpm 来管理包

```shell
nvm install 20.0.0
nvm use 20.0.0
npm i pnpm@8.6.0 -g
pnpm i
```

* nodejs > 16.18.0 && pnpm > 8.6.0 (强制使用pnpm)
* 演示地址【Vue3 + element-plus】：<http://dashboard-vue3.yudao.iocoder.cn>
* 演示地址【Vue3 + vben(ant-design-vue)】：<http://dashboard-vben.yudao.iocoder.cn>
* 演示地址【Vue2 + element-ui】：<http://dashboard.yudao.iocoder.cn>
* 启动文档：<https://doc.iocoder.cn/quick-start/>
* 视频教程：<https://doc.iocoder.cn/video/>


## 技术栈

| 框架                                                                   | 说明               | 版本     |
|----------------------------------------------------------------------|------------------|--------|
| [Vue](https://staging-cn.vuejs.org/)                                 | Vue 框架           | 3.3.8 |
| [Vite](https://cn.vitejs.dev//)                                      | 开发与构建工具          | 4.5.0  |
| [Element Plus](https://element-plus.org/zh-CN/)                      | Element Plus     | 2.4.2 |
| [TypeScript](https://www.typescriptlang.org/docs/)                   | JavaScript 的超集   | 5.2.2  |
| [pinia](https://pinia.vuejs.org/)                                    | Vue 存储库 替代 vuex5 | 2.1.7 |
| [vueuse](https://vueuse.org/)                                        | 常用工具集            | 10.6.1 |
| [vue-i18n](https://kazupon.github.io/vue-i18n/zh/introduction.html/) | 国际化              | 9.6.5  |
| [vue-router](https://router.vuejs.org/)                              | Vue 路由           | 4.2.5  |
| [unocss](https://uno.antfu.me/)                                      | 原子 css          | 0.57.4  |
| [iconify](https://icon-sets.iconify.design/)                         | 在线图标库            | 3.1.1  |
| [wangeditor](https://www.wangeditor.com/)                            | 富文本编辑器           | 5.1.23 |

## 开发工具

推荐 VS Code 开发，配合插件如下：

| 插件名                           | 功能                       |
|-------------------------------|--------------------------|
| TypeScript Vue Plugin (Volar) | 用于 TypeScript 的 Vue 插件  |
| Vue Language Features (Volar) | Vue3.0 语法支持              |
| unocss                        | unocss for vscode           |
| Iconify IntelliSense          | Iconify 预览和搜索           |
| i18n Ally                     | 国际化智能提示               |
| Stylelint                     | Css    格式化               |
| Prettier                      | 代码格式化                   |
| ESLint                        | 脚本代码检查                  |
| DotENV                        | env 文件高亮                 |

## 🔥 后端架构

支持 Spring Boot、Spring Cloud 两种架构：

① Spring Boot 单体架构：<https://github.com/YunaiV/ruoyi-vue-pro>

![架构图](/.image/common/ruoyi-vue-pro-architecture.png)

② Spring Cloud 微服务架构：<https://github.com/YunaiV/yudao-cloud>

![架构图](/.image/common/yudao-cloud-architecture.png)

## 内置功能

系统内置多种多种业务功能，可以用于快速你的业务系统：

* 系统功能
* 基础设施
* 工作流程
* 支付系统
* 会员中心
* 数据报表
* 商城系统
* 微信公众号
* ERP 系统
* CRM 系统

### 系统功能

|     | 功能    | 描述                              |
|-----|-------|---------------------------------|
|     | 用户管理  | 用户是系统操作者，该功能主要完成系统用户配置          |
| ⭐️  | 在线用户  | 当前系统中活跃用户状态监控，支持手动踢下线           |
|     | 角色管理  | 角色菜单权限分配、设置角色按机构进行数据范围权限划分      |
|     | 菜单管理  | 配置系统菜单、操作权限、按钮权限标识等，本地缓存提供性能    |
|     | 部门管理  | 配置系统组织机构（公司、部门、小组），树结构展现支持数据权限  |
|     | 岗位管理  | 配置系统用户所属担任职务                    |
| 🚀  | 租户管理  | 配置系统租户，支持 SaaS 场景下的多租户功能        |
| 🚀  | 租户套餐  | 配置租户套餐，自定每个租户的菜单、操作、按钮的权限       |
|     | 字典管理  | 对系统中经常使用的一些较为固定的数据进行维护          |
| 🚀  | 短信管理  | 短信渠道、短息模板、短信日志，对接阿里云、腾讯云等主流短信平台 |
| 🚀  | 邮件管理  | 邮箱账号、邮件模版、邮件发送日志，支持所有邮件平台       |
| 🚀  | 站内信   | 系统内的消息通知，提供站内信模版、站内信消息          |
| 🚀  | 操作日志  | 系统正常操作日志记录和查询，集成 Swagger 生成日志内容 |
| ⭐️  | 登录日志  | 系统登录日志记录查询，包含登录异常               |
| 🚀  | 错误码管理 | 系统所有错误码的管理，可在线修改错误提示，无需重启服务     |
|     | 通知公告  | 系统通知公告信息发布维护                    |
| 🚀  | 敏感词   | 配置系统敏感词，支持标签分组                  |
| 🚀  | 应用管理  | 管理 SSO 单点登录的应用，支持多种 OAuth2 授权方式 |
| 🚀  | 地区管理  | 展示省份、城市、区镇等城市信息，支持 IP 对应城市      |

![功能图](/.image/common/system-feature.png)

### 工作流程

|     | 功能    | 描述                                     |
|-----|-------|----------------------------------------|
| 🚀  | 流程模型  | 配置工作流的流程模型，支持文件导入与在线设计流程图，提供 7 种任务分配规则 |
| 🚀  | 流程表单  | 拖动表单元素生成相应的工作流表单，覆盖 Element UI 所有的表单组件 |
| 🚀  | 用户分组  | 自定义用户分组，可用于工作流的审批分组                    |
| 🚀  | 我的流程  | 查看我发起的工作流程，支持新建、取消流程等操作，高亮流程图、审批时间线    |
| 🚀  | 待办任务  | 查看自己【未】审批的工作任务，支持通过、不通过、转发、委派、退回等操作    |
| 🚀  | 已办任务  | 查看自己【已】审批的工作任务，未来会支持回退操作               |
| 🚀  | OA 请假 | 作为业务自定义接入工作流的使用示例，只需创建请求对应的工作流程，即可进行审批 |

![功能图](/.image/common/bpm-feature.png)

### 支付系统

|     | 功能   | 描述                        |
|-----|------|---------------------------|
| 🚀  | 商户信息 | 管理商户信息，支持 Saas 场景下的多商户功能  |
| 🚀  | 应用信息 | 配置商户的应用信息，对接支付宝、微信等多个支付渠道 |
| 🚀  | 支付订单 | 查看用户发起的支付宝、微信等的【支付】订单     |
| 🚀  | 退款订单 | 查看用户发起的支付宝、微信等的【退款】订单     |

ps：核心功能已经实现，正在对接微信小程序中...

### 基础设施

|    | 功能       | 描述                                           |
|----|----------|----------------------------------------------|
| 🚀 | 代码生成     | 前后端代码的生成（Java、Vue、SQL、单元测试），支持 CRUD 下载       |
| 🚀 | 系统接口     | 基于 Swagger 自动生成相关的 RESTful API 接口文档          |
| 🚀 | 数据库文档    | 基于 Screw 自动生成数据库文档，支持导出 Word、HTML、MD 格式      |
|    | 表单构建     | 拖动表单元素生成相应的 HTML 代码，支持导出 JSON、Vue 文件         |
| 🚀 | 配置管理     | 对系统动态配置常用参数，支持 SpringBoot 加载                 |
| ⭐️ | 定时任务     | 在线（添加、修改、删除)任务调度包含执行结果日志                     |
| 🚀 | 文件服务     | 支持将文件存储到 S3（MinIO、阿里云、腾讯云、七牛云）、本地、FTP、数据库等   |
| 🚀 | API 日志   | 包括 RESTful API 访问日志、异常日志两部分，方便排查 API 相关的问题   |
|    | MySQL 监控 | 监视当前系统数据库连接池状态，可进行分析SQL找出系统性能瓶颈              |
|    | Redis 监控 | 监控 Redis 数据库的使用情况，使用的 Redis Key 管理           |
| 🚀 | 消息队列     | 基于 Redis 实现消息队列，Stream 提供集群消费，Pub/Sub 提供广播消费 |
| 🚀 | Java 监控  | 基于 Spring Boot Admin 实现 Java 应用的监控           |
| 🚀 | 链路追踪     | 接入 SkyWalking 组件，实现链路追踪                      |
| 🚀 | 日志中心     | 接入 SkyWalking 组件，实现日志中心                      |
| 🚀 | 服务保障     | 基于 Redis 实现分布式锁、幂等、限流功能，满足高并发场景              |
| 🚀 | 日志服务     | 轻量级日志中心，查看远程服务器的日志                           |
| 🚀 | 单元测试     | 基于 JUnit + Mockito 实现单元测试，保证功能的正确性、代码的质量等    |

![功能图](/.image/common/infra-feature.png)

### 数据报表

|     | 功能    | 描述                 |
|-----|-------|--------------------|
| 🚀  | 报表设计器 | 支持数据报表、图形报表、打印设计等  |
| 🚀  | 大屏设计器 | 拖拽生成数据大屏，内置几十种图表组件 |

### 微信公众号

|     | 功能     | 描述                            |
|-----|--------|-------------------------------|
| 🚀  | 账号管理   | 配置接入的微信公众号，可支持多个公众号           |
| 🚀  | 数据统计   | 统计公众号的用户增减、累计用户、消息概况、接口分析等数据  |
| 🚀  | 粉丝管理   | 查看已关注、取关的粉丝列表，可对粉丝进行同步、打标签等操作 |
| 🚀  | 消息管理   | 查看粉丝发送的消息列表，可主动回复粉丝消息         |
| 🚀  | 自动回复   | 自动回复粉丝发送的消息，支持关注回复、消息回复、关键字回复 |
| 🚀  | 标签管理   | 对公众号的标签进行创建、查询、修改、删除等操作       |
| 🚀  | 菜单管理   | 自定义公众号的菜单，也可以从公众号同步菜单         |
| 🚀  | 素材管理   | 管理公众号的图片、语音、视频等素材，支持在线播放语音、视频 |
| 🚀  | 图文草稿箱  | 新增常用的图文素材到草稿箱，可发布到公众号         |
| 🚀  | 图文发表记录 | 查看已发布成功的图文素材，支持删除操作           |

### 商城系统

![功能图](/.image/common/mall-feature.png)

![功能图](/.image/common/mall-preview.png)

_前端基于 crmeb uniapp 经过授权重构，优化代码实现，接入芋道快速开发平台_

演示地址：<https://doc.iocoder.cn/mall-preview/>

### ERP 系统

![功能图](/.image/common/erp-feature.png)

演示地址：<https://doc.iocoder.cn/erp-preview/>

### CRM 系统

![功能图](/.image/common/crm-feature.png)

演示地址：<https://doc.iocoder.cn/crm-preview/>

## 🐷 演示图

### 系统功能

| 模块       | biu                         | biu                       | biu                      |
|----------|-----------------------------|---------------------------|--------------------------|
| 登录 & 首页  | ![登录](/.image/登录.jpg)       | ![首页](/.image/首页.jpg)     | ![个人中心](/.image/个人中心.jpg) |
| 用户 & 应用  | ![用户管理](/.image/用户管理.jpg)   | ![令牌管理](/.image/令牌管理.jpg) | ![应用管理](/.image/应用管理.jpg) |
| 租户 & 套餐  | ![租户管理](/.image/租户管理.jpg)   | ![租户套餐](/.image/租户套餐.png) | -                        |
| 部门 & 岗位  | ![部门管理](/.image/部门管理.jpg)   | ![岗位管理](/.image/岗位管理.jpg) | -                        |
| 菜单 & 角色  | ![菜单管理](/.image/菜单管理.jpg)   | ![角色管理](/.image/角色管理.jpg) | -                        |
| 审计日志     | ![操作日志](/.image/操作日志.jpg)   | ![登录日志](/.image/登录日志.jpg) | -                        |
| 短信       | ![短信渠道](/.image/短信渠道.jpg)   | ![短信模板](/.image/短信模板.jpg) | ![短信日志](/.image/短信日志.jpg) |
| 字典 & 敏感词 | ![字典类型](/.image/字典类型.jpg)   | ![字典数据](/.image/字典数据.jpg) | ![敏感词](/.image/敏感词.jpg)  |
| 错误码 & 通知 | ![错误码管理](/.image/错误码管理.jpg) | ![通知公告](/.image/通知公告.jpg) | -                        |

### 工作流程

| 模块      | biu                             | biu                             | biu                             |
|---------|---------------------------------|---------------------------------|---------------------------------|
| 流程模型    | ![流程模型-列表](/.image/流程模型-列表.jpg) | ![流程模型-设计](/.image/流程模型-设计.jpg) | ![流程模型-定义](/.image/流程模型-定义.jpg) |
| 表单 & 分组 | ![流程表单](/.image/流程表单.jpg)       | ![用户分组](/.image/用户分组.jpg)       | -                               |
| 我的流程    | ![我的流程-列表](/.image/我的流程-列表.jpg) | ![我的流程-发起](/.image/我的流程-发起.jpg) | ![我的流程-详情](/.image/我的流程-详情.jpg) |
| 待办 & 已办 | ![任务列表-审批](/.image/任务列表-审批.jpg) | ![任务列表-待办](/.image/任务列表-待办.jpg) | ![任务列表-已办](/.image/任务列表-已办.jpg) |
| OA 请假   | ![OA请假-列表](/.image/OA请假-列表.jpg) | ![OA请假-发起](/.image/OA请假-发起.jpg) | ![OA请假-详情](/.image/OA请假-详情.jpg) |

### 基础设施

| 模块            | biu                           | biu                         | biu                       |
|---------------|-------------------------------|-----------------------------|---------------------------|
| 代码生成          | ![代码生成](/.image/代码生成.jpg)     | ![生成效果](/.image/生成效果.jpg)   | -                         |
| 文档            | ![系统接口](/.image/系统接口.jpg)     | ![数据库文档](/.image/数据库文档.jpg) | -                         |
| 文件 & 配置       | ![文件配置](/.image/文件配置.jpg)     | ![文件管理](/.image/文件管理2.jpg)  | ![配置管理](/.image/配置管理.jpg) |
| 定时任务          | ![定时任务](/.image/定时任务.jpg)     | ![任务日志](/.image/任务日志.jpg)   | -                         |
| API 日志        | ![访问日志](/.image/访问日志.jpg)     | ![错误日志](/.image/错误日志.jpg)   | -                         |
| MySQL & Redis | ![MySQL](/.image/MySQL.jpg)   | ![Redis](/.image/Redis.jpg) | -                         |
| 监控平台          | ![Java监控](/.image/Java监控.jpg) | ![链路追踪](/.image/链路追踪.jpg)   | ![日志中心](/.image/日志中心.jpg) |

### 支付系统

| 模块      | biu                       | biu                             | biu                             |
|---------|---------------------------|---------------------------------|---------------------------------|
| 商家 & 应用 | ![商户信息](/.image/商户信息.jpg) | ![应用信息-列表](/.image/应用信息-列表.jpg) | ![应用信息-编辑](/.image/应用信息-编辑.jpg) |
| 支付 & 退款 | ![支付订单](/.image/支付订单.jpg) | ![退款订单](/.image/退款订单.jpg)       | ---                             |

### 数据报表

| 模块    | biu                             | biu                             | biu                                   |
|-------|---------------------------------|---------------------------------|---------------------------------------|
| 报表设计器 | ![数据报表](/.image/报表设计器-数据报表.jpg) | ![图形报表](/.image/报表设计器-图形报表.jpg) | ![报表设计器-打印设计](/.image/报表设计器-打印设计.jpg) |
| 大屏设计器 | ![大屏列表](/.image/大屏设计器-列表.jpg)   | ![大屏预览](/.image/大屏设计器-预览.jpg)   | ![大屏编辑](/.image/大屏设计器-编辑.jpg)         |
