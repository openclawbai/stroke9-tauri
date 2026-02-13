# 九方輸入法 Stroke9 IME

> 跨平台開源中文筆劃輸入法 - 支持 Mac, Windows, Linux, Android, iOS

![License](https://img.shields.io/badge/License-MIT-blue)
![Platform](https://img.shields.io/badge/Platform-Mac%20%7C%20Windows%20%7C%20Linux%20%7C%20Android%20%7C%20iOS-green)

## ✨ 特色

- 🎯 **筆劃輸入** - 基於中文筆劃（橫豎撇點折）
- ⚡ **連碼表** - 常用字 2 鍵快速輸入
- 📱 **跨平台** - 單一代碼庫，發布到所有平台
- 🎨 **現代 UI** - 美觀易用的界面
- 🔓 **開源免費** - MIT License

## 🚀 快速開始

### 開發模式
```bash
cd stroke9-tauri
npm install
npm run tauri dev
```

### 打包發布

**Mac:**
```bash
npm run tauri build -- --target universal-apple-darwin
```

**Windows:**
```bash
npm run tauri build -- --target x86_64-pc-windows-msvc
```

**Linux:**
```bash
npm run tauri build
```

**Android:**
```bash
npm run tauri android init
npm run tauri android dev
npm run tauri android build
```

**iOS:**
```bash
npm run tauri ios init
npm run tauri ios dev
```

## 📦 下載

發布版本將在 GitHub Releases 提供：
- `.dmg` - macOS
- `.exe` / `.msi` - Windows
- `.deb` / `.AppImage` - Linux
- `.apk` - Android
- `.ipa` - iOS (需要 Apple Developer 帳號)

## 🎮 使用方法

### 基本輸入
1. 按數字鍵 1-9 輸入筆劃
2. 查看候選字
3. 點擊或按數字鍵選字

### 連碼快速輸入
常用字只需 2 鍵：
- `34` → 的、人、我
- `11` → 二、三、王
- `24` → 是、國
- `31` → 人、入、久

### 鍵盤快捷鍵
- `1-9`: 輸入筆劃
- `Backspace`: 刪除
- `Esc`: 清除編碼
- `Space`: 空格
- `0-9`: 選擇候選字

## 🛠️ 技術棧

- **前端**: HTML/CSS/JavaScript (原生)
- **後端**: Rust (Tauri)
- **跨平台**: Tauri v2
- **構建**: npm + cargo

## 📱 平台支持

| 平台 | 狀態 | 備註 |
|------|------|------|
| macOS | ✅ 支持 | Universal binary (Intel + Apple Silicon) |
| Windows | ✅ 支持 | x64 |
| Linux | ✅ 支持 | Debian/Ubuntu/AppImage |
| Android | ✅ 支持 | APK (API 24+) |
| iOS | ⏳ 開發中 | 需要 Mac + Xcode |

## 🔧 開發

### 環境要求
- Node.js 18+
- Rust 1.90+
- Platform-specific tools (見 Tauri 文檔)

### 項目結構
```
stroke9-tauri/
├── index.html          # 前端 UI
├── src-tauri/          # Rust 後端
│   ├── src/
│   │   └── main.rs
│   ├── Cargo.toml
│   └── tauri.conf.json
├── package.json
└── README.md
```

### 添加新字典
編輯 `index.html` 中的 `strokeDict` 對象，或：
1. 創建 `dict.json`
2. 在代碼中加載
3. 動態更新候選字

## 🎯 路線圖

### v1.0 (當前)
- [x] 基礎筆劃輸入
- [x] 連碼表支持
- [x] 桌面版 (Mac/Windows/Linux)
- [ ] Android APK
- [ ] iOS IPA

### v2.0 (未來)
- [ ] 完整 20,000+ 字庫
- [ ] 智能詞組預測
- [ ] 雲同步設置
- [ ] 深色模式
- [ ] 自定義主題

### v3.0 (願景)
- [ ] AI 輔助候選
- [ ] 手寫識別
- [ ] 語音輸入
- [ ] 多語言支持

## 📄 授權

MIT License - 自由使用、修改、分發

## 🤝 貢獻

歡迎 PR！
- 添加字庫
- 優化連碼
- 改進 UI
- Bug 修復

## 📞 聯繫

- GitHub: [openclawbai/stroke9-tauri](https://github.com/openclawbai/stroke9-tauri)
- Issues: 提交問題和建議

---

*Created by Buffett 🦅*  
*2026-02-13*
