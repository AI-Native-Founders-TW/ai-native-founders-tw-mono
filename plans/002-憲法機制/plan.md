---
adopted: false
---

# 憲法 specs/constitution 機制

## 需求原文

> 接著我想要打一下憲法 specs/constitution 機制
>
> 並且在 AGENTS.md 中會去強調憲法約束，請 AI 在產出完之後，尤其是 Deliver/Push 之前，必須以 subagent 以極度嚴格的角度去檢查是否有違反憲法中的每一條規則。

> 你可以參考 SpecKit

對這個組織的治理：

> 不用有拍板啦

對創辦人的話裡這一句算不算商業意圖：

> 如果這個組織能夠幫助我自己，還有我很棒的團隊做出能出海的 Business 的話，那一定也能幫助其他的台灣人。
>
> 這句不算，NPO 本來就要有 value proposition
> value proposition 要定義清楚在憲法中，目的本身可以容忍，其他的商業意圖講清楚怎麼區分那才是憲法中比較需要明定的

對建立憲法的過程：

> 另外上述迭代過程別紀錄，不想在 kickoff 時有這麼多複雜的脈絡

創辦人選定寫進憲法的內容（選項文字由 AI 擬）：

- 其他的商業意圖怎麼區分：
    - 此組織給的 value，每個人都拿得到的（包含創辦人自己的創業），不算商業意圖；只有付錢的人或特定公司拿得到的，就是商業意圖。
    - 不用此組織的名義、筆記或活動，推銷特定公司的產品或服務，包含創辦人自己的公司。
    - 不收錢換筆記或活動裡的廣告、置入或推薦。
    - 此組織如果有收入，只用在此組織的活動，不分給任何人。
- 「有正向意圖、是個良好的公民」是對每個人的期待，不是門檻，沒有人審核；申請就能加入。

## As-Is 盤點現況

- `specs/` 有 [Vision](../../specs/Vision.md) 與 [創辦人的話](../../specs/創辦人的話.md)，還沒有憲法。
- [AGENTS.md](../../AGENTS.md) 只寫 specs 與 plans 的寫法；AI 產出完之後、Deliver／Push 之前，沒有任何檢查。

## 使用者目前覺得的 Problem

### 是否有違反憲法中的每一條規則

AI 在產出完之後，尤其是 Deliver／Push 之前，沒有以 subagent 去檢查是否有違反憲法中的每一條規則。

### 其他的商業意圖怎麼區分

NPO 本來就要有 value proposition，但 value proposition 還沒有定義清楚；目的本身可以容忍，其他的商業意圖怎麼區分也還沒有講清楚。

## To-Be 目標

1. 憲法寫在 `specs/constitution.md`：每一條都有名稱、規則與出處，可以逐條檢查（[憲法](../../specs/constitution.md)）。
2. 憲法定義清楚 value proposition，並講清楚其他的商業意圖怎麼區分（[憲法](../../specs/constitution.md#第-2-條value-proposition)）。
3. AGENTS.md 強調憲法約束：AI 在產出完之後，尤其是 Deliver／Push 之前，必須以 subagent 以極度嚴格的角度去檢查是否有違反憲法中的每一條規則（[AGENTS.md](../../AGENTS.md#憲法)）。
4. 每個 Plan 在 Deliver 之前都有「憲法檢查」，寫出每一條的結論。

## 工程摘要

### 工程戰略

參考 SpecKit 的 constitution，取三件事：

- 憲法是一個檔：SpecKit 放在 `memory/constitution.md`，這裡放在 `specs/constitution.md`。
- Plan 裡有憲法檢查：對應 SpecKit plan template 的 Constitution Check。
- 和憲法衝突時改產出、不改憲法，要改憲法另外做：對應 SpecKit `analyze` 的 Constitution Authority。

SpecKit 的版本號與 Ratified／Last Amended 日期不採用：修改紀錄由 Plan 與 git 承擔。

條文從 Vision、創辦人的話與需求原文取出，逐字沿用。順序：先寫 `specs/constitution.md`，再在 AGENTS.md 加「憲法」一節、在 plans 的章節表加「憲法檢查」，最後以 subagent 檢查整個 repo。

### 規格差異

1. 新增 [憲法](../../specs/constitution.md)：第 1 條到第 8 條與治理。第 2 條（value proposition）與第 3 條（其他的商業意圖怎麼區分）對應 [其他的商業意圖怎麼區分](#其他的商業意圖怎麼區分)；其餘對應 [是否有違反憲法中的每一條規則](#是否有違反憲法中的每一條規則)。

## 驗收

- [x] 1. 定位在 `specs/constitution.md`。動作是逐條對回出處。
    - 預期：每一條的規則都找得到出處的原句，沒有出處裡沒有的詞。

## 憲法檢查

範圍：整個 repo，含還沒 push 的 commit。

| 條文 | 結論 |
|---|---|
| 第 1 條　公益性質的非營利組織 | 沒有違反 |
| 第 2 條　value proposition | 沒有違反 |
| 第 3 條　其他的商業意圖怎麼區分 | 沒有違反 |
| 第 4 條　附上所有資訊貢獻者 | 沒有違反 |
| 第 5 條　大家共同編輯協作 | 沒有違反 |
| 第 6 條　不會限制任何門檻 | 沒有違反 |
| 第 7 條　不會要求你一定要幫忙 | 沒有違反 |
| 第 8 條　Open-Minded | 沒有違反 |
| 治理：都受憲法約束 | 沒有違反 |
| 治理：原話不改寫 | 拿不準：[visioning 的 Plan](../001-visioning-and-problem-statement/plan.md#需求原文) 引用的 2026-10-21 貼文，和 Threads 上現在的貼文不一樣；等創辦人決定 specs 要不要照現在的貼文改 |
| 治理：修改憲法 | 沒有違反 |
| 治理：怎麼檢查 | 沒有違反 |
