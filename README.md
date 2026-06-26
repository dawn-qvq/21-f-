# 21-f-
本项目基于 STM32F103C8T6 主控，融合 K210 AI视觉、八路灰度循迹、TB6612电机驱动、编码器反馈、HC-05蓝牙通信及OLED显示 等模块，实现了 2021年全国大学生电子设计竞赛F题智能送药小车。CSDN链接：https://blog.csdn.net/2301_79957440/article/details/162345381?spm=1001.2014.3001.5501
🚗 Intelligent Medicine Delivery Robot (2021 National Undergraduate Electronic Design Contest - Problem F)

基于 STM32F103C8T6 + K210 + 八路灰度 + 串级PID 实现的智能送药小车（2021 年全国大学生电子设计竞赛 F 题）

📖 项目简介 | Introduction

本项目基于 STM32F103C8T6 作为主控制器，结合 K210 AI 视觉模块、八路灰度循迹、TB6612 双路电机驱动、编码器闭环控制、HC-05 蓝牙通信以及 OLED 显示，完成了 2021 年全国大学生电子设计竞赛 F 题《智能送药小车》 的完整实现。

系统采用有限状态机（FSM）+ 串级 PID 控制算法 + K210 视觉导航，实现自动识别目标、路径规划、精准循迹、路口转向、送药及原路径返回等功能，具有较高的稳定性和扩展性。

This project implements the 2021 National Undergraduate Electronic Design Contest (NUEDC) Problem F - Intelligent Medicine Delivery Robot, based on STM32F103C8T6 and K210 AI Vision. It integrates line tracking, visual navigation, cascade PID control, encoder feedback, Bluetooth communication, and OLED display to achieve autonomous medicine delivery and return.

✨ 项目特点 | Features
🚗 STM32F103C8T6 主控
👁 K210 AI 视觉数字识别
📍 八路灰度高精度循迹
⚙ 串级 PID（位置环 + 速度环）
🔄 编码器闭环速度控制
🧭 状态机路径规划（FSM）
↩ 支持送药 + 自动返回
📟 OLED 实时状态显示
📶 HC-05 蓝牙无线通信
🔋 TB6612FNG 双路电机驱动
🛠️ 硬件组成 | Hardware
STM32F103C8T6
K210 Vision Module
8-Channel Gray Sensor
TB6612FNG Motor Driver
DC Geared Motor with Encoder
HC-05 Bluetooth Module
0.96" OLED Display
Lithium Battery Power Supply
📂 项目结构 | Project Structure
MedicineDeliveryCar/
│
├── USER/                // 主程序
├── SYSTEM/              // 系统驱动
├── HARDWARE/
│   ├── Gray             // 八路灰度
│   ├── Encoder          // 编码器
│   ├── Motor            // 电机驱动
│   ├── PID              // PID控制
│   ├── OLED             // OLED显示
│   ├── HC05             // 蓝牙通信
│   ├── Serial           // K210通信
│   └── Timer            // 定时器
│
├── K210/                // K210视觉程序
├── Docs/                // 项目文档
└── README.md
🚀 功能演示 | Functions

✅ 数字识别导航

✅ 八路灰度循迹

✅ 十字路口识别

✅ 自动路径规划

✅ 左转 / 右转 / 掉头

✅ 编码器闭环控制

✅ 串级 PID 调速

✅ 自动送药

✅ 原路径返回

📚 技术栈 | Tech Stack
STM32 Standard Peripheral Library
C Language
UART Communication
PWM Motor Control
Encoder Feedback
Cascade PID Control
Finite State Machine (FSM)
Computer Vision (K210)
📖 项目解析

本项目配套完整开发教程，详细介绍：

硬件设计
电路连接
软件架构
状态机设计
串级 PID 控制
八路灰度循迹
K210 通信
调试经验
完整源码解析

📌 CSDN 项目详解：

👉 https://blog.csdn.net/2301_79957440/article/details/162345381?spm=1001.2014.3001.5501

⭐ Star History

如果本项目对你的学习有所帮助，欢迎：

⭐ Star 本仓库

🍴 Fork 学习交流

🐞 提交 Issue

💡 提交 Pull Request

共同完善本项目，一起交流 STM32、电子设计竞赛及嵌入式开发经验！
