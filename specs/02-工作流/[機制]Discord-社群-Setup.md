# Problem

## Discord 加入、交流與活動

Discord 需要支援新人開始、創業交流、志工號召工作，以及線上與實體活動的發起及參與。參與者各有工作與生活，投入時間有限；組織需要讓這些行為容易發生，也需要讓重要資訊可以被找到。以下定義本次設計要滿足的需要，不表示目前 Discord 已完成設定或發生過特定問題。

### 新人理解組織並知道如何加入

收到邀請的人需要理解組織目的、知道如何加入，以及遇到問題時能在哪裡詢問。

1. Discord 身分與組織成員資格需要分清楚；具體資格及加入方式依[申請制度](../01-制度/[機制]申請制度.md)，交流工具不自行增加加入條件。
2. 新人需要找得到目的、加入說明與提問位置；重要內容不能只靠逐一私訊說明或翻找大量聊天。

### 創業者容易討論問題、分享經驗與認識彼此

創業者需要能提出具體問題、分享經驗並認識彼此，也需要在自己的時間能投入時接續討論。

1. 交流需要容納不同創業階段與背景，不將特定背景當作參與條件；開放原則依[憲法](../01-制度/constitution.md#第-17-條開放原則)。
2. 日常對話與值得深入、持續參考的內容都需要空間；重要內容不能一直被聊天洗掉。知識整理仍承接[志工協作與開源知識](./[機制]志工協作與開源知識.md#開源知識如何被使用)。
3. 主動參與不等於要求每天發言；具體參與安排依[成員參與制度](../01-制度/[機制]成員參與制度.md)。

### 志工容易號召工作並找到願意一起做的人

志工需要能讓其他人知道正在發起什麼工作、需要哪些幫忙，以及如何參與，讓願意一起做的人可以接續。

1. 參與者時間有限，需要容易理解工作內容與參與方式，不以持續盯著聊天作為協作前提。
2. 號召不能變成強制幫忙；能力與意願不等於已接受工作。認領及決策的關係依[協作工作流](./[機制]志工協作與開源知識.md#認領與拍板)與[憲法](../01-制度/constitution.md#第-16-條分工與決策)。

### 線上與實體活動容易發起及參與

參與者需要能發起線上或實體活動、號召有興趣的人，並讓有興趣的人容易找到活動及參與方式。

1. 辦活動與號召工作、日常討論是不同情境；討論容易，不代表活動的發起與參與就容易。
2. 活動資訊與接續討論需要能找到，避免參與者必須持續讀取日常聊天才能知道如何參與。
3. 讓活動容易發起不等於規定固定頻率或強制出席；尚未決定的頻率及參與標準仍依[成員參與制度](../01-制度/[機制]成員參與制度.md#尚未決定事項)。

# Specs

## Discord 社群的適用範圍

本文件集中維護上述新人加入、創業交流、志工號召工作及活動參與所需的 Discord 設定。頻道名稱全部使用英文。

Discord 身分與組織成員資格分開：申請及審查依[申請制度](../01-制度/[機制]申請制度.md)，具體參與安排依[成員參與制度](../01-制度/[機制]成員參與制度.md)。平台設定不另行增加組織加入條件，也不以進入 server 取代既有申請與審查。

## 設定狀態

已確認四種使用情境與頻道英文命名。整體頻道配置、角色與權限、新人引導及活動安排尚未確認；以下 Note 保存候選設計與現況，不是已採納的機制。Discord 尚未因本次工作新增、改名、移動或刪除頻道，亦未發布訊息或變更權限；文件整合不表示設定完成。

# Note

## 目標 server 現況（2026-10-26）

目標為 AI-Native Global Founders Speedrun Taiwan。以下是原生 Discord computer use 唯讀盤點的當時畫面，實際設定前須重新核對。

- 既有文字頻道：welcome、onboard、chit-chat、funding。
- 既有論壇：events、collaborations，已有討論串，應保留。
- 既有語音：General。
- onboard 畫面顯示頻道起始頁，沒有加入步驟；welcome 的首次訊息列表尚未顯示內容，未據此斷言永久空白。
- 設定頁顯示 Enable Community，Community 尚未啟用。既有兩個論壇仍可在側欄定位；不再用官方文件的 Community 必要條件推斷現有論壇不存在。
- Roles 頁只有預設權限入口，沒有顯示任何自訂角色。
- @everyone 的 Create Events 與 Mention @everyone, @here, and All Roles 為 on；Manage Events、Manage Channels、Manage Roles、Manage Server、Administrator 為 off。
- Safety Setup 顯示 Verification Level 為 None、Sensitive content filters 為 Do not filter，安全通知頻道未選定。未改動這些值。

## 參考 server 與平台條件

參考 server 已啟用 Community、Onboarding 與 Server Guide，使用公開公告、用途明確的論壇、新人任務及規則入口。這些可作為設計參考，不複製公司的私人權限結構到本組織。

參考 server 的實際 Default Channels 設定畫面列出十個預設頻道，並顯示 Must include 1 channel where @everyone can read and send messages。此畫面與前輪查到的官方 FAQ 七個預設、五個可發言的敘述不同。目標 server 的 Onboarding 尚不可從現況讀取；實作時須以目標介面的實際條件確認，不預建無用途的頻道湊數，也不宣稱已完成啟用。

## 頻道整體配置（尚未採納）

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

候選安排保留一般加入者建立自己活動的權限；不另設逐場核准或先審成員的門檻。活動權限尚未採納，不改變組織成員資格。

## 完整 setup 的交付範圍（尚未採納）

1. 依上表整理 categories 及 channels，保留既有訊息與論壇串；設定 topic、用途說明、論壇發文引導及必要標籤。
2. 完成 welcome、onboard、rules、announcements 的初始內容與 repo 入口。Discord 的簡短介紹不取代 repo 自介 PR，不自動把進 server 的人認定為組織成員。
3. 啟用 Community，確認規則頻道與私有管理更新位置；依目標介面實際條件設定 Onboarding 與 Server Guide，提供歡迎文字、新人任務及資源入口。平台要求、條款或須使用者操作的步驟在實際遇到時處理，不預先聲稱可代為完成。
4. 整理 @everyone、公開 category 及唯讀頻道的權限；一般交流、論壇發文及建立自己的活動維持開放，管理全部活動與伺服器仍限管理者。建議關閉一般人的大量提及權限。需要新增管理角色時，只配置必要權限；具體授權人選須明確確認，不自行把其他人升為管理者。
5. 啟用基本 AutoMod 及安全通知；按 Community 的實際要求設定驗證與敏感媒體檢查，不改組織申請資格。尚未實測的規則不宣稱已有效。
6. 檢查邀請連結的進入位置、有效性與到期設定；確認新人可讀說明、發問、開論壇串及進語音，管理頻道確實隔離。若沒有第二個可用測試帳號，只回報已完成的角色預覽與實際檢查，不假冒完整新人測試。
7. 回報各項設定的實際結果與剩餘阻礙，取得實際可用的頻道／資源連結後更新相關規格與邀請流程；不把設定清單存在當成已完成。

## 活動排程與參與（尚未採納）

原生 Events 用於活動排程與表達參與興趣；events 論壇保存詳情與討論，collaborations 論壇承接籌備工作的號召。線下活動使用 Somewhere Else 的實際地點，線上活動連到語音或實際會議位置。

若活動有名額、付費、審核或其他報名需求，需另行確認報名方式；Discord 的 Interested 不直接等於完成報名。活動尚未建立時，不預填真實日期、地點或出席承諾。活動仍須遵守[憲法](../01-制度/constitution.md)，容易發起活動不改變非營利及不得推銷、收費置入的規定。

## 配置取捨與待確認事項

全部放單一聊天室雖然建立快，但問題、號召工作及活動資訊較難持續找到；一開始按產業與地區建立很多頻道，又增加新人選擇與維護負擔。目前候選以文字頻道承接即時交流，以論壇承接需要持續接續的問題、工作與活動，並共用一個語音空間；暫無同時舉辦多場活動的依據，不增設多間語音。

不新增自介機器人、自動核准流程或產業／地區頻道。Community、Onboarding 與 Server Guide 的安排仍待整體確認及目標介面驗證，不為湊平台數量要求建立無用途頻道。管理者人選、管理角色的具體授權與活動權限仍待確認；尚未指定任何人取得管理權。

## 官方能力依據（2026-10-26 查核）

- [論壇需要 Community](https://support.discord.com/hc/en-us/articles/6208479917079-Forum-Channels-FAQ)。
- [Community 的必要設定](https://support.discord.com/hc/en-us/articles/360047132851-Enabling-Your-Community-Server)。
- [Scheduled Events 與建立／管理權限](https://support.discord.com/hc/en-us/articles/4409494125719-Scheduled-Events)。
- [角色與管理權限](https://support.discord.com/hc/en-us/articles/214836687-Discord-Roles-and-Permissions)。
- [AutoMod](https://support.discord.com/hc/en-us/articles/4421269296535-AutoMod-FAQ)。
- [Onboarding FAQ 所載七個預設頻道、其中五個可發言的條件；與實際參考畫面不同，目標條件仍待確認](https://support.discord.com/hc/en-us/articles/11074987197975-Community-Onboarding-FAQ)。
