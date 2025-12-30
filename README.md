# HarmonyOS-Health-Assistant
HarmonyOS Software Development - HealthAssistant
# HarmonyOS-Software-Development-Health-Assistant

基于鸿蒙OS的轻量级健康管理应用，实现健康监测、运动指导、饮食管理、习惯养成等核心功能，达成"麻雀虽小，五脏俱全"的开发目标。

## 项目简介
- **开发环境**：DevEco Studio 4.0+、鸿蒙OS 6.0+、Java Development Kit 11+
- **项目周期**：2周
- **代码量目标**：2.5万行
- **核心定位**：面向个人用户的分布式健康助手，支持本地数据存储与鸿蒙原生能力调用

## 核心功能模块
1. **健康监测（SRS_HM01）**：步数统计、心率监测、睡眠追踪、健康评分（0-100分）与趋势分析
2. **运动指导（SRS_SP02）**：3类训练计划、50个标准动作库、动作识别与计时提醒
3. **饮食管理（SRS_DI03）**：饮食记录、热量计算、营养分析（蛋白质/脂肪/碳水比例）
4. **习惯养成（SRS_HA04）**：打卡跟踪、健康提醒、本地排行榜、成就系统
5. **系统管理（SRS_SY05）**：用户注册登录、个人资料管理、BMI计算、数据备份导出

## 技术架构
- **架构分层**：表示层（UI组件/交互处理器）→ 业务逻辑层（核心服务）→ 数据访问层（本地存储/传感器适配）→ 鸿蒙OS平台层
- **核心依赖**：鸿蒙传感器API、VisionKit（动作识别）、Preferences/RelationalStore（本地存储）
- **关键算法**：健康评分加权算法（运动30%+饮食30%+作息20%+习惯20%）、动作识别对比算法

## 快速开始
1. 克隆仓库：`git clone https://github.com/USERNAME/HarmonyOS-Software-Development-Health-Assistant.git`
2. 打开DevEco Studio导入项目，配置鸿蒙OS开发环境
3. 连接鸿蒙真机或启动模拟器，编译运行
