---
title: 二次元图片网站
published: 2026-06-15
pinned: false
description: 一些免费的图片网站，大多需要英文搜索。
tags: [资源网站]
category: 工具
draft: false
image: ./cover_images/yinlang-1.avif
---

# 资源网站

## 🌟 综合推荐（含R18内容）

### Konachan（K站）
- **网址**：https://konachan.net/post
- **特点**：经典的二次元壁纸站，图片质量极高（很多4K+），标签系统完善，方便查找
- **注意**：分为SFW版和R18版，浏览时注意内容分级

### Gelbooru
- **网址**：https://gelbooru.com
- **特点**：海量二次元图片库，无需注册即可访问，基于标签搜索功能强大
- **注意**：包含成人向内容

### Anime-Pictures
- **网址**：https://anime-pictures.net
- **特点**：全球动漫爱好者共建的社区，收录超60万张作品，支持多语言
- **注意**：包含部分成人向内容

---

## 🖼️ 纯壁纸类（一般不含R18）

### Wallhaven
- **网址**：https://wallhaven.cc
- **特点**：全球最大壁纸库之一，资源极其丰富，支持最高8K分辨率，界面清爽
- **注意**：需要用英文关键词搜索，国内访问速度可能较慢

### 彼岸图网
- **网址**：http://www.netbian.com
- **特点**：国内综合性壁纸站，动漫分类资源丰富，支持免费无水印下载，可按分辨率筛选

### 2DWallpapers
- **网址**：http://www.2dwallpapers.com
- **特点**：专注动漫和游戏的壁纸站，以作品合集形式展示（鬼灭、海贼、崩坏等），完全免费无需注册

### ACG66
- **网址**：https://www.acg66.com
- **特点**：专注ACG领域，紧跟新番热度更新素材，分辨率多样适配不同设备

---

## 🆕 AI生成二次元类（完全免费商用）

### StockCake
- **网址**：https://stockcake.com
- **特点**：公共领域（CC0）图片站，**AI生成的二次元/动漫图片**，每日更新超300张，无需注册，可免费商用
- **优势**：完全的版权无忧，适合用于博客配图、视频素材等

---

## 📋 快速对比

| 网站 | 主要特点 | 是否含R18 | 国内访问 |
|:---|:---|:---|:---|
| Konachan | 高质量壁纸，标签完善 | 有 | 一般 |
| Gelbooru | 海量图片库，标签搜索 | 有 | 一般 |
| Anime-Pictures | 60万+作品，社区属性 | 有 | 一般 |
| Wallhaven | 全球最大壁纸库，8K | 较少 | 较慢 |
| 彼岸图网 | 国内站，中文友好 | 无 | 流畅 |
| 2DWallpapers | 作品合集展示 | 无 | 流畅 |
| ACG66 | 新番更新快 | 无 | 流畅 |
| StockCake | AI生成，免费商用 | 无 | 一般 |

---

💡 **建议**：如果你只是想找好看的壁纸或素材，优先试**彼岸图网**和**2DWallpapers**，国内访问流畅；如果追求最高画质，**Konachan**和**Wallhaven**质量最佳；如果用于博客配图需要避免版权问题，**StockCake**是最安全的选择。


# AVIF

**AVIF** 正在快速成为网页图片的主流格式，主要原因是它在 **体积、画质、功能** 三个维度上全面超越了传统的 PNG 和 JPG。

## AVIF 相比 PNG / JPG 的核心优势

| 对比维度 | JPG (JPEG) | PNG | AVIF |
|:---|:---|:---|:---|
| **压缩率** | 一般 | 差（无损压缩，体积大） | **极高**（比 JPG 小约 50%） |
| **透明通道** | ❌ 不支持 | ✅ 支持 | ✅ 支持 |
| **动画支持** | ❌ 不支持 | ❌ 不支持（有 APNG 但少见） | ✅ 支持（可替代 GIF） |
| **HDR/广色域** | ❌ 有限支持 | ❌ 不支持 | ✅ 支持 |
| **无损压缩** | ❌ 不支持 | ✅ 支持 | ✅ 支持（且体积更小） |

### 一句话总结
> **AVIF 能在保持相同画质的情况下，文件体积只有 JPG 的一半左右，比 PNG 小 80% 以上。**

---

## 实际效果对比（直观感受）

假设同一张高质量图片：

| 格式 | 文件大小 | 相对体积 | 画质 |
|:---|:---|:---|:---|
| PNG（无损） | 800 KB | 100% | 完美 |
| JPG（高质量，90%） | 200 KB | 25% | 较好 |
| AVIF（高质量） | **80 KB** | **10%** | 接近无损 |

**对博客的实际意义**：
- 网页加载速度提升明显（尤其是移动网络）
- 节省服务器流量（GitHub Pages 有带宽限制吗？没有，但用户加载更快）
- Google 搜索排名会奖励加载速度快的网站

---

## 举例：Netflix 的实测数据

Netflix 在 2020 年做过大规模对比测试：
- 将 JPG 图库换成 AVIF
- **相同画质下，AVIF 比 JPG 小 50%-70%**
- 用户带宽消耗减少，卡顿率下降

---

## AVIF 有什么缺点？

| 缺点 | 说明 | 影响程度 |
|:---|:---|:---|
| **兼容性** | 旧版浏览器（如 IE、老 Safari）不支持 | 逐渐改善，2025 年主流浏览器全支持 |
| **编解码速度** | 压缩/解压比 JPG 慢（服务器端影响大，用户端几乎无感） | 开发/构建时稍慢 |
| **工具支持** | Photoshop、Lightroom 等软件支持较晚（近年才加入） | 普通用户处理麻烦 |

### 当前浏览器支持情况（2025-2026）

- ✅ Chrome / Edge / Firefox / Opera：完全支持
- ✅ Safari（macOS 11+ / iOS 14+）：完全支持
- ❌ IE 11：不支持（但已淘汰）
- ⚠️ 部分旧版 Android WebView：可能不支持

---

## 博客中如何使用 AVIF？

### 方案一：手动转换（适合少量图片）

| 工具名称 | 类型 | 链接/获取方式 | 特点 |
| :--- | :--- | :--- | :--- |
| **Squoosh** | 在线网页 | https://squoosh.app | Google 出品，操作简单直观，可实时预览画质和体积变化，能直观看到 AVIF 的巨大优势（例如可将 3.3MB 原图压缩至约 378KB） |
| **avifenc** | 命令行工具 | GitHub: `AOMediaCodec/libavif` | 适合批量处理大量图片，官方编码器，功能强大 |
| **compressjpg.io** | 在线网页 | https://compressjpg.io/zh-CN | 支持 AVIF 等多种格式的批量压缩，可一次性处理多达 1000 张图片，方便快捷 |
| **FFmpeg** | 命令行工具 | 官网: ffmpeg.org | 处理能力强，特别适合将视频或动图转换为**动画 AVIF** 文件 |

> 💡 **简单上手**：对于博客上零散的几张图片，直接使用 **Squoosh** 网页版是最方便的选择——拖入图片、选择 AVIF 格式、调整质量、下载即可。

### 方案二：构建时自动转换（推荐）

在你的 Astro / Vite / Webpack 项目中安装插件：

```bash
# Astro 示例
npm install astro-avif
```

```js
// astro.config.mjs
import avif from 'astro-avif';

export default {
  integrations: [avif()]
}
```

### 方案三：使用 `<picture>` 标签提供降级方案

```html
<picture>
  <!-- 优先使用 AVIF -->
  <source srcset="image.avif" type="image/avif">
  <!-- 降级到 WebP（比 JPG 好） -->
  <source srcset="image.webp" type="image/webp">
  <!-- 最终降级到 JPG/PNG -->
  <img src="image.jpg" alt="description">
</picture>
```

这样 100% 兼容所有浏览器：支持 AVIF 的用 AVIF，不支持的自动降级。
