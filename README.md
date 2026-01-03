# 外卖订餐系统（sky-take-out）
[![GitHub license](https://img.shields.io/github/license/valicuausmonidri/takeaway-ordering-system)](https://github.com/valicuausmonidri/takeaway-ordering-system)
> 一款基于Java（Spring Boot）+ Vue + 微信小程序的全栈外卖订餐系统，支持用户点餐、商家管理、订单处理、菜品维护等核心功能。

## 核心特性
*   特性 1：用户端（微信小程序）- 菜品浏览、购物车、下单支付、订单查询
*   特性 2：管理端（Vue+TS）- 商家信息配置、菜品管理、订单审核、数据统计
*   特性 3：后端服务（Spring Boot）- 接口提供、权限控制、数据库交互、业务逻辑处理
*   特性 4：数据库支持 - 基于MySQL搭建，提供完整sql脚本快速初始化数据

## 快速开始

### 先决条件
*   JDK 8+ / 11+（后端运行必备）
*   Node.js 14+（前端管理端运行必备）
*   微信开发者工具（小程序端调试必备）
*   Git
*   MySQL 5.7+（数据库存储必备）
*   Docker (可选，快速部署)

### 安装与运行
1.  `git clone https://github.com/valicuausmonidri/takeaway-ordering-system.git`
2.  `cd takeaway-ordering-system`
3.  后端运行（进入backend文件夹）：
    *   执行 `sky_take_out.sql` 初始化数据库
    *   配置application.yml中的数据库连接（账号/密码）
    *   `mvn clean install` 打包项目
    *   `java -jar target/sky-take-out.jar` 启动后端服务
4.  管理端运行（进入frontend-admin文件夹）：
    *   `npm install` 安装依赖
    *   `npm run dev` / `npm start` 启动管理端
5.  小程序端运行（进入frontend-mini文件夹）：
    *   打开微信开发者工具，导入该文件夹
    *   配置小程序AppID，直接编译运行

## 项目结构
├── backend/          # 后端核心代码（Spring Boot）
├── frontend-admin/   # 管理端前端代码（Vue+TS）
├── frontend-mini/    # 微信小程序前端代码
├── docs/             # 项目文档（毕业设计、开题报告、论文等）
├── README.md         # 项目自述文件
└── sky_take_out.sql  # 数据库初始化脚本

## 如何贡献
我们欢迎贡献！请阅读我们的 [贡献指南](CONTRIBUTING.md)。

## 许可证
本项目基于 [MIT](LICENSE) 许可证开源。

## 获取帮助
*   [提交 Issue](https://github.com/valicuausmonidri/takeaway-ordering-system/issues) - 报告Bug或提出新特性
*   沟通平台 - 微信（可补充个人微信/项目沟通群链接）