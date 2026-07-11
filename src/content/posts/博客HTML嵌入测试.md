---
title: 嵌入HTML测试
published: 2026-07-11 15:00:00
tags: [博客,测试]
category: 博客
draft: false
---

## 1. 呼吸脉冲圆环

<div align="center">
  <div style="width: 80px; height: 80px; border-radius: 50%; background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); animation: pulse 2s ease-in-out infinite; margin: 20px auto;"></div>
</div>

<style>
@keyframes pulse {
  0%, 100% { transform: scale(1); opacity: 1; box-shadow: 0 0 0 0 rgba(102, 126, 234, 0.7); }
  50% { transform: scale(1.1); opacity: 0.8; box-shadow: 0 0 0 20px rgba(102, 126, 234, 0); }
}
</style>

---

## 2. 渐变文字流光

<div align="center">
  <h2 style="font-size: 2.5em; background: linear-gradient(90deg, #ff6b6b, #feca57, #48dbfb, #ff9ff3, #ff6b6b); background-size: 200% auto; -webkit-background-clip: text; -webkit-text-fill-color: transparent; animation: shine 3s linear infinite;">
    ✨ 流光溢彩 ✨
  </h2>
</div>

<style>
@keyframes shine {
  to { background-position: 200% center; }
}
</style>

---

## 3. 悬浮卡片

<div align="center" style="perspective: 1000px; margin: 30px;">
  <div style="width: 280px; height: 160px; background: linear-gradient(135deg, #11998e, #38ef7d); border-radius: 16px; display: flex; align-items: center; justify-content: center; color: white; font-size: 1.5em; font-weight: bold; box-shadow: 0 10px 30px rgba(0,0,0,0.2); animation: float 3s ease-in-out infinite; cursor: pointer; transition: transform 0.3s;">
    🚀 悬浮卡片
  </div>
</div>

<style>
@keyframes float {
  0%, 100% { transform: translateY(0) rotateX(0); }
  50% { transform: translateY(-15px) rotateX(5deg); }
}
</style>

---

## 4. 加载动画

<div align="center" style="margin: 30px;">
  <div style="display: inline-block; width: 50px; height: 50px; border: 4px solid #f3f3f3; border-top: 4px solid #3498db; border-radius: 50%; animation: spin 1s linear infinite;"></div>
  <p style="color: #666; margin-top: 10px;">加载中...</p>
</div>

<style>
@keyframes spin {
  0% { transform: rotate(0deg); }
  100% { transform: rotate(360deg); }
}
</style>

---

## 5. 打字机效果

<div align="center" style="margin: 30px;">
  <p style="font-family: monospace; font-size: 1.2em; color: #2c3e50; border-right: 2px solid #2c3e50; white-space: nowrap; overflow: hidden; animation: typing 4s steps(20) infinite, blink 0.7s step-end infinite;">
    Hello, World! 🌍
  </p>
</div>

<style>
@keyframes typing {
  0% { width: 0; }
  50% { width: 200px; }
  100% { width: 200px; }
}
@keyframes blink {
  50% { border-color: transparent; }
}
</style>

---

## 6. 弹跳小球

<div align="center" style="margin: 30px; height: 100px;">
  <div style="width: 30px; height: 30px; background: #e74c3c; border-radius: 50%; animation: bounce 1s ease-in-out infinite;"></div>
</div>

<style>
@keyframes bounce {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-40px); }
}
</style>

---

> 💡 **提示**：以上动效使用纯 CSS `@keyframes` 实现，无需 JavaScript，兼容大多数支持 HTML 渲染的 Markdown 平台（如 GitHub、GitLab、Notion 等部分支持）。
使用说明：
将上述内容保存为 .md 文件，在支持 HTML 渲染的 Markdown 查看器中即可看到动效
大部分平台（如 GitHub）出于安全考虑会过滤掉 <style> 标签，建议将 style 改为内联 style 属性配合部分动画
如果是自建博客或文档站点，完整代码可以完美运行
我用在 GitHub pages astro firefly主题里的
编辑
复制
分享
思考已完成
搜索网页
Astro Firefly theme GitHub Pages astro firefly theme markdown animation
20 个结果
混合内联样式与 Tailwind 类实现动画
针对 Astro Firefly 主题，这里提供一段可直接粘贴到文章 .md 文件里的动效文本。Firefly 基于 Astro + Tailwind CSS，支持原生 HTML 嵌入，且适配亮暗模式。
Markdown
复制
代码
预览
---
title: 动效展示
published: 2026-07-11
description: 在 Firefly 主题中嵌入 HTML 动效
tags: [Astro, Firefly, 动效]
category: 前端
draft: false
---

## 🎆 萤火虫主题动效合集

以下动效均使用原生 HTML + CSS，可直接嵌入 Firefly 的 Markdown 文章中。

---

### 1. 呼吸脉冲

<div align="center" style="margin: 2rem 0;">
  <div style="width: 80px; height: 80px; border-radius: 50%; background: linear-gradient(135deg, #f59e0b, #ec4899); animation: firefly-pulse 2s ease-in-out infinite; box-shadow: 0 0 20px rgba(245, 158, 11, 0.5);"></div>
</div>

---

### 2. 流光文字

<div align="center" style="margin: 2rem 0;">
  <h2 style="font-size: 2rem; font-weight: 800; background: linear-gradient(90deg, #0ea5e9, #8b5cf6, #ec4899, #0ea5e9); background-size: 300% 100%; -webkit-background-clip: text; -webkit-text-fill-color: transparent; animation: firefly-flow 4s linear infinite;">
    Firefly Theme ✨
  </h2>
</div>

---

### 3. 悬浮卡片

<div align="center" style="margin: 2rem 0; perspective: 1000px;">
  <div style="width: 260px; height: 140px; background: linear-gradient(135deg, #10b981, #06b6d4); border-radius: 16px; display: flex; align-items: center; justify-content: center; color: white; font-size: 1.25rem; font-weight: 700; box-shadow: 0 20px 40px rgba(0,0,0,0.15); animation: firefly-float 3s ease-in-out infinite;">
    🚀 悬浮卡片
  </div>
</div>

---

### 4. 旋转加载

<div align="center" style="margin: 2rem 0;">
  <div style="width: 48px; height: 48px; border: 4px solid #e5e7eb; border-top: 4px solid #3b82f6; border-radius: 50%; animation: firefly-spin 1s linear infinite;"></div>
  <p style="margin-top: 12px; color: #6b7280; font-size: 0.875rem;">加载中...</p>
</div>

---

### 5. 弹跳小球

<div align="center" style="margin: 2rem 0; height: 100px;">
  <div style="width: 32px; height: 32px; background: #ef4444; border-radius: 50%; animation: firefly-bounce 1.2s ease-in-out infinite;"></div>
</div>

---

### 6. 打字机效果

<div align="center" style="margin: 2rem 0;">
  <p style="font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, monospace; font-size: 1.125rem; color: #374151; border-right: 2px solid #374151; white-space: nowrap; overflow: hidden; display: inline-block; animation: firefly-typing 3s steps(16) infinite, firefly-blink 0.8s step-end infinite;">
    Hello, Firefly! 🌟
  </p>
</div>

---

### 7. 萤火虫粒子（契合主题）

<div align="center" style="margin: 2rem 0; position: relative; width: 100%; height: 120px; overflow: hidden; border-radius: 12px; background: linear-gradient(to bottom, #0f172a, #1e293b);">
  <div style="position: absolute; width: 6px; height: 6px; background: #fbbf24; border-radius: 50%; box-shadow: 0 0 10px #fbbf24; top: 20%; left: 20%; animation: firefly-fly 4s ease-in-out infinite;"></div>
  <div style="position: absolute; width: 4px; height: 4px; background: #a78bfa; border-radius: 50%; box-shadow: 0 0 8px #a78bfa; top: 60%; left: 50%; animation: firefly-fly 5s ease-in-out infinite 1s;"></div>
  <div style="position: absolute; width: 5px; height: 5px; background: #34d399; border-radius: 50%; box-shadow: 0 0 10px #34d399; top: 40%; left: 80%; animation: firefly-fly 6s ease-in-out infinite 2s;"></div>
  <div style="position: absolute; width: 3px; height: 3px; background: #f472b6; border-radius: 50%; box-shadow: 0 0 6px #f472b6; top: 70%; left: 30%; animation: firefly-fly 4.5s ease-in-out infinite 0.5s;"></div>
  <p style="position: relative; z-index: 1; color: #e2e8f0; font-size: 1rem; line-height: 120px; text-align: center; font-weight: 600;">流萤飞舞 ✨</p>
</div>

---

<style>
@keyframes firefly-pulse {
  0%, 100% { transform: scale(1); opacity: 1; }
  50% { transform: scale(1.15); opacity: 0.7; }
}
@keyframes firefly-flow {
  0% { background-position: 0% 50%; }
  100% { background-position: 300% 50%; }
}
@keyframes firefly-float {
  0%, 100% { transform: translateY(0) rotateX(0); }
  50% { transform: translateY(-12px) rotateX(4deg); }
}
@keyframes firefly-spin {
  0% { transform: rotate(0deg); }
  100% { transform: rotate(360deg); }
}
@keyframes firefly-bounce {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-35px); }
}
@keyframes firefly-typing {
  0% { width: 0; }
  50% { width: 180px; }
  100% { width: 180px; }
}
@keyframes firefly-blink {
  50% { border-color: transparent; }
}
@keyframes firefly-fly {
  0%, 100% { transform: translate(0, 0) scale(1); opacity: 0.8; }
  25% { transform: translate(20px, -15px) scale(1.2); opacity: 1; }
  50% { transform: translate(-10px, 10px) scale(0.8); opacity: 0.6; }
  75% { transform: translate(15px, 5px) scale(1.1); opacity: 0.9; }
}
</style>