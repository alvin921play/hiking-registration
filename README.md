[README.md](https://github.com/user-attachments/files/31447069/README.md)


# 登山報名系統 v16｜Supabase 線上測試版

這不是最終版，而是第一個跨裝置連線測試。

## 目前測試
1. 建立活動
2. Supabase 寫入 activities
3. 產生活動代碼 / 分享網址
4. 另一台裝置打開活動
5. 送出報名
6. Supabase 寫入 participants

## 上傳 GitHub 前
打開 `config.js`，只填：
- SUPABASE_URL = Supabase Project URL
- SUPABASE_PUBLISHABLE_KEY = Publishable key

不要填 Secret key / service_role。

## Vercel
這是純靜態網站，不需要 Build Command。
把整個資料夾內容上傳到 GitHub repository 根目錄，再由 Vercel Import。

## 注意
目前還沒接：
- 活動管理頁
- 阿翰總管理入口
- 費用建立/管理
- CSV
- 個人修改/找回 UI
- 60 天排程清除

資料庫端前四段功能已先建立；這版只驗證核心跨裝置連線。
