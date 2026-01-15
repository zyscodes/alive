# Alive

> **Keep it that way.**
>
> *Status: Demo / Experimental*

[🇨🇳 中文说明](#-alive-中文说明) | [🇺🇸 English](#-introduction)

---

## 🟢 Introduction

**Alive** is a minimalist, browser-based **Dead Man's Switch**.

It serves as a passive monitoring system for your digital existence. You set a check-in interval (e.g., 7 days). As long as you return to tap **"I'M ALIVE"**, the system resets. If the countdown reaches zero, Alive assumes you are no longer responsive and triggers the **Handover Protocol**—releasing your pre-encrypted digital notes (wills, passwords, secrets) to designated contacts.

**⚠️ DISCLAIMER:** This is a **frontend-only demonstration**. Data is stored locally in your browser (`LocalStorage`). No real emails are sent unless you configure your own API keys. **Do not rely on this for life-critical situations.**

### ✨ Features

* **❤️ The Pulse:** A visceral, beating visual indicator of your status.
* **⏳ Countdown Logic:** Automatic calculation of your next required check-in time.
* **🔐 Local Encryption:** All notes ("Handover Data") are stored locally on your device.
* **🔥 Burn Effect:** A unique visual effect for destroying unwanted data permanently.
* **📱 Mobile-First:** Designed to function like a native app. Supports "Add to Home Screen" (PWA-like experience) with haptic feedback.
* **🌑 Cyberpunk Aesthetics:** Pure black OLED-friendly UI with immersive animations.

### 🚀 Quick Start

#### 1. Run Locally
Simply download the `index.html` file and open it in any modern browser (Chrome, Safari, Edge).

#### 2. Deploy (Recommended)
To experience the full mobile UI, deploy it to **GitHub Pages** or **Vercel**:

1.  Fork this repository.
2.  Go to **Settings** -> **Pages** -> **Deploy from Main Branch**.
3.  Open the URL on your phone.

### ⚙️ Configuration

To enable real email sending via **EmailJS**, configure the `EMAIL_CONFIG` object in `index.html`.

### 📄 License

MIT License.

---

## 🔴 Alive (中文说明)

> **保持这种状态。**

[Go to English](#-introduction)

**Alive** 是一个极简主义的网页版**数字死手开关 (Dead Man's Switch)**。

它是一个为你设计的被动状态监测器。设定一个周期（例如 7 天），只要你在此期间点击 **“I'M ALIVE”**（我还在），倒计时就会重置。一旦倒计时归零，系统将判定你失联（或已故），并自动触发 **Handover（交代）** 协议，将你预存的遗嘱、密码或秘密分发给指定联系人。

**⚠️ 郑重声明：** 本项目目前仅为**纯前端演示 (Demo)**。所有数据仅存储在您的浏览器本地 (`LocalStorage`)，且在未配置 API Key 的情况下不会发送真实邮件。**请勿将其用于真正的生命托付。**

### ✨ 核心功能

* **❤️ 脉搏视觉：** 模拟心跳的呼吸动效，直观展示存活状态。
* **⏳ 倒计时机制：** 自动计算下一次必须签到的截止时间。
* **🔐 本地加密：** 所有的嘱托数据都存储在本地，不上传服务器。
* **🔥 焚毁特效：** 删除数据时伴随震撼的视觉销毁动画。
* **📱 移动端原生感：** 专为手机设计，支持震动反馈、防误触、深色模式。
* **🌑 黑镜美学：** 纯黑 OLED 风格 UI，沉浸式体验。

### 🚀 快速开始

#### 1. 本地运行
下载 `index.html` 文件，直接用浏览器（Chrome/Safari）打开即可。

#### 2. 部署（推荐）
为了获得最佳的手机体验，建议部署到 **GitHub Pages**：
1. Fork 本仓库。
2. 进入 Settings -> Pages -> Deploy from Main Branch。
3. 用手机访问生成的链接，并“添加到主屏幕”。

### 📄 许可证

MIT License.
