Alive (活着)
Keep it that way.

Status: Demo / Experimental

English | 中文

🟢 Introduction
Alive is a minimalist, browser-based Dead Man's Switch (死手开关).

It serves as a passive monitoring system for your digital existence. You set a check-in interval (e.g., 7 days). As long as you return to tap "I'M ALIVE", the system resets. If the countdown reaches zero, Alive assumes you are no longer responsive and triggers the Handover Protocol—releasing your pre-encrypted digital notes (wills, passwords, secrets) to designated contacts.

⚠️ DISCLAIMER: This is a frontend-only demonstration. Data is stored locally in your browser (LocalStorage). No real emails are sent unless you configure your own API keys. Do not rely on this for life-critical situations.

✨ Features
❤️ The Pulse: A visceral, beating visual indicator of your status.

⏳ Countdown Logic: Automatic calculation of your next required check-in time.

🔐 Local Encryption: All notes ("Handover Data") are stored locally on your device.

🔥 Burn Effect: A unique visual effect for destroying unwanted data permanently.

📱 Mobile-First: Designed to function like a native app. Supports "Add to Home Screen" (PWA-like experience) with haptic feedback.

🌑 Cyberpunk Aesthetics: Pure black OLED-friendly UI with immersive animations.

🚀 Quick Start
1. Run Locally
Simply download the index.html file and open it in any modern browser (Chrome, Safari, Edge).

2. Deploy (Recommended)
To experience the full mobile UI, deploy it to GitHub Pages or Vercel:

Fork this repository.

Go to Settings -> Pages -> Deploy from Main Branch.

Open the URL on your phone.

⚙️ Configuration (Advanced)
By default, the app runs in Demo Mode (simulating email sending). To make it functional, you need to integrate EmailJS.

Register at EmailJS.com.

Create a Service (e.g., Gmail) and a Template.

Open index.html and locate the CONFIG section:

JavaScript

// Replace with your actual keys
const EMAIL_CONFIG = {
    PUBLIC_KEY: "YOUR_PUBLIC_KEY_HERE",
    SERVICE_ID: "YOUR_SERVICE_ID_HERE",
    TEMPLATE_ID: "YOUR_TEMPLATE_ID_HERE"
};
Template Variables: In your EmailJS template, use these variables:

{{to_email}}: The recipient's address.

{{subject}}: Note subject.

{{message}}: The note content.

📱 Mobile Experience
For the best experience on iOS/Android:

Open the site in Safari/Chrome.

Tap Share -> Add to Home Screen.

Launch from the home screen.

The address bar will be hidden.

Full-screen immersion enabled.

Haptic feedback enabled.

🛡️ Privacy & Security
No Database: We do not own a server. We do not see your data.

Local Storage: Everything lives in your browser's localStorage.

Risk: If you clear your browser cache/data, your notes will be lost.

Risk: Anyone with physical access to your unlocked phone can see your notes.

📄 License
MIT License. Feel free to fork, modify, and keep yourself alive.

<a name="chinese"></a>

Alive (中文说明)
保持这种状态。

Alive 是一个极简主义的网页版数字死手开关。

它是一个为你设计的被动状态监测器。设定一个周期（例如 7 天），只要你在此期间点击 “I'M ALIVE”（我还在），倒计时就会重置。一旦倒计时归零，系统将判定你失联（或已故），并自动触发 Handover（交代） 协议，将你预存的遗嘱、密码或秘密分发给指定联系人。

⚠️ 郑重声明： 本项目目前仅为纯前端演示 (Demo)。所有数据仅存储在您的浏览器本地 (LocalStorage)，且在未配置 API Key 的情况下不会发送真实邮件。请勿将其用于真正的生命托付。

✨ 核心功能
❤️ 脉搏视觉： 模拟心跳的呼吸动效，直观展示存活状态。

⏳ 倒计时机制： 自动计算下一次必须签到的截止时间。

🔐 本地加密： 所有的嘱托数据都存储在本地，不上传服务器。

🔥 焚毁特效： 删除数据时伴随震撼的视觉销毁动画。

📱 移动端原生感： 专为手机设计，支持震动反馈、防误触、深色模式。

🌑 黑镜美学： 纯黑 OLED 风格 UI，沉浸式体验。

⚙️ 如何使其真正工作？
默认代码处于 演示模式。如果你希望倒计时结束后真的发送邮件，需要配置 EmailJS：

去 EmailJS 注册账号。

获取你的 Public Key, Service ID 和 Template ID。

修改 index.html 中的配置区域：

JavaScript

const EMAIL_CONFIG = {
    PUBLIC_KEY: "你的_KEY",
    SERVICE_ID: "你的_SERVICE_ID",
    TEMPLATE_ID: "你的_TEMPLATE_ID"
};
注意：由于这是纯前端项目，只有当某人（如你的信任联系人）打开这个网页时，触发逻辑才会执行。它无法在浏览器关闭时自动后台发送。

📱 最佳食用方式
建议将本网页**“添加到主屏幕”**使用：

iOS: Safari -> 分享按钮 -> 添加到主屏幕。

Android: Chrome -> 菜单 -> 添加到主屏幕。

这样可以获得无地址栏的沉浸式全屏体验。
