---
adopted: false
---

# 第一次核心會議萃取進 Vision

## 需求原文

> ai-native-founders-tw-mono/logs/20261024-第一次核心會議-會議記錄.md
>
> 把這文充分萃取寫進去 ai-native-founders-tw-mono/specs/Vision.md
> 適當分層級做 formulation
>
> 會議中全部提到的共識決議如果有背後的 vision & problem 都要好好萃取，不能漏掉

## As-Is 盤點現況

- [Vision](../../specs/Vision.md) 有「我們希望改變什麼」、三個 Problem statement（出海創業之路該怎麼進行、upfront plan 和募資成本計算、攻略跟流派）與「我們希望留下什麼」，都來自 2026-10-21 的發起貼文與訊息。
- [第一次核心會議](../../logs/20261024-第一次核心會議-會議記錄.md)（2026-10-24）有 7 條決議、四個議題的分享與未決事項，還沒有進 specs。

## 使用者目前覺得的 Problem

### 會議的 vision 與 problem 沒有進 Vision

會議中全部提到的共識決議，背後的 vision 與 problem 還沒有萃取進 Vision。

## To-Be 目標

1. 「我們希望改變什麼」加上這個Organization最重要的一個目的，與會中提出的對臺灣新創社會的終局改變（[Vision](../../specs/Vision.md#我們希望改變什麼)）。
2. Problem statement 原有三個之後，跟著會議 Miro 上的 Frame 加兩段：對臺灣新創社會、你加入這個NPO 你想要的Benefit是什麼（[Vision](../../specs/Vision.md#problem-statement)）。
3. 7 條決議每一條背後的 problem 都寫出來（[每一條決議背後的 problem](../../specs/Vision.md#每一條決議背後的-problem)）。
4. 還沒有收斂、背後有 problem 的列出來，連到會議記錄的未決事項（[open issue](../../specs/Vision.md#open-issue)）。

## 工程摘要

### 工程戰略

原有內容不動，只加。新加的段落以原話為主：引號內逐字取自會議字幕（以腳本逐句核對），引號後是那句話開始的錄影時間，前面寫說話者。標題用發言者講過的詞或 Miro 卡片上的字，不另取標題；決議背後的 problem 用會議記錄的決議編號當標題。

「分層級」的做法是 AI 的決定：Vision 由上到下是我們希望改變什麼 → Problem statement → 我們希望留下什麼；新加的段落跟著會議 Miro 上的 Frame 分段，再加每一條決議背後的 problem 與 open issue。決議本身（Discord、PR 自介、Mono 加 submodule、ownership 分工）是機制，不寫進 Vision；寫進憲法的部分在 [Plan 004（依第一次核心會議修憲）](../004-依第一次核心會議修憲/plan.md)。

會中沒有表決的內容（三個區隔、信任與賽道兩層等）照實寫明是誰提的、沒有表決，不寫成「會中」的結論。

本 Plan 先在本地 commit，不 push。

### 規格差異

1. 修改 [Vision](../../specs/Vision.md)：「我們希望改變什麼」加兩段，Problem statement 加四段（對臺灣新創社會、你加入這個NPO 你想要的Benefit是什麼、每一條決議背後的 problem、open issue）。對應 [會議的 vision 與 problem 沒有進 Vision](#會議的-vision-與-problem-沒有進-vision)。

## 驗收

- [ ] 1. 定位在 Vision 新加的段落。動作是逐句對回會議字幕。
    - 預期：引號內逐字找得到；時間對得上。
- [ ] 2. 定位在會議記錄的 7 條決議。動作是逐條找 Vision「每一條決議背後的 problem」裡對應的段落。
    - 預期：D1（搬到 Discord）到 D7（誰 care 誰 own）每一條都有。

## 關鍵決策

- 2026-10-24：「把這文充分萃取寫進去 ai-native-founders-tw-mono/specs/Vision.md 適當分層級做 formulation」「會議中全部提到的共識決議如果有背後的 vision & problem 都要好好萃取，不能漏掉」。寫進 [Vision](../../specs/Vision.md)。

其餘是 AI 的決定，不是創辦人的決策：分層的方式；從原話或 Miro 卡片挑哪幾個字當標題；決議本身不寫進 Vision。

## 憲法檢查

範圍：本 Plan 全文、`specs/Vision.md` 的 diff 與全文，以修改後的憲法為準；引號與時間對照會議字幕（2026-10-24，第一輪）。第一輪結論：第 4 條、第 5 條、第 6 條、第 8 條與治理「原話不改寫」違反（拿不準），本 Plan 還不能 Deliver；本 Plan 引用 Plan 004（依第一次核心會議修憲）改過的憲法，不能比它先 Deliver。

| 條文 | 結論 | 依據 |
|---|---|---|
| 第 1 條　公益性質的非營利組織 | 沒有違反 | 「我要飛了」同一句原話寫了「帶大家一起去」「獨享不如眾樂」，落在第 2 條容忍的範圍內。 |
| 第 2 條　value proposition | 沒有違反 | 沒有限縮或否定第 2 條列的 value。 |
| 第 3 條　其他的商業意圖怎麼區分 | 沒有違反 | AppWorks、886、YC、GCP、AWS、GitHub、Discord 只出現在討論中；水球介紹自己公司與方法論的段落沒有搬進 Vision。 |
| 第 4 條　附上所有資訊貢獻者 | 違反（拿不準） | 第一輪：Vision 沒有寫說話者可能錯置。之後已在檔頭寫明。 |
| 第 5 條　大家共同編輯協作 | 違反（拿不準） | 第一輪：四處把個人的話或沒表決的內容寫成「會中」的結論。之後已改成寫出說話者，信任與賽道兩層標明會中沒有表決。 |
| 第 6 條　唯一的門檻是自介 | 違反（拿不準） | 第一輪：D5（有心但菜也能加入）的標題與內文讀起來像自介之外還有信任、賽道兩關；D1（搬到 Discord）沒寫 Discord 不是門檻。之後標題改成決議編號，寫明入會門檻只有自介、Discord 不是門檻。 |
| 第 7 條　不會要求你一定要幫忙 | 沒有違反 | 「希望用自己的方式去貢獻」和第 7 條一致。 |
| 第 8 條　Open-Minded | 違反（拿不準） | 第一輪：「範疇」列為 open issue，和「不看背景」衝突；Vision 沒寫錄影不公開。之後「範疇」改寫成入會不看背景、分組或賽道要不要限縮還沒有共識；檔頭寫明錄影不公開。 |
| 治理：都受憲法約束 | 沒有違反 | 沒有用重新解讀條文的方式放行。 |
| 治理：原話不改寫 | 違反（拿不準） | 第一輪：AppWorks 那句的轉述把說話的角度反過來；「AI 也讀不到」不是原話；AI 自創的標題；時間範圍沒包到引號、時間標準不一。之後已改成整句引用原話、刪掉「AI 也讀不到」改引「AI就完全在這個Context裡面」、標題改用原話或 Miro 卡片的字、每句原話後面標那句話開始的時間；待下一輪複查。 |
| 治理：修改憲法 | 沒有違反 | 本 Plan 只改 Vision。 |
| 治理：怎麼檢查 | 沒有違反 | 由 subagent 拿憲法全文、Vision 的 diff 與全文、Plan 全文和會議字幕逐條檢查。 |
