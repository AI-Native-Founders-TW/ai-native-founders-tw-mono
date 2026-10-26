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
