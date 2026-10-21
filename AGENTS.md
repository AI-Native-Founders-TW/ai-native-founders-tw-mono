# ai-native-founders-tw-mono

AI-Native Founders Summit Taiwan 的 specs 與 plans。根層只有 `specs/` 與 `plans/`。

## specs

`specs/` 放 specs truth：上游 why／should、Problem、Forces 與規格。`specs/Vision.md` 寫願景與 problem statement；其他規格依業務編號分目錄 `specs/<業務編號>/`，業務編號連續，沒有內容就缺號。

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

每個有意義的 commit 都能對回 `git commit → plan → specs truth change`；沒有 specs truth 變更時，commit 或 Plan 明記原因，不虛構 change。
