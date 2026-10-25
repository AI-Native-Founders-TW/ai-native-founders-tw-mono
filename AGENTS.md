# ai-native-founders-tw-mono

AI-Native Founders Summit Taiwan 的 specs、plans 與 logs。根層只有 `specs/`、`plans/` 與 `logs/`。

## 憲法

**[`specs/01-憲法/constitution.md`](specs/01-憲法/constitution.md) 是憲法。這個 repo 的所有產出都受憲法約束，不能違反憲法中的任何一條規則。**

AI 在產出完之後，尤其是 Deliver／Push 之前，必須以 subagent 以極度嚴格的角度去檢查是否有違反憲法中的每一條規則：

- 交給 subagent 的是憲法全文與這次產出的實際內容（diff 與改到的檔案全文），不是產出者的摘要。
- 逐條檢查憲法「規則」的每一條與「治理」的每一點，每一條都要有結論：違反，或沒有違反；違反時指出哪個檔案的哪一段。拿不準的算違反。
- subagent 只檢查，不修改。
- 有任何一條違反，就不 Deliver、不 Push，照憲法「治理」處理：改產出，不改憲法；違反的是創辦人的話時，由創辦人自己改；建立或修改憲法的 Plan 裡，憲法本身就是產出。改完再以 subagent 檢查每一條。
- 檢查的結論寫進該 Plan 的「憲法檢查」。

## specs

`specs/` 放 specs truth：上游 why／should、Problem、Forces 與規格。specs 分 package，一個 package 一個目錄 `specs/<編號>-<名稱>/`：

| package | 放什麼 |
|---|---|
| `specs/00-願景和問題/` | `Vision.md` 寫願景與 problem statement，`創辦人的話.md` 記錄創辦人的話 |
| `specs/01-憲法/` | `constitution.md` 是憲法 |
| `specs/02-工作流/` | 還沒有內容 |

新的 package 接在既有最大編號之後。

規格分四層，由上游到下游。每份規格一個檔，檔名以該層的前綴開頭：

| 層 | 檔名前綴 | 寫什麼 |
|---|---|---|
| Problem | `[Problem]` | 誰在什麼情境想達成什麼、遇到什麼問題，以及哪些 constraints 使問題困難。Problem 是設計的上游依據，不是已選解法。 |
| Principle | `[Principle]` | 為解決上游的 Problem 而採用的抽象設計方針。非必要：解法簡單、方向已清楚時，直接寫下游。 |
| 機制 | `[機制]` | 整體如何運作。每個機制都必須定位到至少一個已定義的 Problem。 |
| 功能 | `[功能]` | 一個具體使用意圖：前置、成功的後置，以及前置成立但沒有完成時的後置。 |

## plans

一次變更是一個 Plan：`plans/<編號>-<名稱>/plan.md`。plans 根層每個目錄都是 Plan，使用連續主編號，新 Plan 接在既有最大純數字主編號之後。

Plan 不是規格：規則一律寫在 specs；Plan 用引用聚合 specs，不另存第二份可編輯 truth。

`plan.md` 的 frontmatter 只有 `adopted`：新建為 `false`，這個 Plan 已經 deliver 時改成 `true`。

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

`logs/` 放會議記錄：一場會議一個檔，檔名以日期開頭。會議記錄記的是當時講了什麼，不是規格：規則一律寫在 specs；會議的共識要寫進 specs，由 Plan 引用會議記錄。

logs 也受憲法約束，Deliver／Push 之前一樣以 subagent 檢查憲法中的每一條規則；檢查的結論寫進加入那份會議記錄的 Plan 的「憲法檢查」。
