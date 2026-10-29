# decisions

本檔只 append。每一筆是使用者在本 plan 的一個決策，舊紀錄不改寫；推翻或更正時新增一筆並寫明是哪一筆。目前有效的承諾以 specs truth 為準。格式見 /sf-plan 的 `formats/decisions.md`。

## 決策 001（自介欄位正名）

- 使用者：Johnny Pan <johnny850807@gmail.com>（git author）
- 時間：2026-10-26T22:18:04+08:00
- 互動：主動拍板
- 完整語意：自我介紹中描述可以幫什麼忙、想要幫什麼忙的欄位改稱 Contributions，不再叫 R&R。
- 推翻：無
- 落點：申請制度、members/README.md、招募與 Discord SOP。

## 決策 002（獨立分工指派）

- 使用者：Johnny Pan <johnny850807@gmail.com>（git author）
- 時間：2026-10-26T22:18:04+08:00
- 互動：主動拍板
- 完整語意：R&R assignment 獨立成表；每個 R&R 有一個 Leader，其他人自行 assign 為 Contributors；每個人至少選一個 R&R 作為 Contributors，可選一個或多個。初始 R&R 採用會議記錄中的 R&Rs。
- 推翻：無
- 落點：成員參與制度、members/r-and-r-assignment.md。

## 決策 003（成員總表追溯）

- 使用者：Johnny Pan <johnny850807@gmail.com>（git author）
- 時間：2026-10-26T22:18:04+08:00
- 互動：主動拍板
- 完整語意：在 members 底下新增 members.md，維護所有 member、自介檔案連結及各成員的 R&Rs；members/README.md 說明 traceability matrix。
- 推翻：無
- 落點：members/members.md 與 members/README.md。

## 決策 004（審查裁決權限）

- 使用者：Johnny Pan <johnny850807@gmail.com>（git author）
- 時間：2026-10-27T17:28:45+08:00
- 互動：問答
- 問題：
  > 誰能正式裁決自介 PR？目前 Council team 已存在，但制度尚未授予它審查權。建議 Council 人員審查、AI 協助核對及 comments。選項：Council 人員裁決，AI 協助；所有正式成員都可裁決；由使用者指定。
- 完整語意：Council 人員負責正式裁決自介 PR；AI 只協助核對標準、整理問題與準備 comments，不作最終裁決。
- 推翻：無
- 落點：自介審查制度、自介PR審查SOP、GitHub org Setup、申請制度與相關入口（已同步）。

## 決策 005（一人核准條件）

- 使用者：Johnny Pan <johnny850807@gmail.com>（git author）
- 時間：2026-10-27T17:28:45+08:00
- 互動：問答
- 問題：
  > 自介 PR 需要幾位有審查權的人核准？選項：一位；兩位。問題明列申請者不能審自己，有尚未解決的反對意見時不通過。
- 完整語意：一位有審查權的 Council 人員完整審查並核准即可通過；申請者不能審自己的申請，有未解決的反對意見時不得通過。
- 推翻：無
- 落點：自介審查制度、自介PR審查SOP、GitHub org Setup、申請制度與相關入口（已同步）。

## 決策 006（只授組織成員）

- 使用者：Johnny Pan <johnny850807@gmail.com>（git author）
- 時間：2026-10-27T17:28:45+08:00
- 互動：問答
- 問題：
  > 通過後是否同時加入已有 mono repo Write 的 Members team？選項：org Member ＋ Members team；只加 org Member，繼續 Fork／PR。
- 完整語意：通過後只邀請成為 GitHub org Member，不加入 Members team，後續繼續以 Fork／PR 協作。
- 推翻：無
- 落點：自介審查制度、自介PR審查SOP、GitHub org Setup、申請制度與相關入口（已同步）。

## 決策 007（補件與拒絕處理）

- 使用者：Johnny Pan <johnny850807@gmail.com>（git author）
- 時間：2026-10-27T17:28:46+08:00
- 互動：問答
- 問題：
  > 未通過需要補充時如何 follow up？推薦保留 PR 等本人補件，不設催辦期限；修改後重審。明確違反原則，由審查人說明理由並關閉，保留重新申請方式。選項：保留補件，不定期催辦；7天提醒、14天關閉；自行指定。後續說明推薦選項是不設定定期催辦或逾期關閉。
- 完整語意：需要補充的 PR 保留，等待本人補件後重新審查，不設定定期催辦或逾期關閉。明確違反組織原則的申請，由審查人說明理由後關閉，並提供修正後重新申請的方式。
- 推翻：無
- 落點：自介審查制度、自介PR審查SOP、GitHub org Setup、申請制度與相關入口（已同步）。

## 決策 008（統一啟動範圍）

- 使用者：Johnny Pan <johnny850807@gmail.com>（git author）
- 時間：2026-10-29T18:23:57+08:00
- 互動：主動拍板
- 完整語意：Council、憲法與 Discord 全部合併回 Kickoff，以目前阻擋 launch 的事項統一管理。Plan 必須完整說明，不因合併或行數長而省略必要內容。本次不採納未決治理 Solution，也不宣告 launch 或 adopt。
- 推翻：先前將 Discord 獨立於 Kickoff 的 Plan 歸屬，以及另建 Council Plan 的工作歸屬；既有規則與歷史決策不撤回。
- 落點：plan.md、AGENTS.md 與同 package 的完整歷史附件。

## 決策 009（問題定義歸規格）

- 使用者：Johnny Pan <johnny850807@gmail.com>（git author）
- 時間：2026-10-29T18:28:31+08:00
- 互動：主動拍板
- 完整語意：完整 Problem statement 應寫入 specs；Plan 只有在 specs 已承載時才作簡短交代與引用。保留完整工程 scope、現況、待辦與驗收，不以精簡刪除必要內容。
- 推翻：無
- 落點：plan.md 的 Problem 摘要、scope 與工程摘要；完整 Problem 沿用現有 specs。
