# 《足跡。歷程》｜周佳慮｜Richard

> 個人歷程、東方文明哲思、專案經歷與 AI 多媒體作品展示單頁網站。

🌐 **線上即時預覽（GitHub Pages）**：  
👉 [https://richardchou7703-cloud.github.io/zuji-licheng/](https://richardchou7703-cloud.github.io/zuji-licheng/)

---

## 📖 目錄與章節導覽

本站採連續畫卷式展演，共分為 8 大核心章節：
1. **封面**：《足跡。歷程》（含 Gmail / Email 快速聯絡連結）
2. **01 墨起**：筆墨序章
3. **02 禮樂**：東方文明（含 YouTube「R.甘露頻率」與 Facebook「禪境AI」社群互動熱區）
4. **03 驛站**：職涯足跡
5. **04 流水**：計畫專案
6. **05 文蘊**：專業積累
7. **06 今章**：AI多媒體（含 YouTube / Facebook 互動連結）
8. **封底**：結尾

---

## 🛠️ 技術亮點與 RWD 優化

- **雙模導覽列**：
  - **桌機版**：左側極簡垂直時間軸導覽，結合漸層細線與節點光暈。
  - **行動版（RWD）**：自動切換為頂部毛玻璃（Frosted Glass）圓角膠囊橫向滑動列，滾動時當前章節自動平滑置中對齊，不遮擋主要內容。
- **效能與體驗優化**：
  - 首屏封面圖設定 `loading="eager"` 與 `fetchpriority="high"`，極速加載。
  - 後續各場景切片圖設定 `loading="lazy"` 與非同步解碼 `decoding="async"`。
  - 明確設定 `aspect-ratio: 941 / 1672` 與尺寸，杜絕頁面載入時的版面跳動（CLS: 0）。
  - 右下角支援平滑「返回頁首」浮動按鈕（Back to Top）。
- **互動熱區**：
  - 精確百分比座標對齊，支援行動端觸控高亮反饋與安全點擊熱區。

---

## 📁 專案結構

```text
zuji-licheng/
├── images/             # 8 大章節高解析切片圖 (01.png ~ 08.png)
├── index.html          # 主頁面原始碼（含全響應式 CSS 與互動 JS）
├── README.md           # 專案說明文件
└── .gitignore          # 忽略檔設定
```

---

## 🚀 本地開發與預覽

直接在瀏覽器中開啟 `index.html` 即可預覽；或使用本機 HTTP 伺服器：

```bash
# Python 內建伺服器
python -m http.server 8080
# 開啟 http://localhost:8080 預覽
```
