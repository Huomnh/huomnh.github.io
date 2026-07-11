---
title: 嵌入HTML测试
published: 2026-07-11 15:00:00
tags: [博客,测试]
category: 博客
draft: false
---

## 🎆 萤火虫主题动效合集

以下动效均使用原生 HTML + CSS，可直接嵌入 Firefly 的 Markdown 文章中。

---

### 1. 呼吸脉冲

&lt;div align="center" style="margin: 2rem 0;"&gt;
  &lt;div style="width: 80px; height: 80px; border-radius: 50%; background: linear-gradient(135deg, #f59e0b, #ec4899); animation: firefly-pulse 2s ease-in-out infinite; box-shadow: 0 0 20px rgba(245, 158, 11, 0.5);"&gt;&lt;/div&gt;
&lt;/div&gt;

---

### 2. 流光文字

&lt;div align="center" style="margin: 2rem 0;"&gt;
  &lt;h2 style="font-size: 2rem; font-weight: 800; background: linear-gradient(90deg, #0ea5e9, #8b5cf6, #ec4899, #0ea5e9); background-size: 300% 100%; -webkit-background-clip: text; -webkit-text-fill-color: transparent; animation: firefly-flow 4s linear infinite;"&gt;
    Firefly Theme ✨
  &lt;/h2&gt;
&lt;/div&gt;

---

### 3. 悬浮卡片

&lt;div align="center" style="margin: 2rem 0; perspective: 1000px;"&gt;
  &lt;div style="width: 260px; height: 140px; background: linear-gradient(135deg, #10b981, #06b6d4); border-radius: 16px; display: flex; align-items: center; justify-content: center; color: white; font-size: 1.25rem; font-weight: 700; box-shadow: 0 20px 40px rgba(0,0,0,0.15); animation: firefly-float 3s ease-in-out infinite;"&gt;
    🚀 悬浮卡片
  &lt;/div&gt;
&lt;/div&gt;

---

### 4. 旋转加载

&lt;div align="center" style="margin: 2rem 0;"&gt;
  &lt;div style="width: 48px; height: 48px; border: 4px solid #e5e7eb; border-top: 4px solid #3b82f6; border-radius: 50%; animation: firefly-spin 1s linear infinite;"&gt;&lt;/div&gt;
  &lt;p style="margin-top: 12px; color: #6b7280; font-size: 0.875rem;"&gt;加载中...&lt;/p&gt;
&lt;/div&gt;

---

### 5. 弹跳小球

&lt;div align="center" style="margin: 2rem 0; height: 100px;"&gt;
  &lt;div style="width: 32px; height: 32px; background: #ef4444; border-radius: 50%; animation: firefly-bounce 1.2s ease-in-out infinite;"&gt;&lt;/div&gt;
&lt;/div&gt;

---

### 6. 打字机效果

&lt;div align="center" style="margin: 2rem 0;"&gt;
  &lt;p style="font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, monospace; font-size: 1.125rem; color: #374151; border-right: 2px solid #374151; white-space: nowrap; overflow: hidden; display: inline-block; animation: firefly-typing 3s steps(16) infinite, firefly-blink 0.8s step-end infinite;"&gt;
    Hello, Firefly! 🌟
  &lt;/p&gt;
&lt;/div&gt;

---

### 7. 萤火虫粒子（契合主题）

&lt;div align="center" style="margin: 2rem 0; position: relative; width: 100%; height: 120px; overflow: hidden; border-radius: 12px; background: linear-gradient(to bottom, #0f172a, #1e293b);"&gt;
  &lt;div style="position: absolute; width: 6px; height: 6px; background: #fbbf24; border-radius: 50%; box-shadow: 0 0 10px #fbbf24; top: 20%; left: 20%; animation: firefly-fly 4s ease-in-out infinite;"&gt;&lt;/div&gt;
  &lt;div style="position: absolute; width: 4px; height: 4px; background: #a78bfa; border-radius: 50%; box-shadow: 0 0 8px #a78bfa; top: 60%; left: 50%; animation: firefly-fly 5s ease-in-out infinite 1s;"&gt;&lt;/div&gt;
  &lt;div style="position: absolute; width: 5px; height: 5px; background: #34d399; border-radius: 50%; box-shadow: 0 0 10px #34d399; top: 40%; left: 80%; animation: firefly-fly 6s ease-in-out infinite 2s;"&gt;&lt;/div&gt;
  &lt;div style="position: absolute; width: 3px; height: 3px; background: #f472b6; border-radius: 50%; box-shadow: 0 0 6px #f472b6; top: 70%; left: 30%; animation: firefly-fly 4.5s ease-in-out infinite 0.5s;"&gt;&lt;/div&gt;
  &lt;p style="position: relative; z-index: 1; color: #e2e8f0; font-size: 1rem; line-height: 120px; text-align: center; font-weight: 600;"&gt;流萤飞舞 ✨&lt;/p&gt;
&lt;/div&gt;

---

&lt;style&gt;
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
&lt;/style&gt;