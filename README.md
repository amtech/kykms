
![KYKMS](./Docs/Pics/logo_keyi.png "科亿文档知识库管理系统")

科亿知识库 KY KMS
===============
当前最新版本： V0.0.1（发布日期：20220808）

项目介绍：
-----------------------------------

<h3 align="center">面向常用文档的知识库管理系统</h3>

科亿知识库 KY KMS 既是一款知识库，同时也是一款易于上手的文档管理工具！

在信息化时代，我们日常工作中产生大量的文档。我们积累下来的文档，是一笔巨大的财富，但文档越多，我们在其中找到我们所需要文档的时间成本越高。

我们面对大量的文档一筹莫展，就好像面前座立着一金山，但我们却不知道如何开采金子。

`科亿知识库宗旨是:` 文档简单整理，知识创造价值


适用项目
-----------------------------------
科亿知识库，可以应用在任何需要进行常用文档整理、分类、归集、检索的地方，尤其适合知识密集型单位/历史文档丰富的单位。

交流互动
-----------------------------------
- 官方站点 ：  [http://www.kykms.cn](http://www.kykms.cn)
- 在线演示 ：  [http://www.kykms.cn:90](http://www.kykms.cn:90) 账号：admin/123456
- QQ ： 22247537
- Mail : hnliuwx#tom.com
- github: [https://github.com/mahonelau/kykms](https://github.com/mahonelau/kykms)
- gitee: [https://gitee.com/kyxxjs/km_community](https://gitee.com/kyxxjs/km_community)
- 微信 ： 如果你有任何产品上的想法、意见或建议，或商务上的合作需求，请扫码添加我们微信进一步沟通：

![微信](./Docs/Pics/wechat.jpg)

版权声明
-----------------------------------
开源不代表免费，科亿遵循 GPL-3.0 开源协议发布，并提供技术交流学习，但 绝不允许修改后和衍生的代码做为闭源的商业软件发布和销售 ！ 如果需要将本产品在本地进行任何附带商业化性质行为使用， 请联系项目负责人进行商业授权 ，以遵守 GPL 协议保证您的正常使用。 
目前在国内 GPL 协议具备合同特征，是一种民事法律行为 ，属于我国《合同法》调整的范围。科亿项目团队保留一切诉讼权利。 科亿开源团队拥有对本开源协议的最终解释权。


为什么选择KY KMS?
-----------------------------------
科亿知识库基于强大的Elasticsearch检索引擎技术构建，检索能力强大，支持最全面的检索特性，同时检索性能卓越，可以无限可能的集群扩展，支持高达百亿级别的记录数量。
在关系数据库方面支持mysql与oracle，更多的数据库支持在开发中。
![KY KMS](./Docs/Pics/advantage_kms.png)
![KY KMS](./Docs/Pics/process.png)



技术架构：
-----------------------------------
#### 技术亮点
- 主流技术，生态完善，易于维护
- 前后端分离，接口文档清晰，易于二次开发
- 后端采用ES搜索引擎，可以按需实行分部署部署
 
#### 开发环境
- 语言：Java 8
- IDE(JAVA)： IDEA / Eclipse安装lombok插件 
- IDE(前端)： WebStorm 或者 IDEA
- 依赖管理：Maven
- 数据库：MySQL5.7+  &  Oracle 11g & Sqlserver2017
- 缓存：Redis
- Node Js: 10.0 +
- Npm: 5.6.0+
- Yarn: 1.21.1+ 

#### 后端
- 基础框架：Spring Boot 2.3.5.RELEASE
- 持久层框架：Mybatis-plus 3.4.1
- 检索引擎：ElasticSearch 7.6.1
- 文档处理与转换： Libre Office 7.1.4
- 文本提取：Tika 1.17
- 安全框架：Apache Shiro 1.7.0，Jwt 3.11.0  
- 数据库连接池：阿里巴巴Druid 1.1.22 
- 缓存框架：redis 
- 日志打印：logback 
- 其他：fastjson，poi，Swagger-ui，quartz, lombok（简化代码）等。


#### 前端
 
- [Vue 2.6.10](https://cn.vuejs.org/),[Vuex](https://vuex.vuejs.org/zh/),[Vue Router](https://router.vuejs.org/zh/)
- [Axios](https://github.com/axios/axios)
- [ant-design-vue](https://vuecomponent.github.io/ant-design-vue/docs/vue/introduce-cn/)
- [webpack](https://www.webpackjs.com/),[yarn](https://yarnpkg.com/zh-Hans/)
- [vue-cropper](https://github.com/xyxiao001/vue-cropper) - 头像裁剪组件
- [@antv/g2](https://antv.alipay.com/zh-cn/index.html) - Alipay AntV 数据可视化图表
- [Viser-vue](https://viserjs.github.io/docs.html#/viser/guide/installation)  - antv/g2 封装实现
- eslint，[@vue/cli 3.2.1](https://cli.vuejs.org/zh/guide)

### 功能模块
```
├─检索首页
│  ├─普通检索
│  ├─高级检索
│  ├─文档预览
│  ├─文档分类
│  ├─知识专题
│  ├─高频访问文档
│  ├─热词统计
│  ├─热门专题统计
├─系统管理
│  ├─用户管理
│  ├─角色管理
│  ├─菜单管理
│  ├─权限设置（支持按钮权限、数据权限）
│  ├─表单权限（控制字段禁用、隐藏）
│  ├─部门管理 
├─文件管理
│  ├─草稿文件上传
│  ├─文档编辑
│  ├─收藏夹
│  ├─待审核文件
│  ├─已审核文件 
│  ├─文件统计 
├─配置管理
│  ├─知识专题定义
│  ├─文档属性定义
├─日志
│  ├─文档操作记录
│  ├─系统日志 
└─其他模块
   └─更多功能开发中。。
   
```
 
项目下载和运行
----
开发环境准备与运行，请参考：开发环境准备与运行.md
- 默认登录账号： admin/123456


系统效果
----

##### 公共检索
检索首页
![检索首页](./Docs/Pics/search_home.png)
检索结果
![检索结果](./Docs/Pics/search_result.png)
高级检索
![高级检索](./Docs/Pics/search_advance.png)
知识专题
![知识专题](./Docs/Pics/km_topic.png)


##### 管理后台
热词统计
![](./Docs/Pics/home.png)
批量上传
![](./Docs/Pics/upload.png)
编辑
![知识专题](./Docs/Pics/edit.png)


附属文档
----
- [Ant Design Vue](https://www.antdv.com/docs/vue/introduce-cn)


特别鸣谢
-----------------------------------
本项目采用Jeecg-boot开发框架，Jeecg-boot，一款优秀的后台管理快速开发框架，让你更专注于业务开发的实现。
- JeecgBoot： [http://doc.jeecg.com](http://doc.jeecg.com)


## 捐赠 

如果觉得还不错，请作者喝杯咖啡鼓励一下吧，敲代码不容易 ☺
![](./Docs/Pics/QR_pay.jpg)


