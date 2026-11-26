# MagicSpark Studio App 教學網站

網址：<https://kuanyiyang-maker.github.io/>（GitHub Pages，Jekyll 自動產生，不需要自己建置）

## 資料夾

| 路徑 | 內容 |
|---|---|
| `index.md` | 首頁：所有 App 與最新文章 |
| `formuscript/index.md` | 算記教學列表 |
| `formuscript/_posts/` | 算記教學文章 |
| `assets/img/<app>/` | 文章圖片 |
| `_config.yml` | 網站設定；`apps:` 放各 App 的名稱、Play 連結、隱私權網址 |
| `_layouts/` | 版面（一般頁、文章頁） |
| `assets/css/style.css` | 樣式（含深色模式） |

## 新增一篇文章

1. 在 `formuscript/_posts/` 新增 `YYYY-MM-DD-英文短名.md`，例如 `2026-12-01-quick-tools.md`。
   網址會是 `/formuscript/quick-tools/`。
2. 檔案開頭寫：

   ```yaml
   ---
   title: 文章標題
   description: 一句話說明（顯示在列表與搜尋結果）
   minutes: 5
   ---
   ```

3. 圖片放 `assets/img/formuscript/`，文章裡寫 `![說明文字](/assets/img/formuscript/檔名.png)`。
4. commit、push 後約 1 分鐘，網站會自動更新。

## 新增另一個 App

1. 在 `_config.yml` 的 `apps:` 加一筆（key 用英文，例如 `calculator`）。
2. 建立 `calculator/index.md`（可複製 `formuscript/index.md`，把 `formuscript` 換掉）和 `calculator/_posts/`。
3. 在 `index.md` 的卡片區加一張卡片，`_layouts/default.html` 的導覽列加連結。

## 注意

- 不要建立 `formuscript-privacy` 資料夾：那個網址是另一個 repo（算記隱私權政策，Play Console 有登記）。
- 文案不寫「無廣告」「免登入」「完全離線」「免費」，也不寫價格。
