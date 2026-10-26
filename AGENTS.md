# ai-native-founders-tw-mono

AI-Native Global Founders Speedrun Taiwan 的 specs、plans 與 logs。根層只有 `specs/`、`plans/` 與 `logs/`。

## 憲法

**[`specs/01-制度/constitution.md`](specs/01-制度/constitution.md) 是憲法。這個 repo 的所有產出都受憲法約束，不能違反憲法中的任何一條規則。**

AI 在產出完之後，尤其是 Deliver／Push 之前，必須以 subagent 以極度嚴格的角度去檢查是否有違反憲法中的每一條規則：

- 交給 subagent 的是憲法全文與這次產出的實際內容（diff 與改到的檔案全文），不是產出者的摘要。
- 逐條檢查憲法的每一條，每一條都要有結論：違反，或沒有違反；違反時指出哪個檔案的哪一段。拿不準的算違反。
- subagent 只檢查，不修改。
- 有任何一條違反，就不 Deliver、不 Push，照憲法第六章（憲法的效力與修改）與第七章（附則）處理：改產出，不改憲法；違反的是創辦人的話時，由創辦人自己改；建立或修改憲法的 Plan 裡，憲法本身就是產出。改完再以 subagent 檢查每一條。
- 檢查的結論寫進該 Plan 的「憲法檢查」。

## 制度與憲法的分工

憲法保留組織目的、基本原則與治理規則。申請方式、自介審查及成員參與的具體安排，分別寫在 `specs/01-制度/[機制]申請制度.md` 與 `specs/01-制度/[機制]成員參與制度.md`。

制度文件不得違反憲法；制度調整寫進各自 Plan 並接受憲法檢查，不必因此修憲。工作流引用制度，不另存第二套可編輯規則。只有涉及憲法本身的變更，才使用專門修憲 Plan。

## specs

`specs/` 放 specs truth：上游 why／should、Problem、Forces 與規格。specs 分 package，一個 package 一個目錄 `specs/<編號>-<名稱>/`：

| package | 放什麼 |
|---|---|
| `specs/00-願景和問題/` | `vision.md` 分開寫 Problem、Principle、Specs 與 Note，保留願景、困難、知識方向與未決構想；`創辦人的話.md` 記錄創辦人的話 |
| `specs/01-制度/` | `constitution.md` 保留組織核心原則與治理規則；申請制度、成員參與制度各自維護具體安排 |
| `specs/02-工作流/` | 志工協作與開源知識的 Problem、已確認機制與未決事項 |
| `specs/03-行政/` | 組織行政工作的固定規定與資料格式；實際邀請經過記於 `logs/邀請日誌.md` |

新的 package 接在既有最大編號之後。每個 package 都要有 `README.md`，說明主要放什麼 subset 的資料及現有文件入口；README 提供導覽，不另存一份可編輯的規則。

同一份文件含多個 layer 時，以唯一的 `# Problem`、`# Principle`、`# Specs` 分開，依上游到下游排列；只寫實際需要的層。討論中的個別構想、候選方案與未決事項放在最後的 `# Note`，不因被引用而成為已確認規則。機制與功能都是具體 Specs，混合文件中的內容集中在 `# Specs`。既有願景檔沿用檔名；憲法以法條維護具體約束。

工作流中的 SOP 寫給人看，以簡短的編號步驟說明要做什麼；不使用 THINK、READ、WRITE、Phase 等 agent 指令格式，不寫工具內部細節。保留完成工作所需的判斷、確認及例外處理即可。

規格正文直接陳述 truth，不交代「初期成員認為」「某人提出」等 speaker 脈絡。原話與討論過程留在 Plan 的需求原文或會議記錄；未決事項直接寫尚未決定。資訊貢獻者名單及實際責任歸屬保留。

規格分四層，由上游到下游。每份規格一個檔，檔名以該層的前綴開頭：

| 層 | 檔名前綴 | 寫什麼 |
|---|---|---|
| Problem | `[Problem]` | 誰在什麼情境想達成什麼、遇到什麼問題，以及哪些 constraints 使問題困難。Problem 是設計的上游依據，不是已選解法。 |
| Principle | `[Principle]` | 為解決上游的 Problem 而採用的抽象設計方針。非必要：解法簡單、方向已清楚時，直接寫下游。 |
| 機制 | `[機制]` | 整體如何運作。每個機制都必須定位到至少一個已定義的 Problem。 |
| 功能 | `[功能]` | 一個具體使用意圖：前置、成功的後置，以及前置成立但沒有完成時的後置。 |

## plans

目前的組織啟動工作統一由 [Kickoff](plans/001-Kickoff/plan.md) 管理；願景、憲法、制度、會議記錄與工作流的既有整理，不再按每一次修改拆成不同 Plan。合併前的需求原文、決策及審查結果保存在同 package 的[歷史紀錄](plans/001-Kickoff/歷史紀錄.md)。

Discord server 的完整設定另由 [discord-server-setup（Discord完整設定）](plans/002-discord-server-setup/plan.md) 接續，包含頻道、權限、新人引導、活動與開放邀請前的驗證；Kickoff 不等待此 Plan 完成。

這次合併整理既有工作的歸屬，不改變憲法中的修憲程序或制度與憲法的分工。未來有獨立範圍需要另建 Plan 時，先依使用者指示確認，不因一次改字、改名或格式調整自行新增。

Plan 不是規格：規則一律寫在 specs；Plan 用引用聚合 specs，不另存第二份可編輯 truth。

文件開頭的 metadata 只保留 `type` 或 `document_type` 類型欄位；移除 `references`、`adopted` 等其他欄位。沒有類型欄位時，不保留 frontmatter。Plan 的交付狀態記於正文的驗收內容。

章節依內容取捨，沒有內容的章節不寫：

| 章節 | 寫什麼 |
|---|---|
| 需求原文 | 提出需求的原話，不改寫；整理後的內容寫在其他章節 |
| As-Is 盤點現況 | 現在是什麼，連到現有規格 |
| 使用者目前覺得的 Problem | 本 Plan 的根項目：每個 Problem 一個子標題，摘要並連到 specs 中的定義 |
| To-Be 目標 | 解決之後的整體改進與可觀察的改變，編號；每一步連到對應的規格 |
| 工程摘要 ＞ 工程戰略 | 改動對象、順序與依賴 |
| 工程摘要 ＞ 規格差異 | 本 Plan 新增、修改與刪除的規格，每一項標注對應的根項目 |
| 驗收 | 完成時要能驗證的結果，可勾選；還沒執行的不勾 |
| 憲法檢查 | 以 subagent 檢查憲法中每一條規則的結論：違反，或沒有違反。Deliver 之前一定要有，而且每一條都沒有違反 |

每個有意義的 commit 都能對回 `git commit → plan → specs truth change`；沒有 specs truth 變更時，commit 或 Plan 明記原因，不虛構 change。

## logs

`logs/` 放會議記錄與執行日誌。會議記錄一場一個檔，檔名以日期開頭；持續追加的邀請日誌固定使用 `logs/邀請日誌.md`，沒有日期前綴，表格內記錄已送出邀請的時間、暱稱、遮蔽帳號、渠道、操作者及備註，不追蹤後續加入結果。會議記錄記的是當時講了什麼，不是規格：規則一律寫在 specs；會議的共識要寫進 specs，由 Plan 引用會議記錄。

logs 也受憲法約束，Deliver／Push 之前一樣以 subagent 檢查憲法中的每一條規則；檢查的結論寫進加入那份會議記錄的 Plan 的「憲法檢查」。
