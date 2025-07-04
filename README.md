# 🏃‍♀️ iRun (團隊專案)
[![iRun](https://firebasestorage.googleapis.com/v0/b/mobaocoffee.appspot.com/o/cover.png?alt=media&token=dd3a3212-687e-439f-b52b-cae057c444b7)](https://clovetseng.github.io/iRun/)*點擊圖片可連結至 Demo 頁*

專案期間：2024/09 ~ 2024/10

## 專案簡介：
此專案是與 UI / UX 設計團隊協作，純手刻切版。
目的為打造一款由 AI 教練陪伴的健身 App Prototype，主打「陪
伴感」與「入門友善」。

## 專案使用技術與工具：
 `HTML`、`SCSS`、`JavaScript`、`Bootstrap`  
`Git`、`GitHub`、`Figma`、`Notion`

## 主要負責頁面
- 登入主頁及登入註冊頁面切版

  <img src="https://firebasestorage.googleapis.com/v0/b/mobaocoffee.appspot.com/o/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202025-04-25%20163107.png?alt=media&token=9e4bed70-17bd-43fe-b5f3-e6b6866a9305" width="200px">
- 填寫個人身體數據及運動頻率頁面切版
- 搭配設計團隊提供之 Design System ，建立變數表方便後續開發進行


## 技術挑戰與解決方案
### 🚧 挑戰 1：從桌機思維出發，導致切版畫面高度未滿版
> 因設計稿為純手機版畫面，許多頁面以一頁顯示為主。但起初仍以桌機網站開發慣性出發，導致頁面容易出現未填滿整頁、高度不足、跑版或出現滾動條的問題。

**任務：**
調整切版邏輯與 CSS 寫法，確保各頁面在手機裝置上能貼齊整頁高度，並避免多餘的滾動或空白區塊。

**解決問題：**
- 設定 `min-height: 100vh` 確保畫面能撐滿一整頁
- 留意 `box-sizing`、`padding`、`margin` 的影響，避免內容撐破畫面或導致捲軸
- 使用 flex 排版讓內容平均分配
- 搭配 DevTools 模擬多款手機螢幕尺寸，逐一測試與調整

最終成功讓畫面在各尺寸裝置上呈現穩定，且符合設計稿預期的「一頁呈現」效果

### 🚧 挑戰 2：設計稿雖然一開始有 Design System，但實際稿件仍出現間距、字體大小不一致的問題
> 設計團隊雖有建立 Design System，但實際畫面設計中有部分元件（如標題、按鈕、間距）未完全遵守規範，導致切版時無法直接套用變數，需自行判斷處理。

**任務：**
在尊重設計風格的前提下，協助整理統一樣式，並優化 CSS 變數管理，使團隊後續開發更一致且易於維護。

**解決問題：**
- 與設計師進行同步會議，確認哪些屬於例外狀況，哪些可以回歸 Design System 規範
- 將實際常見的間距、字體大小等整理為 SCSS 變數，並更新變數表文件
- 針對共用元件如按鈕、表單欄位建立共用 class，提升重用性與一致性
- 共編統一使用的變數與元件，減少樣式混亂的狀況
  <img src="https://firebasestorage.googleapis.com/v0/b/mobaocoffee.appspot.com/o/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202025-04-25%20165305.png?alt=media&token=eb3f6851-d0f6-4845-bc33-c8ef94d10041" width="300px">

## 團隊協作方式
- 使用 **Notion** 管理專案：變數表、會議記錄、分工進度
- 使用 **Figma** 與設計師同步畫面與版面調整
- Git 協作開發，透過 Pull Request 機制共同維護程式碼品質

## 學習與收穫
- 實際演練與設計師協作切版流程，強化協同能力
- 學會以 Design System 為基礎進行變數與元件規劃
- 培養以使用者為中心的 UI/UX 思維與細節調整能力

## 專案連結
- [GitHub](https://github.com/CloveTseng/iRun)
- [Demo](https://clovetseng.github.io/iRun/)
