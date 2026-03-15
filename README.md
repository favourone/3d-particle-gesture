# 🌌 3D Particle Gesture Engine (3D 粒子手势交互系统)

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Click%20Here-success?style=for-the-badge&logo=vercel)](https://favourone.github.io/3d-particle-gesture/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> 一个基于 Three.js 和 MediaPipe 的纯前端 3D 实时手势交互引擎。无需任何外部穿戴设备，仅通过普通摄像头即可在浏览器中“隔空”操控万千星辰。

## 🔗 在线体验 (Live Demo)

👉 **[点击这里直接在浏览器中运行](https://favourone.github.io/3d-particle-gesture/)** *(⚠️ 注意：本项目完全基于纯前端本地算力运行，请允许浏览器调用摄像头权限。推荐在 PC 端全屏获得最佳沉浸体验。)*

## ✨ 核心特性 (Features)

* **🖐️ AI 空间追踪**：集成 Google MediaPipe Hands，实时捕捉手掌坐标与双指开合距离，映射为 3D 空间中的平移与缩放。
* **🌟 发光粒子引擎**：渲染 20,000+ 高帧率粒子，采用自绘 Canvas 径向渐变纹理与 `AdditiveBlending` 加色混合，消除黑边，呈现极致赛博朋克发光质感。
* **🧬 纯数学几何演算**：摒弃静态加载模型，内置 **螺旋星系 (Galaxy)**、**心跳波段 (Heart)** 和 **双螺旋 (DNA)** 三种由纯参数方程实时生成的全息形态。
* **🌊 弹簧物理阻尼 (Lerp)**：深度优化手势交互体验，引入线性插值算法过滤摄像头高频抖动，粒子运动如流体般丝滑跟手。

## 🛠 技术栈 (Tech Stack)

* **Three.js (WebGL)** - 3D 场景与粒子渲染引擎
* **MediaPipe Hands** - 实时计算机视觉与手势关键点追踪
* **lil-gui** - 极简现代调试控制面板
* **HTML5 / WebGL** - 纯原生单文件构建，零构建工具依赖

## 🚀 本地运行 (Local Development)

由于浏览器对 getUserMedia (摄像头调用) 的安全限制，本地运行需开启 HTTP 服务，**请勿直接双击打开 HTML 文件**。

1. 克隆本仓库：

    git clone https://github.com/favourone/3d-particle-gesture.git

2. 启动本地服务（使用 Python）：

    python -m http.server 3000

3. 浏览器访问 http://localhost:3000 即可体验。

## 📝 博客解析

详细的开发思路与底层算法拆解（包含径向渐变纹理、加色混合、Lerp 阻尼算法等），请阅读我的技术博客：
👉 **[手撕“赛博朋克”级 Web 交互：Three.js + AI 视觉打造隔空手势控制的 3D 粒子系统](https://blog.csdn.net/2501_91104204/article/details/159081389)**

---

**如果这个项目对你有启发，或者觉得视觉效果还不错，欢迎点右上角给一个 ⭐️ Star！**
