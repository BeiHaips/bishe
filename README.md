# 基于SpringBoot的酒店信息管理系统的设计与实现

![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=java)
![SpringBoot](https://img.shields.io/badge/SpringBoot-6DB33F?style=flat-square&logo=springboot)
![Vue](https://img.shields.io/badge/Vue-4FC08D?style=flat-square&logo=vue.js)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql)

**广东培正学院本科毕业设计**  
**作者**：彭省  
**指导老师**：张可姗 助教  
**完成日期**：2026年3月

---

## 一、项目简介

这是一个**B/S架构的前后端分离酒店信息管理系统**，专为中小型酒店设计，实现了从客房管理、在线预订到订单处理、入住退房、评价管理的**全流程信息化**。

系统彻底解决了传统手工登记、Excel管理带来的**效率低、易出错、房态不同步**等问题，极大提升了酒店运营效率和客户体验。

**一句话总结**：  
**让中小型酒店告别纸笔，实现实时房态 + 自动化订单 + 可视化后台管理**。

---

## 二、技术栈

| 类别     | 技术                  |
|----------|-----------------------|
| **后端** | Java + SpringBoot     |
| **前端** | Vue                   |
| **数据库** | MySQL              |
| **服务器** | Tomcat 9.0         |
| **架构**   | B/S 前后端分离        |
| **开发工具** | IDEA + Navicat Premium |

---

## 三、系统功能

### 用户端（普通用户）
- 注册 / 登录
- 浏览客房类型与房间信息
- 在线提交预订申请（选择入住/离店日期）
- 查看历史订单及订单详情
- 申请退房（系统自动计算金额）
- 修改个人信息 / 密码
- 联系管理员

### 管理端（管理员）
- 房型信息管理
- 房间信息管理（增删改查）
- 订单管理（审核预订、办理入住/退房）
- 用户管理
- 评论信息管理

---

## 四、系统架构

系统采用**前后端分离**的经典 B/S 架构：

详细架构图见论文第10页 **图4-1 系统架构设计图**。

---

## 五、数据库设计

系统包含 **用户、管理员、房型、房间、订单、评论** 等核心实体。  
详细的**实体-关系图（E-R图）** 和 **数据表结构** 见论文第11-13页 **4.3 数据库设计**。

---

## 六、运行方式

### 1. 后端运行（SpringBoot）
1. 导入 MySQL 数据库脚本
2. 修改 `application.yml` 中的数据库账号、密码、端口
3. 用 IDEA 打开后端项目，运行 `Application.java`
4. 后端默认端口：**8080**

### 2. 前端运行（Vue）
```bash
cd frontend          # 进入前端文件夹
npm install
npm run dev
