---
title: 嵌入HTML测试
published: 2026-07-11 15:00:00
tags: [博客,测试]
category: 博客
draft: false
---

## 一、普通Markdown基础内容
这是常规文本，**加粗文字**、*斜体文字*，博客首页跳转链接：[https://www.huomnh.me](https://www.huomnh.me)

## 二、悬浮变色行内文字动效
<span style="font-size:18px; font-weight:bold; color:#666; transition:color 0.4s ease;"
onmouseover="this.style.color='#f97316'"
onmouseout="this.style.color='#666'">
鼠标放上来自动变色的文字
</span>

## 三、悬浮上浮阴影硬件信息卡片（核心动效）

<div style="background: #fff7ed; padding: 16px; border-radius: 12px; border-left: 4px solid #f97316; transition: all 0.3s ease; cursor: pointer;"
onmouseover="this.style.transform='translateY(-6px)'; this.style.boxShadow='0 8px 20px rgba(249, 115, 22, 0.25)'"
onmouseout="this.style.transform='translateY(0)'; this.style.boxShadow='none'">
  <h3 style="margin-top:0;color:#c2410c;">STM32F407 + ESP8266 接线关键提示</h3>
  <p style="font-size:14px;line-height:1.7;">
    1. 单片机与WiFi模块必须共地，否则串口数据乱码<br>
    2. HX711称重模块仅支持3.3V供电，5V会造成读数漂移<br>
    3. TB6612驱动输入电压区间4.5~15V，不要超压
  </p>
</div>

## 四、鼠标悬停高亮HTML表格
<table border="1" cellpadding="6" cellspacing="0" width="100%" style="margin-top:16px;">
  <tr style="background:#f0f0f0;">
    <th>硬件模块</th>
    <th>标准供电</th>
    <th>通讯方式</th>
  </tr>
  <tr style="transition: background 0.25s ease;"
  onmouseover="this.style.background='#ffedd5'"
  onmouseout="this.style.background='transparent'">
    <td>ESP8266-01S</td>
    <td>3.3V</td>
    <td>硬件串口</td>
  </tr>
  <tr style="transition: background 0.25s ease;"
  onmouseover="this.style.background='#ffedd5'"
  onmouseout="this.style.background='transparent'">
    <td>HX711称重</td>
    <td>3.3V</td>
    <td>SPI类串行</td>
  </tr>
  <tr style="transition: background 0.25s ease;"
  onmouseover="this.style.background='#ffedd5'"
  onmouseout="this.style.background='transparent'">
    <td>TB6612FNG电机驱动</td>
    <td>4.5~15V</td>
    <td>GIO控制</td>
  </tr>
  <tr style="transition: background 0.25s ease;"
  onmouseover="this.style.background='#ffedd5'"
  onmouseout="this.style.background='transparent'">
    <td>OpenMV视觉模块</td>
    <td>5V</td>
    <td>串口/USB</td>
  </tr>
</table>

## 五、两种动效提示框（成功+警告）
<div style="margin-top:20px;background:#ecfccb;padding:12px;border-radius:8px;transition:all 0.3s;"
onmouseover="this.style.boxShadow='0 4px 12px rgba(132, 204, 22, 0.2)'"
onmouseout="this.style.boxShadow='none'">
✅ 操作成功提示：md文件原生支持内联HTML过渡动效，无需修改文件后缀
</div>

<div style="margin-top:12px;background:#fee2e2;padding:12px;border-radius:8px;transition:all 0.3s;"
onmouseover="this.style.boxShadow='0 4px 12px rgba(248, 113, 113, 0.2)'"
onmouseout="this.style.boxShadow='none'">
⚠️ 重要注意：纯md文件不能写&lt;style&gt;关键帧循环动画，循环闪烁浮动请改用.mdx格式
</div>

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