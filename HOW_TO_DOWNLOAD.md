# 📥 如何下載和使用源代碼

## 方法一：從 Skywork 下載（推薦）

由於您目前在 Skywork 平台上，源代碼已經準備好了。

### 下載步驟：

1. **查看項目文件**
   - 項目位置：`/workspace/company_website`
   - 包含所有源代碼和配置文件

2. **需要下載的文件和文件夾：**

```
必需文件：
✅ src/                    (整個文件夾)
✅ public/                 (整個文件夾)
✅ package.json
✅ package-lock.json
✅ vite.config.ts
✅ tailwind.config.ts
✅ tsconfig.json
✅ tsconfig.app.json
✅ tsconfig.node.json
✅ index.html
✅ postcss.config.js
✅ components.json
✅ README.md
✅ DEPLOYMENT_GUIDE.md
✅ .gitignore

不需要下載：
❌ node_modules/         (太大，本地重新安裝)
❌ dist/                 (構建產物，本地重新生成)
❌ .git/                 (Git 歷史)
```

3. **下載後的操作：**

```bash
# 在您的電腦上
cd company_website

# 安裝依賴
npm install

# 啟動開發服務器
npm run dev

# 構建生產版本
npm run build
```

---

## 方法二：使用 Git（如果可用）

如果 Skywork 支持 Git 導出：

```bash
# 克隆項目
git clone <repository-url>

# 進入目錄
cd company_website

# 安裝依賴
npm install
```

---

## 方法三：手動複製文件

如果無法直接下載，您可以：

1. **逐個複製文件內容**
   - 在本地創建相同的文件夾結構
   - 複製每個文件的內容

2. **重要文件清單：**

### 配置文件
- `package.json` - 依賴配置
- `vite.config.ts` - Vite 配置
- `tailwind.config.ts` - Tailwind 配置
- `tsconfig.json` - TypeScript 配置
- `index.html` - HTML 入口

### 源代碼文件夾
- `src/components/` - 所有組件
- `src/pages/` - 頁面
- `src/lib/` - 工具函數
- `src/hooks/` - React Hooks
- `src/index.css` - 全局樣式
- `src/main.tsx` - 應用入口

### 靜態資源
- `public/` - 圖片和其他靜態文件

---

## 📦 完整文件列表

### 根目錄文件
```
company_website/
├── index.html
├── package.json
├── package-lock.json
├── vite.config.ts
├── tailwind.config.ts
├── tsconfig.json
├── tsconfig.app.json
├── tsconfig.node.json
├── postcss.config.js
├── components.json
├── eslint.config.js
├── README.md
├── DEPLOYMENT_GUIDE.md
├── HOW_TO_DOWNLOAD.md
└── .gitignore
```

### src/ 文件夾
```
src/
├── components/
│   ├── ui/                    (約 40+ 個 UI 組件)
│   ├── Hero.tsx
│   ├── Services.tsx
│   ├── ServiceProcess.tsx
│   ├── WhyChooseUs.tsx
│   ├── CaseStudies.tsx
│   ├── FAQ.tsx
│   ├── Contact.tsx
│   ├── Footer.tsx
│   └── FloatingWhatsApp.tsx
├── pages/
│   ├── Index.tsx
│   └── NotFound.tsx
├── lib/
│   ├── utils.ts
│   └── react-router-dom-proxy.tsx
├── hooks/
│   ├── use-mobile.tsx
│   └── use-toast.ts
├── index.css
├── App.css
├── App.tsx
├── main.tsx
└── vite-env.d.ts
```

### public/ 文件夾
```
public/
├── favicon.ico
├── placeholder.svg
└── robots.txt
```

---

## 🚀 下載後立即部署

### 部署到 Vercel

```bash
# 1. 安裝 Vercel CLI
npm install -g vercel

# 2. 登入
vercel login

# 3. 部署
vercel

# 4. 生產環境
vercel --prod
```

### 部署到 Netlify

```bash
# 1. 構建
npm run build

# 2. 拖放 dist 文件夾到 Netlify
# 訪問 https://app.netlify.com/drop
```

---

## ❓ 常見問題

### Q: 下載後無法運行？
A: 確保已安裝 Node.js 18+ 並執行 `npm install`

### Q: 缺少某些文件？
A: 檢查上面的文件列表，確保所有必需文件都已下載

### Q: 如何修改內容？
A: 編輯 `src/components/` 中的對應組件文件

### Q: 如何更換圖片？
A: 將圖片放入 `public/images/` 並更新組件中的路徑

---

## 📞 需要幫助？

如有任何問題，請聯繫：
- WhatsApp: +852 5282 5778
- Email: cs@korecommunity.com

---

**祝您部署順利！** 🎉
