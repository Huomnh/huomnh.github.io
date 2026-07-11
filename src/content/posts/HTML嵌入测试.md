---
title: 嵌入HTML测试
published: 2026-07-11 15:00:00
description: 
image: 
tags: [博客,测试]
category: 博客
draft: false
---

## 一、普通Markdown内容
这是普通文字，**加粗**、*斜体*、[博客首页](https://www.huomnh.me)

## 二、行内HTML（直接嵌在文字里，无需空行）
普通文字 <span style="color:#ff6b6b;font-weight:bold;">红色加粗文字</span> 继续正常书写。

## 三、块级HTML（前后必须空一行，带自定义样式卡片）

<div style="background: #fff7ed; padding: 16px; border-radius: 12px; border-left: 4px solid #f97316;">
  <h3 style="margin-top:0;color:#c2410c;">硬件DIY小提示</h3>
  <p style="font-size:14px;line-height:1.7;">
    STM32F407搭配ESP8266接线时，记得共地，否则串口数据乱码。<br>
    HX711称重模块供电建议3.3V，5V容易漂移。
  </p>
  <img src="/public/demo-hardware.jpg" width="100%" style="border-radius:6px;margin-top:8px;">
</div>

## 四、HTML表格
<table border="1" cellpadding="6" cellspacing="0" width="100%">
  <tr style="background:#f0f0f0;">
    <th>模块</th>
    <th>供电电压</th>
    <th>通讯方式</th>
  </tr>
  <tr>
    <td>ESP8266</td>
    <td>3.3V</td>
    <td>串口</td>
  </tr>
  <tr>
    <td>TB6612</td>
    <td>4.5~15V</td>
    <td>GPIO</td>
  </tr>
</table>

## 五、彩色提示框
<div style="background:#ecfccb;padding:12px;border-radius:8px;">
✅ 成功提示：Astro md 文件原生支持HTML，无需额外转义
</div>

<div style="background:#fee2e2;padding:12px;border-radius:8px;">
⚠️ 注意：不要用 ```html 代码块包裹HTML，否则只会展示源码不渲染
</div>