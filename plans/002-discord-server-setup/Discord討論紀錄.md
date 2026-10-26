# Discord 討論歷史紀錄

以下保留過往原話、確認對象及提案演變，不再維護目前配置。現行 Problem、設定與候選方案集中於 [Discord 社群 Setup](../../specs/02-工作流/[機制]Discord-社群-Setup.md)。歷史草稿中的中文頻道名、權限與平台推測均不作為現在的設定依據。

## 問題確認對象

本節固定保存本次確認的對象，不隨後續設計改寫。

- 新人理解組織、知道怎麼加入。
- 創業者討論問題、分享經驗、認識彼此。
- 志工號召工作、找到願意一起做的人。
- 發起線上或實體活動，讓有興趣的人容易參與。

共同約束：參與者各有工作、時間有限；重要內容不能一直被聊天洗掉；不能靠要求每天發言製造熱絡。加入、參與及認領仍依既有制度與憲法。這次確認範圍，不採納尚未提出的具體頻道或權限配置。

## 目前位置

Problem 已確認並同步；進入整體設計思考。使用者要求先討論開放邀請前必要的 channels 與 infrastructure，整體設計尚未確認，未操作 Discord。

## 原文

> yeah continue, what discord channels or infra must be setup before people join via link?

## 開放邀請前的整體提案草稿

以下僅是本輪建議，尚未採納，也未設定 Discord。

公開入口與交流空間：

| 頻道 | 類型 | 用途 |
|---|---|---|
| 先看這裡 | 唯讀文字 | 組織目的、現行規則、repo、自介 PR 與提問入口；不在 Discord 另建第二套成員資格 |
| 公告 | 唯讀文字 | 重要消息與已確定活動，由管理者發布 |
| 交流大廳 | 文字 | 打招呼、閒聊、即時問答與新人求助；不另要求一份 Discord 自介作入會資格 |
| 問題與經驗 | 論壇 | 一個問題或經驗一篇，相關討論留在同篇 |
| 一起做事 | 論壇 | 號召志工、說明工作及需要的幫忙；活動籌備也能在此找人 |
| 活動與聚會 | 論壇 | 一場活動一篇，保存目的、時間地點、參與方法與活動討論 |
| 線上交流 | 語音 | Coffee Chat、工作討論與小型線上活動；同時活動增加後再考慮第二間 |

管理者另有不對一般參與者開放的「管理紀錄」文字頻道，接收 Discord Community 更新及安全警示；不在其中自創組織決策權，也不搬入本來無權取得的私人資料。

開放前建議完成：

1. 啟用 Community，完成平台要求的已驗證信箱、媒體檢查、規則及管理更新頻道設定。這是平台設定，不取代組織申請制度。
2. 有一位已確認的伺服器擁有者與可處理問題的管理者。一般受邀者可看說明、交流、提問、號召與提出活動；管理伺服器、管理身分組、管理頻道及全體提及權限不開給一般參與者。具體管理者人選要在實際設定前確認。
3. 建議以「組織成員」身分組承接既有審查通過的成員資格，先由指定管理者依資格證據人工設定；不假設 PR 合併就會自動給 Discord 身分。組織成員可建立及管理自己的 Scheduled Events，管理者可管理全部活動。此權限提案尚未採納，審查人與制度程序不在本輪自行決定。
4. 啟用基本防垃圾訊息及大量提及的 AutoMod，警示送管理紀錄；正常提問仍需要有人回應。
5. 先放好歡迎說明、repo 與申請連結、論壇發文引導及未有活動時的說明，避免空頻道讓新人不知下一步。活動尚未建立時不預填真實日期、地點或出席承諾。
6. 用測試帳號從邀請連結走一遍，核對一般參與者看到的內容、可發文及進語音；測試論壇、活動權限與管理頻道隔離，才開放連結。現有連結尚未實測，不以文件存在推定有效。

原生 Events 用於活動排程與表達參與興趣；論壇保存詳情與討論。若活動有名額、付費、審核或其他報名需求，需另行確認適合的報名方式，Discord 的 Interested 不直接等於完成該類報名。線下活動使用 Somewhere Else 的實際地點；線上活動連到語音或實際會議位置。

第一版暫不要求完整 Community Onboarding、不新增自介機器人或自動核准流程、不預建各產業／地區頻道。Onboarding 的預設頻道數量要求會增加第一版配置負擔；需要時再根據實際討論與參與情形調整。

### 整體配置的比較

- 全部放單一聊天室：建立最快，但四類使用情境會混在一起，問題、招募及活動資訊較難持續定位。
- 一開始按產業與地區切很多頻道：分類較細，但增加新人判斷去哪裡的成本，也需要更多維護。
- 本輪建議：入口與公告獨立、即時交流用文字、需要持續接續的問題／工作／活動分成論壇，再共用一個語音空間。代價是要先啟用 Community，並讓參與者理解每篇論壇是一個主題。

拿掉活動論壇後只剩排程清單，活動細節及討論缺少固定位置；拿掉原生 Events 仍能辦活動，但排程與表達參與興趣要靠文字接續。語音可先共用，不需要在尚無同時活動的依據下增設多間。論壇數量可以再裁減，但工作號召與活動公開參與的用途需保持清楚。

### 官方能力依據（2026-10-26 查核）

- [論壇需要 Community](https://support.discord.com/hc/en-us/articles/6208479917079-Forum-Channels-FAQ)。
- [Community 的必要設定](https://support.discord.com/hc/en-us/articles/360047132851-Enabling-Your-Community-Server)。
- [Scheduled Events 與建立／管理權限](https://support.discord.com/hc/en-us/articles/4409494125719-Scheduled-Events)。
- [角色與管理權限](https://support.discord.com/hc/en-us/articles/214836687-Discord-Roles-and-Permissions)。
- [AutoMod](https://support.discord.com/hc/en-us/articles/4421269296535-AutoMod-FAQ)。
- [完整 Onboarding 目前要求至少七個預設頻道、其中五個允許所有人查看並發訊息](https://support.discord.com/hc/en-us/articles/11074987197975-Community-Onboarding-FAQ)。

### 檢驗限制

Auto-sync 啟動器已先以 dry-run 預覽，沒有啟動正式輪次。此專案沿用 Kickoff，啟動器尚未建立檢驗基準，預覽會一併納入其他既有根項目；其 truth 範圍仍設定為 SF mindmap，未把本 repo 的 specs 納入 truth_sync。此結果不當成本輪已檢驗或需求就緒；本輪仍需專案要求的獨立憲法檢查，並等待使用者確認整體設計。

## 英文命名與現況盤點（2026-10-26）

### 使用者原文

> 頻道都是 english name
>
> 然後你參考一下 discord 的 computer use 看一下目前我的 allwill server長怎樣
>我目標是要把 discord 整個 setup 好

本輪以 computer use 唯讀操作原生 Discord，目標仍為 AI-Native Global Founders Speedrun Taiwan；AllWill 所用、目前顯示名稱為 specformula.ai 的 server 僅供參考，未修改。參考來源的私人訊息與公司內部內容不移入本 repo。

### 已觀察的目標 server

- 既有文字頻道：welcome、onboard、chit-chat、funding。
- 既有論壇：events、collaborations，已有討論串，應保留。
- 既有語音：General。
- onboard 畫面顯示頻道起始頁，沒有加入步驟；welcome 的首次訊息列表尚未顯示內容，未據此斷言永久空白。
- 設定頁顯示 Enable Community，Community 尚未啟用。既有兩個論壇仍可在側欄定位；不再用官方文件的 Community 必要條件推斷現有論壇不存在。
- Roles 頁只有預設權限入口，沒有顯示任何自訂角色。
- @everyone 的 Create Events 與 Mention @everyone, @here, and All Roles 為 on；Manage Events、Manage Channels、Manage Roles、Manage Server、Administrator 為 off。
- Safety Setup 顯示 Verification Level 為 None、Sensitive content filters 為 Do not filter，安全通知頻道未選定。未改動這些值。

### 參考方式與前輪更正

參考 server 已啟用 Community、Onboarding 與 Server Guide，使用公開公告、用途明確的論壇、新人任務及規則入口。這些可作為設計參考，不複製公司的私人權限結構到本組織。

參考 server 的實際 Default Channels 設定畫面列出十個預設頻道，並顯示 Must include 1 channel where @everyone can read and send messages。此畫面與前輪查到的官方 FAQ 七個預設、五個可發言的敘述不同。目標 server 的 Onboarding 尚不可從現況讀取；實作時須以目標介面的實際條件確認，不預建無用途的頻道湊數，也不宣稱已完成啟用。

### 取代前輪中文頻道草稿的整體配置（尚未採納）

頻道與 category 名稱均為英文。歡迎、規則、說明與發文引導先以繁體中文呈現，方便目前參與者理解；這是候選內容安排，尚未發布。

| Category | 頻道 | 處理與用途 |
|---|---|---|
| start-here | welcome | 沿用，補組織介紹與下一步，唯讀 |
| start-here | onboard | 沿用，補閱讀規格、repo、自介 PR 及提問入口，唯讀；不另設第二次入會審查 |
| start-here | rules | 新增，提供簡短平台交流規則及現行憲法／制度連結，唯讀；不另改組織規則 |
| start-here | announcements | 新增，發布重要公告與已確認活動，只有伺服器擁有者或指定發布者可發布 |
| community | chit-chat | 沿用，打招呼、閒聊、即時問答與新人求助 |
| community | funding | 沿用，保留原有募資交流用途與內容 |
| community | discussions | 新增論壇，一個問題或經驗一篇；長期有用的知識再依既有規格整理到 repo |
| get-involved | collaborations | 沿用論壇，一件號召工作或活動籌備一篇，保留既有串 |
| get-involved | events | 沿用論壇，一場活動一篇，保存詳情與討論；確定排程後連到原生 Events |
| voice | lounge | 將既有 General 改為英文小寫 lounge，共用即時交流與小型活動空間 |
| management | mod-log | 新增私有文字頻道，接 Community 更新與 AutoMod 警示；只有伺服器擁有者及指定管理者可見 |

此版本沿用既有頻道，加入公告、規則、深入討論及管理入口。前輪把正式 Events 限於已確認組織成員的做法只是候選；現況已允許一般加入者自行建立活動，為回應容易辦活動的目的，本輪改建議保留這項權限，而非另設逐場核准或先審成員的門檻。沒有把這個候選變更寫成制度 truth。

### 完整 setup 的交付範圍（尚未採納）

1. 依上表整理 categories 及 channels，保留既有訊息與論壇串；設定 topic、用途說明、論壇發文引導及必要標籤。
2. 完成 welcome、onboard、rules、announcements 的初始內容與 repo 入口。Discord 的簡短介紹不取代 repo 自介 PR，不自動把進 server 的人認定為組織成員。
3. 啟用 Community，確認規則頻道與私有管理更新位置；依目標介面實際條件設定 Onboarding 與 Server Guide，提供歡迎文字、新人任務及資源入口。平台要求、條款或須使用者操作的步驟在實際遇到時處理，不預先聲稱可代為完成。
4. 整理 @everyone、公開 category 及唯讀頻道的權限；一般交流、論壇發文及建立自己的活動維持開放，管理全部活動與伺服器仍限管理者。建議關閉一般人的大量提及權限。需要新增管理角色時，只配置必要權限；具體授權人選須明確確認，不自行把其他人升為管理者。
5. 啟用基本 AutoMod 及安全通知；按 Community 的實際要求設定驗證與敏感媒體檢查，不改組織申請資格。尚未實測的規則不宣稱已有效。
6. 檢查邀請連結的進入位置、有效性與到期設定；確認新人可讀說明、發問、開論壇串及進語音，管理頻道確實隔離。若沒有第二個可用測試帳號，只回報已完成的角色預覽與實際檢查，不假冒完整新人測試。
7. 回報各項設定的實際結果與剩餘阻礙，取得實際可用的頻道／資源連結後更新相關規格與邀請流程；不把設定清單存在當成已完成。

目前仍在 Brainstorming，等待這份整體配置確認；本輪未新增、改名、移動、刪除頻道，未發布訊息或變更權限。
