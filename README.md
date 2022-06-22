## 项目简介
这个项目是一个大学生信息管理系统,提供用户级别的登录注册资料管理,信息查询,信息修改（管理员权利），简单的数据可视化分析等功能，也有基本的安全性保障*



* 优化数据表结构，对原有的表的部分字段进行了修改，并增加了title和grade两个表
* 优化sql语句效率
* 优化前端查询界面及查询方式，使其更加全面，对用户友好
* 更新登录界面记住密码的cookie设置
* 更新邮箱验证码服务，增加了验证码有效时间
* 优化源代码结构，增强了规范性和可拓展性



## 项目技术
### 前端
* 前端框架 : `layui`
* 数据可视化框架 : `echarts`

### 后端
* IOC容器 : `Spring`
* Web框架 : `SpringMVC`
* ORM框架 : `Mybatis`
* 日志框架 : `Log4j`
* 安全框架 : `Shiro`



## 项目结构
```
├─database                          // 数据库相关文件
│  ├─design				                  // 数据库设计
│  │  └─1
│  └─sql                            // 数据库初始化脚本文件
├─git_screenshot                    // 存放README.md 中的图片
├─src                               // 项目源代码目录
│  ├─main                           //源代码目录
│  │  ├─java
│  │  │  └─com
│  │  │      └─springmvc            // java代码目录
│  │  │          ├─controller       // 控制层
│  │  │          ├─dao              // 持久层
│  │  │          ├─dto              // 传输对象
│  │  │          ├─entity           // 实体类
│  │  │          ├─interceptor      // 拦截器
│  │  │          ├─log              // 日志管理
│  │  │          ├─service          // 服务层
│  │  │          │  └─impl          // 服务层接口实现
│  │  │          └─util             // 工具方法
│  │  ├─resources                   // 资源文件目录
│  │  │  └─com
│  │  │      └─springmvc
│  │  │          └─mapper           // mybatis对dao接口的xml实现
│  │  └─webapp                      // tomcat前端文件目录
│  │      ├─static                  // 静态资源
│  │      │  ├─custom               // 自定义静态资源
│  │      │  └─plugins              // 插件类静态资源
│  │      └─WEB-INF
│  │          └─page                // jsp页面目录 
│  └─test                           // 测试代码目录
├─README.md                         // help
└─pom.xml                           // maven依赖
```


## 运行指南
### 1 : 项目开发环境
- IDE : `IntelliJ IDEA 2018.1.7`
- 项目构建工具 : `Maven 3.x`
- 数据库 : `Mysql 8.0.13`
- JDK版本 : `jdk 1.8`
- Tomcat版本 : `Tomcat 8.x`
