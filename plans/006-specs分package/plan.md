---
adopted: false
---

# specs 分 package

## 需求原文

> specs 分一下 package
> 我想區分
>
> 00-願景和問題
> 01-憲法
> 02-工作流
>
> packages

## As-Is 盤點現況

- `specs/` 根層平放三份檔：`Vision.md`、`創辦人的話.md`、`constitution.md`。
- AGENTS.md 的 specs 一節寫「其他規格依業務編號分目錄 `specs/<業務編號>/`，業務編號連續，沒有內容就缺號」。

## 使用者目前覺得的 Problem

### specs 沒有分 package

specs 沒有區分 00-願景和問題、01-憲法、02-工作流三個 package。package 的定義寫在 [AGENTS.md 的 specs 一節](../../AGENTS.md#specs)。

## To-Be 目標

1. specs 分成三個 package：[00-願景和問題](../../specs/00-願景和問題/)、[01-憲法](../../specs/01-制度/)、`specs/02-工作流/`。
2. [AGENTS.md](../../AGENTS.md#specs) 列出三個 package 各放什麼。
3. repo 裡指到這三份檔的連結都指到新位置。

## 工程摘要

### 工程戰略

只搬檔與改連結。

- `Vision.md` 與 `創辦人的話.md` 放 `00-願景和問題`。創辦人的話放這裡是 AI 的決定，依據是 2026-10-22 的需求「幫我記錄我的 創辦人的話.md next to vision doc」（[Plan 001（visioning 與 problem statement）](../001-visioning-and-problem-statement/plan.md#需求原文)）。
- `constitution.md` 放 `01-憲法`。憲法搬位置一定會改到它裡面的相對連結，照憲法治理「修改憲法要在專門修改憲法的 Plan 裡做」，搬憲法與改憲法裡的連結交給 [Plan 007（憲法搬進 01-憲法）](../007-憲法搬進01-憲法/plan.md)，本 Plan 不改憲法。兩個 Plan 一起 commit、一起 Deliver。
- `02-工作流` 還沒有內容，放一個空的 `.gitkeep` 讓目錄留在 git 裡；AGENTS.md 寫「還沒有內容」。
- AGENTS.md 原本的「業務編號連續，沒有內容就缺號」改成 package 表與「新的 package 接在既有最大編號之後」，因為 02-工作流 是創辦人指定、現在沒有內容的 package。
- Plan 001 到 005 只改可以點的連結，指到新位置。反引號裡的路徑、憲法檢查的紀錄、需求原文與關鍵決策裡引用的原話（例如 Plan 005（第一次核心會議萃取進 Vision）的 `ai-native-founders-tw-mono/specs/Vision.md`）都不改，保留當時的寫法。
- 本 Plan 先在本地 commit，不 push。

### 規格差異

1. 搬移 `specs/Vision.md` → [specs/00-願景和問題/vision.md](../../specs/00-願景和問題/vision.md)，只改三行四個連到會議記錄與憲法的連結路徑。對應 [specs 沒有分 package](#specs-沒有分-package)。
2. 搬移 `specs/創辦人的話.md` → [specs/00-願景和問題/創辦人的話.md](../../specs/00-願景和問題/創辦人的話.md)，內容不變。對應 [specs 沒有分 package](#specs-沒有分-package)。
3. 新增 `specs/02-工作流/`，還沒有內容。對應 [specs 沒有分 package](#specs-沒有分-package)。
4. 修改 [AGENTS.md](../../AGENTS.md#specs) 的 specs 一節，以及憲法一節連到憲法的路徑。對應 [specs 沒有分 package](#specs-沒有分-package)。

## 驗收

- [x] 1. 定位在 repo 全部 Markdown。動作是逐一解析相對連結。
    - 預期：每個連結都指到存在的檔案。
- [x] 2. 定位在搬過的兩份檔。動作是和搬之前比對 diff。
    - 預期：創辦人的話內容沒有變；Vision 只有三行四個連結的路徑變。

## 關鍵決策

- 2026-10-25：「specs 分一下 package 我想區分 00-願景和問題 01-憲法 02-工作流」。寫進 [AGENTS.md](../../AGENTS.md#specs)。

其餘是 AI 的決定，不是創辦人的決策：創辦人的話放 00-願景和問題；02-工作流 先放空的 `.gitkeep`；拿掉「沒有內容就缺號」，改成「新的 package 接在既有最大編號之後」；搬憲法另開 Plan 007（憲法搬進 01-憲法）。

## 憲法檢查

範圍：本 Plan 與 Plan 007（憲法搬進 01-憲法）全文、staged 的全部 diff、AGENTS.md 全文，以憲法全文為準（2026-10-25）。第一輪指出憲法搬家改到出處連結，本 Plan 不是專門修改憲法的 Plan；之後搬憲法交給 Plan 007，Plan 001 到 005 只改可點的連結。第二輪結論：每一條都沒有違反。全部 127 個相對連結與錨點都存在。

| 條文 | 結論 | 依據 |
|---|---|---|
| 第 1 條　公益性質的非營利組織 | 沒有違反 | 只搬檔、改連結與改 AGENTS.md 的 specs 一節，沒有商業內容。 |
| 第 2 條　value proposition | 沒有違反 | 憲法條文與 Vision 遮掉連結後全文相同。 |
| 第 3 條　其他的商業意圖怎麼區分 | 沒有違反 | 沒有推銷、置入或收入相關的內容。 |
| 第 4 條　附上所有資訊貢獻者 | 沒有違反 | Vision 與創辦人的話除了連結以外全文相同，貢獻者名字都在。 |
| 第 5 條　大家共同編輯協作 | 沒有違反 | package 表沒有加上拍板或權限限制。 |
| 第 6 條　唯一的門檻是自介 | 沒有違反 | 沒有碰到入會規則。 |
| 第 7 條　不會要求你一定要幫忙 | 沒有違反 | 沒有碰到參與義務。 |
| 第 8 條　Open-Minded | 沒有違反 | 沒有和背景或封閉有關的內容。 |
| 治理：都受憲法約束 | 沒有違反 | 沒有用重新解讀條文的方式放行；本 Plan 寫明不改憲法。 |
| 治理：原話不改寫 | 沒有違反 | Plan 001、002、004、005 遮掉連結後全文相同，需求原文、關鍵決策、反引號路徑與憲法檢查紀錄都沒變；創辦人的話內容沒變；引用 Plan 001 的「next to vision doc」逐字相符。 |
| 治理：修改憲法 | 沒有違反 | 搬憲法交給 Plan 007；AGENTS.md 改的是連到憲法的路徑，不是憲法本身。 |
| 治理：怎麼檢查 | 沒有違反 | 由 subagent 拿憲法全文、diff 與檔案全文逐條檢查，結論寫在本節。 |
