# 黃豆副產物循環利用網站（GitHub Pages）

這是由原始 `黃豆殼(1).html` 整理出的靜態網站版本，首頁已改名為 `index.html`，保留原有繁中/英文切換、深色模式、試算工具、照片藝廊與瀏覽器本機儲存功能，並修正藝廊刪除按鈕的 HTML 標記。

## 發布到 GitHub Pages

1. 登入 https://github.com/ 。
2. 點右上角 `+` → `New repository`。
3. Repository name 可填 `soybean-circular-economy`，選 `Public`，建立 Repository。
4. 在 Repository 頁面點 `Add file` → `Upload files`。
5. 上傳本資料夾內的 `index.html` 與 `images` 資料夾（不要只上傳 ZIP）。
6. 點 `Commit changes`。
7. 開啟 Repository 的 `Settings` → `Pages`。
8. 在 `Build and deployment` 設定 `Deploy from a branch`，Branch 選 `main`，資料夾選 `/(root)`，按 `Save`。
9. 等待發布完成，網址通常會是 `https://你的GitHub帳號.github.io/soybean-circular-economy/`。

## 真實照片注意事項

原始 HTML 內的 12 張藝廊卡片是由程式產生的 SVG 示意圖，不是真實拍攝照片。你目前尚未提供真實照片，因此此版本先保留示意圖，避免出現破圖。請把真實照片上傳到對話中，我可以再幫你把它們接入網站。建議準備黃豆殼與豆渣各 6 張；照片可以是 JPG、PNG 或 WebP。

## 重要限制

- Tailwind、Alpine.js、Font Awesome 與 Google Fonts 使用外部 CDN，因此首次載入及相關功能需要網路連線。
- 藝廊使用 `localStorage` 儲存使用者在該瀏覽器新增/刪除的照片資料；這不會把照片同步到 GitHub，也不會自動同步到其他裝置。
- 這是靜態網站，不包含後端資料庫或多人同步功能。
