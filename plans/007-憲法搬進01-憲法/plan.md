---
adopted: false
---

# 憲法搬進 01-憲法

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

憲法在 `specs/constitution.md`。第 1 條到第 8 條各有「出處」，連到創辦人的話、Vision、Plan 與會議記錄；治理第四點連到 AGENTS.md。

## 使用者目前覺得的 Problem

### 憲法沒有放進 01-憲法

[Plan 006（specs 分 package）](../006-specs分package/plan.md#specs-沒有分-package) 的 package 裡，憲法要放進 [01-憲法](../../AGENTS.md#specs)。

## To-Be 目標

1. 憲法在 [specs/01-憲法/constitution.md](../../specs/01-憲法/constitution.md)，裡面的連結都指到存在的檔案。

## 工程摘要

### 工程戰略

這是專門修改憲法的 Plan。改哪一條、為什麼改：

- 改哪裡：第 1 條到第 8 條的「出處」連結路徑，以及治理第四點連到 AGENTS.md 的路徑。
- 為什麼改：憲法從 `specs/` 搬進 `specs/01-憲法/`，創辦人的話與 Vision 搬進 `specs/00-願景和問題/`（[Plan 006（specs 分 package）](../006-specs分package/plan.md)），相對路徑不改就會斷。
- 不改：條文的文字、出處連到哪一份文件。

和 Plan 006（specs 分 package）一起 commit、一起 Deliver。本 Plan 先在本地 commit，不 push。

### 規格差異

1. 搬移 `specs/constitution.md` → [specs/01-憲法/constitution.md](../../specs/01-憲法/constitution.md)，修改第 1 條到第 8 條的出處連結路徑與治理第四點的 AGENTS.md 連結路徑。對應 [憲法沒有放進 01-憲法](#憲法沒有放進-01-憲法)。

## 驗收

- [x] 1. 定位在憲法。動作是和搬之前比對 diff。
    - 預期：只有第 1 條到第 8 條的出處與治理第四點的連結路徑變，條文的文字沒有變。
- [x] 2. 定位在憲法的每個連結。動作是逐一解析。
    - 預期：每個連結都指到存在的檔案與錨點。

## 關鍵決策

- 2026-10-25：見[需求原文](#需求原文)，01-憲法 是創辦人指定的 package。

其餘是 AI 的決定，不是創辦人的決策：搬憲法另開本 Plan，不放在 Plan 006（specs 分 package）。

## 憲法檢查

範圍：本 Plan 與 Plan 006（specs 分 package）全文、staged 的全部 diff，以憲法全文為準（2026-10-25，第二輪）。結論：每一條都沒有違反。

| 條文 | 結論 | 依據 |
|---|---|---|
| 第 1 條到第 8 條 | 沒有違反 | 條文文字沒變，只有出處的連結路徑變；本 Plan 沒有牴觸這 8 條的內容。 |
| 治理：都受憲法約束 | 沒有違反 | 憲法在專門修改憲法的 Plan 裡改，不是拿來給其他產出放行。 |
| 治理：原話不改寫 | 沒有違反 | 需求原文和 Plan 006 逐字相同；AI 的決定另外標明。 |
| 治理：修改憲法 | 沒有違反 | 寫明改哪裡（第 1 條到第 8 條的出處、治理第四點）、為什麼改、不改什麼；範圍和 diff 一致：17 個連結都在這九行，連到的檔案與錨點沒變。 |
| 治理：怎麼檢查 | 沒有違反 | 治理第四點連到 `../../AGENTS.md#憲法`，連結有效；結論寫在本節。 |
