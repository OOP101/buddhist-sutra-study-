<div align="center">

![Static](https://img.shields.io/badge/技术栈-原生HTML%2FCSS%2FJS-blue) ![Pages](https://img.shields.io/badge/GitHub%20Pages-已启用-brightgreen) ![License](https://img.shields.io/badge/经典原文-Public%20Domain-lightgrey)

# 金刚经 · 楞严咒 学习网站

> 素净排版 · 全文注音 · 自动朗读 · 经文详解

</div>

一个单文件佛教经典学习网站，收录 **《金刚般若波罗蜜经》全文（三十二品）** 与 **《大佛顶首楞严神咒》全文（五会四百二十七句）**，以素净的纸墨风格呈现，供读诵、听经、抄经与深入研读之用。

## 在线预览

**https://oop101.github.io/buddhist-sutra-study-/**

> 若链接打不开，说明尚未开启 GitHub Pages：仓库 → Settings → Pages → Source 选 `Deploy from a branch` → Branch 选 `main`、文件夹选 `/ (root)` → Save，等待一至二分钟即可访问。

## 功能特性

- **经文全文** — 金刚经三十二品完整收录，楞严咒五会及咒心逐句排版
- **自动朗读** — 一键连读当前页经文/咒语/详解，逐段高亮跟随滚动；自动选用最自然的中文语音（Edge 下为微软神经网络语音），遇「（三称）」自动读诵三遍；基于浏览器 Web Speech API，零服务端依赖（建议 Edge / Chrome）
- **全文注音** — 楞严咒每句咒文附注音，可一键开合，不影响原文排版
- **章节导航** — 桌面端左侧常驻目录，窄屏为浮动面板；金刚经诸品、楞严咒五会及咒心一键直达
- **经文详解** — 第三标签页收录金刚经总论、重点品讲解、楞严咒缘起功德与修持要点
- **字号调节** — 三档缩放，便于读诵抄写
- **阅读进度** — 顶部进度条，实时显示阅读位置
- **整页滚动** — 标签栏吸顶，长文阅读更顺畅

## 经文详解内容

### 金刚经

- 经名释义：金刚 · 般若 · 波罗蜜
- 核心思想：应无所住而生其心、凡所有相皆是虚妄
- 历史背景与翻译流传
- 重点品讲解：第一品（法会因由）、第三品（大乘正宗）、第四品（妙行无住）、第五品（如理实见）、第十品（庄严净土）、第十四品（离相寂灭）、第十八品（一体同观）、第二十六品（法身非相）、第三十二品（应化非真）

### 楞严咒

- 出处与缘起（阿难摩登伽女之难）
- 五会结构：毗卢遮那佛法会、释迦牟尼佛法会、观世音菩萨法会、刚藏菩萨法会、文殊师利菩萨法会
- 咒心逐句略释
- 持诵功德与注意事项

## 目录结构

```
.
├── index.html   # 单文件应用：经文 + 注音 + 朗读 + 导航 + 详解（约 96KB）
└── README.md    # 项目说明
```

## 本地使用

直接双击打开 `index.html` 即可（朗读功能建议使用 Edge / Chrome 浏览器），或部署至任意静态托管平台（GitHub Pages、Vercel、CloudStudio 等）。

```bash
# 本地预览（Python 方式）
python -m http.server 8000
# 浏览器访问 http://localhost:8000
```

## 技术栈

- 原生 HTML / CSS / JavaScript（零构建、零框架）
- 思源宋体（Noto Serif SC）经 Google Fonts 加载，离线时自动回退系统宋体
- CSS 变量实现主题与字号缩放（`--font-scale` / `--pinyin-display`）
- CSS 伪元素 `attr(data-pinyin)` 实现注音叠加
- Web Speech API（`speechSynthesis`）实现自动朗读与逐段高亮
- 桌面端双栏布局（左侧目录 + 右侧正文），1200px / 640px 断点响应式

## 许可证

文本内容：佛教经典原文属公共领域（Public Domain）。
页面代码与详解内容：保留所有权利（All Rights Reserved）。
