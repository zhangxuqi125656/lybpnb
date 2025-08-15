# 抽奖网页应用

## 项目概述
这是一个基于Web的抽奖应用，具有以下特点：
- 设置10份抽奖额度及2个中奖名额
- 实现具备唯一性的中奖核销功能
- 使用Firebase实现不同用户间的数据同步
- 部署至GitHub Pages后可直接访问使用

## 技术栈
- 前端：HTML, CSS, JavaScript, Tailwind CSS, Font Awesome
- 后端：Firebase Realtime Database
- 部署：GitHub Pages

## 功能介绍
1. **抽奖功能**：用户可参与一次抽奖，系统随机产生中奖结果
2. **核销功能**：中奖用户可使用唯一核销码兑换奖品
3. **数据同步**：所有用户数据存储在Firebase云端数据库，确保数据一致性
4. **响应式设计**：适配各种屏幕尺寸的设备

## 使用说明
1. 访问网页后，点击"立即抽奖"按钮参与抽奖
2. 抽奖结束后，查看结果
3. 若中奖，妥善保管您的核销码
4. 进入"中奖核销"页面，输入核销码进行兑换

## Firebase配置指南
1. 访问[Firebase控制台](https://console.firebase.google.com/)
2. 创建新项目
3. 在项目设置中获取您的Firebase配置信息
4. 替换`lottery.html`文件中的Firebase配置：
```javascript
const firebaseConfig = {
    apiKey: "YOUR_API_KEY",
    authDomain: "YOUR_AUTH_DOMAIN",
    databaseURL: "YOUR_DATABASE_URL",
    projectId: "YOUR_PROJECT_ID",
    storageBucket: "YOUR_STORAGE_BUCKET",
    messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
    appId: "YOUR_APP_ID"
};
```
5. 启用Firebase Realtime Database

## 部署步骤
1. 将代码提交至GitHub仓库
2. 在仓库设置中启用GitHub Pages
3. 选择主分支作为来源
4. 访问生成的GitHub Pages URL

## 开发计划
1. 添加用户认证功能
2. 优化抽奖动画效果
3. 添加奖品管理功能
4. 增加活动统计和数据分析

## 注意事项
- 本应用使用localStorage存储用户标识，在隐私模式下可能无法正常工作
- 请确保正确配置Firebase，否则数据同步功能将无法使用
- 为保证公平性，每个用户仅限参与一次抽奖

© 2023 抽奖网页应用. 保留所有权利.