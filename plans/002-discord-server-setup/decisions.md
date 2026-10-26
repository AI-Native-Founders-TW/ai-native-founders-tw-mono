# decisions

本檔只 append。每一筆是使用者在本 plan 的一個決策，舊紀錄不改寫；推翻或更正時新增一筆並寫明是哪一筆。目前有效的承諾以 specs truth 為準。格式見 /sf-plan 的 `formats/decisions.md`。

## 決策 001（確認四項情境）

- 使用者：Johnny Pan <johnny850807@gmail.com>（git author）
- 時間：2026-10-26T19:15:18+08:00
- 互動：confirm Problem
- 問題：
  > 更新後，Discord 要讓四件事容易：新人理解組織、知道怎麼加入；創業者討論問題、分享經驗、認識彼此；志工號召工作、找到願意一起做的人；發起線上或實體活動，讓有興趣的人容易參與。這四項是否就是這次的完整範圍？確認後，我就據此提出 channels 的整體配置。
- 確認對象：[本次確認對象](./Discord討論紀錄.md#問題確認對象)；記錄版本固定為本輪確認時的四項情境，不隨後續設計改寫。
- 完整語意：確認本次 Discord 設計涵蓋新人開始、創業交流、志工號召工作，以及線上與實體活動的發起與參與；接著討論開放邀請連結前需要的 channels 與 infrastructure。
- 推翻：無
- 落點：specs/02-工作流/[Problem]Discord加入交流與活動.md；plan.md 的 Discord 根項目、To-Be 及規格差異。

## 決策 002（頻道英文命名）

- 使用者：Johnny Pan <johnny850807@gmail.com>（git author）
- 時間：2026-10-26T19:28:53+08:00
- 互動：主動拍板
- 完整語意：Discord 頻道名稱全部使用英文；使用 computer use 查看 AllWill 參考 server 與目標 server 的現況，目標是完成整個 Discord setup。尚未指定或確認本輪新增的完整頻道、權限與角色配置。
- 推翻：無
- 落點：Discord Problem 的英文命名要求、plan.md Discord 範圍與 Discord討論紀錄.md 的現況及整體配置草稿。

## 決策 003（獨立設定計畫）

- 使用者：Johnny Pan <johnny850807@gmail.com>（git author）
- 時間：2026-10-26T19:33:40+08:00
- 互動：新建或沿用 Plan
- 完整語意：將 Discord server setup 自 Kickoff 拆為獨立的 discord-server-setup Plan，承接既有 Problem、英文命名、決策、盤點與候選整體配置，讓 Kickoff 可以先行 push。本次只拆分歸屬，未確認整體設計，也未要求 AI 執行 push。
- 推翻：無
- 落點：plans/002-discord-server-setup/plan.md、decisions.md、Discord討論紀錄.md；Kickoff 移除 Discord 專屬工作並保留導向；AGENTS 更新入口。

## 決策 004（集中混合規格）

- 使用者：Johnny Pan <johnny850807@gmail.com>（git author）
- 時間：2026-10-26T19:39:54+08:00
- 互動：主動拍板
- 完整語意：Discord 相關 Problem、已確認安排、現況與候選設計集中在同一份混合文件，將原 Problem 檔更名為 [機制]Discord-社群-Setup.md。依 Problem、Specs、Note 分層；此裁決是內容組織與命名，不代表尚未確認的配置已採納或 Discord 已設定完成。
- 推翻：無
- 落點：[Discord 社群 Setup](../../specs/02-工作流/[機制]Discord-社群-Setup.md)、工作流 README、plan.md；歷史討論及舊決策保留。

## 決策 005（明列頻道類型）

- 使用者：Johnny Pan <johnny850807@gmail.com>（git author）
- 時間：2026-10-26T19:49:28+08:00
- 互動：主動拍板
- 完整語意：Discord 規格用表格明列 channel、type、描述，並以 clarify 釐清尚未決定的內容。此要求不等於採納目前候選頻道與權限配置。
- 推翻：無
- 落點：[Discord 社群 Setup](../../specs/02-工作流/[機制]Discord-社群-Setup.md)的頻道整體配置表；本輪對話提出待確認事項。

## 決策 006（採納頻道配置）

- 使用者：Johnny Pan <johnny850807@gmail.com>（git author）
- 時間：2026-10-26T19:54:33+08:00
- 互動：問答
- 問題：
  > 是否採用目前的十一個頻道配置？
  > 1. 採用這份配置（推薦：四種使用情境各有明確位置）：沿用既有頻道，新增規則、公告、深入討論與管理紀錄。
  > 2. Others：指出要刪減、合併或調整的頻道。
- 完整語意：使用者依序回答「1. 1」「2. 1」「3. 1」，本題選擇第一項。採用提問時的十一個頻道配置，包含 Category、Channel、Type 與描述；保留既有訊息與論壇串。其餘未確認的平台設定不因此獲採納。
- 推翻：無
- 落點：[Discord 社群 Setup](../../specs/02-工作流/[機制]Discord-社群-Setup.md#頻道整體配置)；plan.md 的規格差異、待辦與驗收。

## 決策 007（開放活動建立）

- 使用者：Johnny Pan <johnny850807@gmail.com>（git author）
- 時間：2026-10-26T19:54:33+08:00
- 互動：問答
- 問題：
  > 誰可以自行建立活動排程？
  > 1. 所有加入者（推薦：符合容易辦活動的目標）：可建立自己的活動；管理全部活動仍限管理者。
  > 2. 審查通過的組織成員：須先完成既有入會程序，才能建立活動排程。
  > 3. 僅管理者：其他人先提出活動，再由管理者建立排程。
  > 4. Others：補充其他權限安排。
- 完整語意：使用者依序回答「1. 1」「2. 1」「3. 1」，本題選擇第一項。所有 server 加入者均可自行建立自己的原生 Events 活動排程，管理全部活動仍限管理者；不以組織成員資格作為建立活動的條件。
- 推翻：無
- 落點：[Discord 社群 Setup](../../specs/02-工作流/[機制]Discord-社群-Setup.md#活動建立與管理權限)；plan.md 的規格差異、待辦與驗收。

## 決策 008（不新增管理授權）

- 使用者：Johnny Pan <johnny850807@gmail.com>（git author）
- 時間：2026-10-26T19:54:33+08:00
- 互動：問答
- 問題：
  > 這次是否新增管理者或公告發布者？
  > 1. 先不新增授權（推薦：先完成配置，避免自行擴張權限）：保留既有管理權；公告先由既有管理者發布。
  > 2. 現在指定人選：請列出人選，並註明「管理」或「僅發布公告」。
  > 3. Others：補充其他分工方式。
- 完整語意：使用者依序回答「1. 1」「2. 1」「3. 1」，本題選擇第一項。本次不新增管理者或公告發布者，維持既有管理權，公告先由既有管理者發布；不自行新增人選或擴張授權。
- 推翻：無
- 落點：[Discord 社群 Setup](../../specs/02-工作流/[機制]Discord-社群-Setup.md#管理與公告發布)；plan.md 的規格差異、待辦與驗收。
