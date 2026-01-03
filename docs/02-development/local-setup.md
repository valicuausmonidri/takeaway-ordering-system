# 本地开发环境搭建指南
## 1. 后端环境搭建（Spring Boot）
### 前置条件
- 已安装 JDK 8+（推荐1.8）、MySQL 5.7+、Maven 3.6+、IntelliJ IDEA（或Eclipse）
### 详细步骤
1. 克隆仓库到本地：  
   `git clone httpsgithub.comvalicuausmonidritakeaway-ordering-system.git`
2. 初始化数据库：
   - 打开MySQL客户端（如Navicat），创建数据库`sky_take_out`（编码格式：utf8mb4）；
   - 执行`backendsky_take_out.sql`脚本，自动创建表结构和初始化数据（如测试菜品、管理员账号）。
3. 配置后端项目：
   - 用IDEA打开`backend`文件夹，等待Maven自动下载依赖（若依赖下载慢，可配置阿里云镜像）；
   - 打开`srcmainresourcesapplication.yml`，修改数据库连接配置：
     ```yaml
     spring
       datasource
         url jdbcmysqllocalhost3306sky_take_outuseSSL=false&serverTimezone=UTC
         root
         123456