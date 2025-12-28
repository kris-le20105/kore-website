# Kore Communication 官方網站

![Kore Communication](https://img.shields.io/badge/Kore-Communication-purple)
![React](https://img.shields.io/badge/React-18-blue)
![TypeScript](https://img.shields.io/badge/TypeScript-5-blue)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-3-cyan)

## 🌟 項目簡介

Kore Communication HK Limited（克珞傳播香港有限公司）官方網站。專注於 O2O 教師和 B2B SaaS 服務，為零售、服務、餐飲業商家提供專業的數字化解決方案。

**在線預覽：** https://camwpiygh2.skywork.website

## ✨ 主要功能

- 🎨 **現代化設計** - 紫白配色，專業優雅
- 📱 **響應式佈局** - 完美適配手機、平板、電腦
- 💬 **WhatsApp 整合** - 一鍵聯繫客服
- 🚀 **高性能** - Vite + React 快速加載
- ♿ **無障礙設計** - 符合 WCAG 標準
- 🎯 **SEO 優化** - 搜索引擎友好

## 📋 網站板塊

1. **英雄區** - 品牌展示與核心價值
2. **服務介紹** - 6 大核心服務項目
3. **服務流程** - 5 步驟完整流程
4. **為什麼選擇我們** - 6 大核心優勢
5. **成功案例** - 真實客戶案例展示
6. **常見問題** - 8 個精選 FAQ
7. **聯繫我們** - 完整聯絡資訊
8. **浮動 WhatsApp** - 隨時聯繫

## 🛠️ 技術棧

- **框架：** React 18 + TypeScript
- **構建工具：** Vite
- **樣式：** Tailwind CSS
- **UI 組件：** shadcn/ui
- **圖標：** Lucide React
- **動畫：** Tailwind Animate

## 🚀 快速開始

### 環境要求

- Node.js 18.0 或更高版本
- npm 或 pnpm

### 安裝

```bash
# 克隆項目
git clone <your-repo-url>

# 進入項目目錄
cd company_website

# 安裝依賴
npm install
# 或使用 pnpm
pnpm install
```

### 開發

```bash
# 啟動開發服務器
npm run dev

# 在瀏覽器打開
# http://localhost:5173
```

### 構建

```bash
# 構建生產版本
npm run build

# 預覽構建結果
npm run preview
```

## 📦 部署

### Vercel（推薦）

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new)

1. 點擊上方按鈕
2. 連接您的 Git repository
3. 自動部署完成

**或使用 CLI：**

```bash
npm install -g vercel
vercel
```

### Netlify

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start)

**構建設置：**
- Build command: `npm run build`
- Publish directory: `dist`

### 其他平台

構建後的文件在 `dist` 目錄，可部署到任何靜態網站託管服務。

## 🎨 自定義

### 修改品牌顏色

編輯 `src/index.css`：

```css
:root {
  --primary: 270 70% 50%;      /* 主紫色 */
  --accent: 280 70% 55%;       /* 強調色 */
}
```

### 修改聯繫方式

在以下組件中更新：
- `src/components/Hero.tsx`
- `src/components/Contact.tsx`
- `src/components/FloatingWhatsApp.tsx`
- `src/components/Footer.tsx`

### 添加新頁面

1. 在 `src/pages/` 創建新組件
2. 在 `src/App.tsx` 添加路由
3. 更新導航菜單

## 📁 項目結構

```
company_website/
├── public/                 # 靜態資源
│   ├── favicon.ico
│   └── images/
├── src/
│   ├── components/         # React 組件
│   │   ├── ui/            # 基礎 UI 組件
│   │   ├── Hero.tsx
│   │   ├── Services.tsx
│   │   ├── ServiceProcess.tsx
│   │   ├── WhyChooseUs.tsx
│   │   ├── CaseStudies.tsx
│   │   ├── FAQ.tsx
│   │   ├── Contact.tsx
│   │   ├── Footer.tsx
│   │   └── FloatingWhatsApp.tsx
│   ├── pages/             # 頁面組件
│   │   └── Index.tsx
│   ├── lib/               # 工具函數
│   ├── hooks/             # 自定義 Hooks
│   ├── index.css          # 全局樣式
│   └── main.tsx           # 應用入口
├── index.html
├── package.json
├── vite.config.ts
├── tailwind.config.ts
├── tsconfig.json
└── README.md
```

## 🔧 可用腳本

```bash
npm run dev          # 啟動開發服務器
npm run build        # 構建生產版本
npm run preview      # 預覽構建結果
npm run lint         # 代碼檢查
```

## 📞 聯繫方式

**Kore Communication HK Limited**  
克珞傳播（香港）有限公司

- 📱 WhatsApp: +852 5282 5778
- 📧 Email: cs@korecommunity.com
- 📍 地址: 香港九龍觀塘區興業街4號Thewave 7樓

## 📄 授權

© 2024 Kore Communication HK Limited. All Rights Reserved.

---

**需要技術支援？** 請通過 WhatsApp 或 Email 聯繫我們！
