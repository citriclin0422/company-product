# 立赫精密 (AXEQUATOR PRECISION LTD) 官網建置與部署工作日誌

- **專案名稱**：立赫精密公司形象官網建置 (PJ1_company-product)
- **GitHub 儲存庫**：[`citriclin0422/company-product`](https://github.com/citriclin0422/company-product)
- **GitHub Pages 公開網址**：[https://citriclin0422.github.io/company-product/](https://citriclin0422.github.io/company-product/)
- **建置日期**：2026-09-02
- **狀態**：✅ 已完成本機建置、瀏覽器驗證、README 建立與 GitHub main 分支推送

---

## 📑 1. 需求與資料來源研讀

依據 `.preparation/` 目錄中之規格書、設定檔與中英文名片圖檔，核對提取出以下真實企業資訊：

| 項目 | 內容 | 來源依據 |
| :--- | :--- | :--- |
| **公司中文名稱** | 立赫精密有限公司 | 名片 / 統編登錄 |
| **公司英文名稱** | AXEQUATOR PRECISION LTD | 英文名片 |
| **統一編號** | `60765834` | 中文名片 |
| **聯絡窗口** | 邱炘然 Lorenzo Chiu (特助 / Executive Assistant) | 中英文名片 |
| **行動電話** | `0919-912963` / `+886-919-912963` | 中英文名片 |
| **公司電話** | `04-25576888` / `+886-4-25576888` | 中英文名片 |
| **通訊軟體 ID** | Line / WeChat: `AEP0520` | 中英文名片 |
| **公司 Email** | `Service@axequator.com` | 中英文名片 |
| **公司地址** | 台中市后里區三豐路四段129巷48號2樓<br>(2F., No.48, Ln. 129, Sec. 4, Sanfeng Rd., Houli Dist., Taichung City 421012, Taiwan) | 中英文名片 |
| **三大核心服務** | 1. 半導體設備維修<br>2. 零組件檢查與更換<br>3. 鋼瓶更換作業支援 | 規格書與 YAML |
| **業務規範原則** | 嚴格遵守規範，不宣稱未經授權之原廠認證、ISO標章或揭露客戶機密 | 規格書約束 |

---

## 🎨 2. 視覺與前端架構設計

1. **設計哲學與色調 Token**：
   - **底色**：深海軍藍 `#0B1F33` 與微透光科技網格背景 (`#07121E`)
   - **主視覺強調色**：科技天藍 `#38BDF8`、深科技藍 `#1677B8`
   - **工安與重要提示色**：安全亮橙 `#F59E0B`
   - **排版字型**：`Noto Sans TC` (中文) + `Inter` (英文/數字)
   - **專屬 Logo**：比對名片之電路球體圖形，以高精度純向量 SVG 重繪內嵌。
2. **單頁 9 大結構區塊**：
   - `Header`：毛玻璃固定導覽列、平滑錨點捲動、Active 區塊追蹤、手機版抽屜選單。
   - `Hero`：首頁主視覺大標題、核心業務說明、雙 CTA 行動按鈕、三大特色 Badge。
   - `About`：團隊定位、5 大核心理念（專業、安全、精準、協作、穩定）、公司基本資訊表。
   - `Services`：3 大核心服務卡片（設備維修、零組件更換、鋼瓶更換）。
   - `Process`：5 步驟標準作業時序流程（需求確認 $\rightarrow$ 現場及風險確認 $\rightarrow$ 維修執行 $\rightarrow$ 復原 $\rightarrow$ 完工回報）。
   - `Safety`：4 大專業與安全原則（作業前確認、規範化執行、品質核對、紀錄與交接）。
   - `Scenarios`：4 大服務場景（半導體製造廠、封測廠、廠務與氣體系統、設備承攬商）。
   - `Contact`：完整實體名片數據卡片、一鍵點擊複製 Toast 提示、快速產生 `mailto:` 洽詢表單。
   - `Footer`：版權資訊、快速導覽與通訊連結。

---

## ⚙️ 3. 執行與部署歷程 (Task Log)

1. **拉取專案**：
   - 初始化並拉取遠端 `https://github.com/citriclin0422/company-product.git` 至本機目錄。
2. **重構 `index.html`**：
   - 全面改寫為完整響應式形象單頁官網，整合名片資訊、SVG 圖示與 JavaScript 互動功能。
3. **本機預覽與瀏覽器驗證**：
   - 啟動測試伺服器進行瀏覽器多解析度（桌機、平板、360px 手機）完整渲染與互動測試。
   - 驗證結果：控制台 0 錯誤，導覽錨點、一鍵複製 Toast、選單開合與 mailto 產出均正常。
4. **撰寫 `README.md`**：
   - 建立專案說明文件，放置中文名片 (`companycard_chinese.jpg`) 與英文名片 (`companycard_english.jpg`) 預覽圖。
   - 附上 GitHub Pages 網站正式連結 [立赫精密｜AXEQUATOR PRECISION LTD](https://citriclin0422.github.io/company-product/)。
5. **Git 提交與推送 (Push to Remote)**：
   - 提交 `index.html`、`README.md`、`.preparation/` 相關資源。
   - 執行 `git push origin main` 成功推送到 GitHub 遠端儲存庫。

---

## 📦 4. 交付檔案清單

- [`index.html`](file:///c:/AI_class/PJ1_company-product/index.html)：官網前端主要單頁程式碼。
- [`README.md`](file:///c:/AI_class/PJ1_company-product/README.md)：GitHub 專案說明文件（含名片圖與公開網站連結）。
- [`.preparation/`](file:///c:/AI_class/PJ1_company-product/.preparation/)：規格書、YAML 設定檔與中英文名片原始圖檔。
- [`.md_doc/log.md`](file:///c:/AI_class/PJ1_company-product/.md_doc/log.md)：本工作日誌記錄檔。
