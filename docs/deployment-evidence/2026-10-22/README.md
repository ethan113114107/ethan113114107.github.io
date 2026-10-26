# 慈濟大學經營管理學系網站｜GitHub Pages 上線驗證紀錄

> 本紀錄保存 2026 年 10 月 22 日的單次公開存取驗證證據，於 2026 年 10 月 26 日封存。它不是持續監控紀錄，也不保證網站目前或未來一直可用。

## 一、網站、版本與來源

| 項目 | 紀錄 |
| --- | --- |
| 正式網站網址 | https://ethan113114107.github.io/ |
| 正式 GitHub 儲存庫 | https://github.com/ethan113114107/ethan113114107.github.io |
| 驗證時的網站版本標記 | `tcu-public-photo-20261022` |
| 對應提交版本 | `473df5fee1ba9e75ae39379261fe1e6117db8889`（簡寫 `473df5f`） |
| 工作流程 | `Verify public department website` |
| GitHub Actions 執行編號 | `39721625719`，第 1 次執行 |
| 工作流程狀態／結果 | `completed`／`success` |
| 分支／觸發事件 | `main`／`push` |
| 報告時間（UTC，原始值） | `2026-10-22T04:18:43.991231+00:00` |
| 報告時間（臺灣，UTC+08:00） | **2026 年 10 月 22 日 12:18:43.991231** |
| 公開請求方式 | 未登入、未帶 GitHub 驗證憑證（原始欄位 `unauthenticated: true`） |
| 結果摘要 | **12 個公開資源，12 筆 HTTP 200，沒有記錄到非 200 結果。** |
| 本次封存日期 | 2026 年 10 月 26 日（臺灣） |

來源：[GitHub Actions 執行紀錄](https://github.com/ethan113114107/ethan113114107.github.io/actions/runs/39721625719)、[驗證時的提交版本](https://github.com/ethan113114107/ethan113114107.github.io/commit/473df5fee1ba9e75ae39379261fe1e6117db8889)、[固定版本的驗證程式](https://github.com/ethan113114107/ethan113114107.github.io/blob/473df5fee1ba9e75ae39379261fe1e6117db8889/.github/workflows/verify-public-site.yml)。

`checked_at` 是程式在所有請求完成後產生報告時記錄的時間，不是每個請求各自的精確時間。原始 JSON 本身沒有提交 SHA 欄位；上述提交關聯來自 GitHub Actions 執行資料與 Artifact 的 `head_sha`，沒有將它補寫進原始 JSON。

## 二、逐項檢查結果

下表完整轉錄原始 JSON 的 12 筆結果。位元組數為當次讀取到的回應本文長度，不是頁面瀏覽人數或傳輸速率。連結指向現行網站；歷史證據以本目錄的原始 JSON 為準。

| 編號 | 公開資源 | HTTP | Content-Type | 本文位元組數 |
| --- | --- | ---: | --- | ---: |
| 1 | [首頁 `/`](https://ethan113114107.github.io/) | 200 | `text/html; charset=utf-8` | 23,401 |
| 2 | [首頁 `index.html`](https://ethan113114107.github.io/index.html) | 200 | `text/html; charset=utf-8` | 23,401 |
| 3 | [學生作品 `studentworks.html`](https://ethan113114107.github.io/studentworks.html) | 200 | `text/html; charset=utf-8` | 25,725 |
| 4 | [AI 協作紀錄 `ai-collaboration.html`](https://ethan113114107.github.io/ai-collaboration.html) | 200 | `text/html; charset=utf-8` | 32,143 |
| 5 | [照片來源 `photo-credits.html`](https://ethan113114107.github.io/photo-credits.html) | 200 | `text/html; charset=utf-8` | 19,324 |
| 6 | [完整 Prompt `AI-COLLABORATION-FULL.txt`](https://ethan113114107.github.io/AI-COLLABORATION-FULL.txt) | 200 | `text/plain; charset=utf-8` | 15,571 |
| 7 | [校園照片 `graph/tcu-campus.jpg`](https://ethan113114107.github.io/graph/tcu-campus.jpg) | 200 | `image/jpeg` | 618,551 |
| 8 | [圖書館照片 `graph/tcu-library.jpg`](https://ethan113114107.github.io/graph/tcu-library.jpg) | 200 | `image/jpeg` | 378,834 |
| 9 | [數位學習照片 `graph/digital-learning.jpg`](https://ethan113114107.github.io/graph/digital-learning.jpg) | 200 | `image/jpeg` | 255,109 |
| 10 | [自然主題照片 `graph/circular-nature.jpg`](https://ethan113114107.github.io/graph/circular-nature.jpg) | 200 | `image/jpeg` | 522,512 |
| 11 | [分類意象圖 `graph/work-sort.svg`](https://ethan113114107.github.io/graph/work-sort.svg) | 200 | `image/svg+xml` | 503 |
| 12 | [影片 `graph/learning-intro.mp4`](https://ethan113114107.github.io/graph/learning-intro.mp4) | 200 | `video/mp4` | 277,163 |

共 5 筆 HTML 回應、1 筆文字檔、5 筆圖片與 1 筆影片。`/` 與 `index.html` 是首頁的兩個存取路徑，不應當成兩個不同的內容頁。

## 三、此次驗證能證明什麼

依原始報告及固定提交版本的工作流程，當次檢查使用不帶登入憑證的 HTTP 請求讀取這 12 個網址，要求全部回應為 200；另外檢查首頁與 HTML 內含指定版本標記、JPEG 檔頭，以及 MP4 前 32 位元組內的 `ftyp` 標記。工作流程成功完成並輸出本報告。

這證明指定檢查執行期間，所列資源可由該 GitHub Actions 執行環境公開讀取，並通過上述檢查。它不等同於全球所有網路、所有瀏覽器皆可使用，也不等同於完整的視覺、互動、無障礙、安全性或影片播放驗收。原始 JSON 沒有逐筆記錄版本與檔頭判定欄位，相關檢查方式由工作流程原始碼與執行成功結果佐證。

本次工作只下載、核對與封存歷史證據，沒有重跑網站公開驗證，也沒有建立排程或持續監控。

## 四、Artifact 來源與保存期限

| 項目 | 原始來源資料 |
| --- | --- |
| Artifact 名稱 | `tcu-public-verification` |
| Artifact 編號 | `12401327383` |
| 壓縮檔大小 | 626 位元組 |
| 建立時間（UTC） | `2026-10-22T04:18:44Z` |
| 建立時間（臺灣） | 2026 年 10 月 22 日 12:18:44 |
| 工作流程設定的保留時間 | 7 天 |
| 原 Artifact 到期時間（UTC） | `2026-10-29T04:18:44Z` |
| 原 Artifact 到期時間（臺灣） | **2026 年 10 月 29 日 12:18:44** |
| 下載時的狀態 | `expired: false` |

[Artifact 中繼資料來源](https://api.github.com/repos/ethan113114107/ethan113114107.github.io/actions/runs/39721625719/artifacts)；[原 Artifact 下載 API](https://api.github.com/repos/ethan113114107/ethan113114107.github.io/actions/artifacts/12401327383/zip)（可能需要 GitHub 權限，且受原 Artifact 到期限制）。

本目錄將原始 ZIP 與 JSON 保存為正式儲存庫內的版本控制檔案，不再依賴該 Artifact 的七天保留期。原 Artifact 的到期時間沒有被延長。只要儲存庫與相關 Git 歷史仍保留，即可從此目錄查閱；這不是不可刪除或永不失效的第三方存證服務。

## 五、原始資料與完整性核對

| 檔案 | 用途 |
| --- | --- |
| [PUBLIC-VERIFICATION.json](PUBLIC-VERIFICATION.json) | 從原 ZIP 解出的原始驗證資料，逐位元組保存；未改寫時間、版本、網址、狀態、排序或格式。 |
| [tcu-public-verification.original.zip](tcu-public-verification.original.zip) | 從指定 Artifact 下載的原始 ZIP，未重新壓縮。 |
| [PROVENANCE.json](PROVENANCE.json) | 封存時整理的來源中繼資料、完整提交 SHA、檢查範圍與核對結果；不是原始 API 回應全文。 |
| [SHA256SUMS](SHA256SUMS) | 原始 JSON 與 ZIP 的 SHA-256 校驗值。 |
| [README.md](README.md) | 本繁體中文紀錄；屬後製說明，不冒充原始測試輸出。 |

原始 ZIP 的 SHA-256（與 GitHub Artifact `digest` 完全一致）：

```text
0c6ae74b842997542d5baff0da3eae7ca9ab91ac771eadeffc0d2da94391dbd4
```

原始 JSON 的 SHA-256：

```text
59902aa10f70bf3e086b6c5f32e584777ffbd0dc25b0b0b401858c2bf0d9b54e
```

核對過程：確認 ZIP 大小為 626 位元組、CRC 檢查通過、壓縮檔只包含 `PUBLIC-VERIFICATION.json`、JSON 大小為 2,150 位元組且可正常解析、結果筆數為 12 且全部狀態為 200。SHA-256 用於核對檔案一致性，不代表具有第三方數位簽章。

下載本目錄後，可在終端機執行 `sha256sum -c SHA256SUMS`；Windows PowerShell 可分別執行 `Get-FileHash .\PUBLIC-VERIFICATION.json -Algorithm SHA256` 與 `Get-FileHash .\tcu-public-verification.original.zip -Algorithm SHA256`，比對上述數值。

## 六、變更範圍與長期查閱方式

此次封存僅在 `docs/deployment-evidence/2026-10-22/` 新增上述 5 個證據檔案。不修改 `index.html`、`studentworks.html`、AI 協作頁、照片來源頁、`graph/`、網站設計、既有功能、既有 README 或工作流程設定。

查閱入口：[正式儲存庫中的封存目錄](https://github.com/ethan113114107/ethan113114107.github.io/tree/main/docs/deployment-evidence/2026-10-22)。如需引用本次封存的固定內容，可使用保存提交的完整 SHA 建立 GitHub `blob/<commit>/...` 連結，避免未來 `main` 更新影響引用。

依既有 Pages 設定，新增文件可能觸發正常的重新部署；這不代表重跑了 2026 年 10 月 22 日的驗證，也不會改變上述歷史結果。將來若另做驗證，應建立新的日期目錄，不覆寫本次原始證據。
