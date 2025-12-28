# Kore Communication 網站部署指南

## 📦 項目說明

這是 Kore Communication HK Limited（克珞傳播香港有限公司）的官方網站源代碼。

**網站特色：**
- O2O 教師 B2B SaaS 平台展示
- 紫白配色專業設計
- 響應式設計，支持各種設備
- WhatsApp 即時聯繫功能
- 完整的服務介紹和 FAQ

**聯繫方式：**
- WhatsApp: +852 5282 5778
- Email: cs@korecommunity.com
- 地址: 香港九龍觀塘區興業街4號Thewave 7樓

---

## 🚀 部署到 Vercel（推薦）

### 方法一：通過 GitHub（最簡單）

1. **上傳到 GitHub**
   - 在 GitHub 創建新 repository
   - 將此項目所有文件上傳到 repository

2. **連接 Vercel**
   - 訪問 [vercel.com](https://vercel.com)
   - 使用 GitHub 帳號登入
   - 點擊 "Add New Project"
   - 選擇您的 repository
   - 框架選擇：**Vite**
   - 點擊 "Deploy"

3. **完成！**
   - 等待 2-3 分鐘
   - 獲得免費的 .vercel.app 域名
   - 可綁定自定義域名

### 方法二：使用 Vercel CLI

```bash
# 1. 安裝 Vercel CLI
npm install -g vercel

# 2. 在項目文件夾中執行
cd company_website
vercel login

# 3. 部署
vercel

# 4. 生產環境部署
vercel --prod
```

---

## 💻 本地運行

### 環境要求
- Node.js 18+ 
- npm 或 pnpm

### 安裝步驟

```bash
# 1. 安裝依賴
npm install
# 或
pnpm install

# 2. 啟動開發服務器
npm run dev
# 或
pnpm dev

# 3. 在瀏覽器打開
# http://localhost:5173
```

### 構建生產版本

```bash
# 構建
npm run build

# 預覽構建結果
npm run preview
```

---

## 🌐 部署到其他平台

### Netlify

1. 訪問 [netlify.com](https://netlify.com)
2. 拖放 `dist` 文件夾（需先執行 `npm run build`）
3. 或連接 GitHub repository 自動部署

**構建設置：**
- Build command: `npm run build`
- Publish directory: `dist`

### GitHub Pages

```bash
# 1. 安裝 gh-pages
npm install -D gh-pages

# 2. 在 package.json 添加
"scripts": {
  "deploy": "npm run build && gh-pages -d dist"
}

# 3. 部署
npm run deploy
```

---

## 🔧 自定義配置

### 修改聯繫方式

在以下文件中搜索並替換：

**WhatsApp 號碼：** `85252825778`
- `src/components/Hero.tsx`
- `src/components/Contact.tsx`
- `src/components/FloatingWhatsApp.tsx`
- `src/components/Footer.tsx`

**Email：** `cs@korecommunity.com`
- `src/components/Contact.tsx`
- `src/components/Footer.tsx`

**地址：** `香港九龍觀塘區興業街4號Thewave 7樓`
- `src/components/Contact.tsx`
- `src/components/Footer.tsx`

### 修改品牌顏色

編輯 `src/index.css` 中的 CSS 變量：

```css
:root {
  --primary: 270 70% 50%;        /* 主色調（紫色）*/
  --primary-glow: 270 80% 65%;   /* 發光效果 */
  --accent: 280 70% 55%;         /* 強調色 */
}
```

---

## 📁 項目結構

```
company_website/
├── src/
│   ├── components/          # React 組件
│   │   ├── ui/             # UI 基礎組件
│   │   ├── Hero.tsx        # 首頁英雄區
│   │   ├── Services.tsx    # 服務介紹
│   │   ├── ServiceProcess.tsx  # 服務流程
│   │   ├── WhyChooseUs.tsx     # 選擇我們的理由
│   │   ├── CaseStudies.tsx     # 成功案例
│   │   ├── FAQ.tsx             # 常見問題
│   │   ├── Contact.tsx         # 聯繫方式
│   │   ├── Footer.tsx          # 頁腳
│   │   └── FloatingWhatsApp.tsx # 浮動 WhatsApp 按鈕
│   ├── pages/              # 頁面
│   │   └── Index.tsx       # 首頁
│   ├── index.css           # 全局樣式
│   └── main.tsx            # 入口文件
├── public/                 # 靜態資源
├── package.json            # 依賴配置
├── vite.config.ts          # Vite 配置
├── tailwind.config.ts      # Tailwind 配置
└── tsconfig.json           # TypeScript 配置
```

---

## 🔒 環境變量（如需要）

創建 `.env` 文件：

```env
# 如果需要添加環境變量
VITE_API_URL=your_api_url
```

---

## 📞 技術支援

如有任何問題，請聯繫：
- WhatsApp: +852 5282 5778
- Email: cs@korecommunity.com

---

## 📄 授權

© 2024 Kore Communication HK Limited. All Rights Reserved.
