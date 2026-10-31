# Problem

## Discord 加入、交流與活動

Discord 需要支援新人開始、創業交流、志工號召工作，以及線上與實體活動的發起及參與。參與者各有工作與生活，投入時間有限；組織需要讓這些行為容易發生，也需要讓重要資訊可以被找到。

### 新人理解組織並知道如何加入

收到邀請的人需要理解組織目的、知道如何加入，以及遇到問題時能在哪裡詢問。

1. Discord 身分與組織成員資格需要分清楚；具體資格及加入方式依[申請制度](<../01-制度/[機制] 憲政制度.md>)，交流工具不自行增加加入條件。
2. 新人需要找得到目的、加入說明與提問位置；重要內容不能只靠逐一私訊說明或翻找大量聊天。

### 創業者容易討論問題、分享經驗與認識彼此

創業者需要能提出具體問題、分享經驗並認識彼此，也需要在自己的時間能投入時接續討論。

1. 交流需要容納不同創業階段與背景，不將特定背景當作參與條件；開放原則依[憲法第 4 條（開放成員資格）](<../01-制度/憲法.md#第-4-條開放與成員資格>)。
2. 日常對話與值得深入、持續參考的內容都需要空間；重要內容不能一直被聊天洗掉。知識整理仍承接[志工協作與開源知識](<../03-SOP/[SOP]志工協作與開源知識.md#開源知識如何被使用>)。
3. 主動參與不等於要求每天發言；具體參與安排依[成員參與制度](<../01-制度/[機制] 憲政制度.md>)。

### 志工容易號召工作並找到願意一起做的人

志工需要能讓其他人知道正在發起什麼工作、需要哪些幫忙，以及如何參與，讓願意一起做的人可以接續。

1. 參與者時間有限，需要容易理解工作內容與參與方式，不以持續盯著聊天作為協作前提。
2. 號召不能變成強制幫忙；能力與意願不等於已接受工作。認領及決策的關係依[協作工作流](<../03-SOP/[SOP]志工協作與開源知識.md#認領與拍板>)與[憲法第 5 條（自願貢獻參與）](<../01-制度/憲法.md#第-5-條自願貢獻與參與義務>)及[第 7 條（決策範圍任命）](<../01-制度/憲法.md#第-7-條決策範圍與任命>)。

### 線上與實體活動容易發起及參與

參與者需要能發起線上或實體活動、號召有興趣的人，並讓有興趣的人容易找到活動及參與方式。

1. 辦活動與號召工作、日常討論是不同情境；討論容易，不代表活動的發起與參與就容易。
2. 活動資訊與接續討論需要能找到，避免參與者必須持續讀取日常聊天才能知道如何參與。
3. 讓活動容易發起不等於規定固定頻率或強制出席；尚未決定的頻率及參與標準仍依[成員參與制度](<../01-制度/[機制] 憲政制度.md#長期不參與與成員資格處理>)。

# Specs

## Discord 社群的適用範圍

本機制以頻道分工、權限與新人導覽，支援上方 [Discord 加入、交流與活動](#discord-加入交流與活動)的四種情境。Server Guide 帶新人找到加入方式、協作與活動；實際申請由 repo 的制度承接。

目標 server 為 [AI-Native Global Founders Speedrun Taiwan](https://discord.com/channels/1563453138810306612/1563453141641597000)。頻道與 category 名稱均使用英文，描述及新人說明使用繁體中文；既有訊息與論壇討論串保留。

Discord 身分與組織成員資格分開。申請與審查依[申請制度](<../01-制度/[機制] 憲政制度.md>)，自介放在公開 repo 的 [members](<../../members/README.md>) 資料夾，以 PR 提交；具體參與安排依[成員參與制度](<../01-制度/[機制] 憲政制度.md>)。進入 server、新人導覽與活動權限不另設組織加入條件。

## 頻道整體配置

分類與頻道依下表排列。Text 是文字頻道、Forum 是論壇、Voice 是語音；括號說明可見及發文限制。

| Category | Channel | Type | 描述 |
|---|---|---|---|
| start-here | [welcome](https://discord.com/channels/1563453138810306612/1563453141641597000) | Text（唯讀） | 歡迎加入 AI-Native Global Founders Speedrun Taiwan！我們共享創業知識、交流經驗並一起做事。新人請先看 #onboard 與 #rules，有問題到 #chit-chat 詢問。 |
| start-here | [onboard](https://discord.com/channels/1563453138810306612/1563456791050977341) | Text（唯讀） | 從這裡開始：閱讀組織願景、憲法與申請制度，再於公開 repo 的 members 資料夾以 PR 提交自介。自介審查通過並合併 PR 後成為組織成員；進入 Discord 不等於已入會。Repo：https://github.com/AI-Native-Founders-TW/ai-native-founders-tw-mono |
| start-here | [rules](https://discord.com/channels/1563453138810306612/1564249902475907172) | Text（唯讀） | 交流請遵守組織憲法與現行制度：開放學習、尊重彼此、自願貢獻；不得以本組織名義、筆記或活動為特定公司推銷產品、服務或提供收費置入。規範以 repo 為準：https://github.com/AI-Native-Founders-TW/ai-native-founders-tw-mono |
| start-here | [announcements](https://discord.com/channels/1563453138810306612/1564249954266914846) | Text（唯讀） | 重要公告、組織更新與已確認活動，由具有效公告職責與平台能力的人發布。日常討論請到 #chit-chat；活動詳情與接續討論請到 #events。 |
| community | [chit-chat](https://discord.com/channels/1563453138810306612/1563454007605723186) | Text | 打招呼、閒聊、即時問答與新人求助。想深入討論創業問題或分享經驗，請到 #discussions 開一篇，讓大家能在自己的時間接續。 |
| community | [funding](https://discord.com/channels/1563453138810306612/1564236090770984970) | Text | 交流募資問題、經驗與資源。請交代創業階段、具體問題與需要的幫忙；仍須遵守不得以組織名義推銷產品、服務或提供收費置入的規定。 |
| community | [discussions](https://discord.com/channels/1563453138810306612/1564250031706607657) | Forum | 一個創業問題或一份經驗分享開一篇。請說明背景、具體問題、已嘗試的方法與希望得到的幫忙；相關討論留在同篇，長期有用的知識再整理到 repo。 |
| get-involved | [collaborations](https://discord.com/channels/1563453138810306612/1563454194541658122) | Forum | 號召志工與協作，一件工作或活動籌備開一篇。請說明要做什麼、需要哪些幫忙、如何參與，以及由誰負責決策；參與自願，認領不代表必須獨自完成。 |
| get-involved | [events](https://discord.com/channels/1563453138810306612/1563454084168814612) | Forum | 一場線上或實體活動開一篇，說明目的、時間、地點或會議連結及參與方式；活動討論留在同篇。所有加入者都可建立自己的 Events 排程；Interested 表示興趣，不取代另有要求的報名程序。 |
| voice | [lounge](https://discord.com/channels/1563453138810306612/1563453141641597001) | Voice | 即時交流、Coffee Chat、工作討論與小型線上活動共用語音空間。活動目的、時間與參與方式請放 #events，工作號召請放 #collaborations。 |
| management | [mod-log](https://discord.com/channels/1563453138810306612/1564250087775932556) | Text（私有） | 私有管理紀錄：接收 Community 更新與 AutoMod 警示，僅供具有必要管理職責與平台能力的人查看；不在此新增組織決策權或管理授權。 |

文字頻道的描述填入 Channel Topic，論壇填入 Post Guidelines。lounge 的設定頁沒有描述欄位，使用語音頻道的[文字聊天用途說明](https://discord.com/channels/1563453138810306612/1563453141641597001/1564251491944898581)。announcements 使用一般 Text；原生 Events 是活動排程功能，不是額外頻道。

<a id="管理與公告發布"></a>

## 維護責任與制度接合

[Repository Leader](<../02-R&R/[Role]基建-Repository維護.md>)承接 Discord 技術設定、權限與事故處理。第二位接續 Leader 須在自己的有效 R&R 明列 Discord 接續範圍與必要權限；Council 身分不代表取得 Administrator，伺服器 Role 也不代表有效任命。

變更依有效決定核對分類、頻道與帳號，操作後回讀確認，保留不含秘密的證據。任免交接、備援、緊急限制與非本人覆核依[憲政制度](<../01-制度/[機制] 憲政制度.md>)，具體操作接續依 Repository 職責文件。不得以封鎖平台存取代替永久取消組織成員資格；制度有效變更與平台實際完成分開記錄。

## 公開、唯讀與管理權限

權限分成 server 的 @everyone 預設權限、分類限制及頻道覆寫。@everyone 提供一般交流能力，start-here 再限制入口頻道發文，management 再限制管理紀錄可見性。

| 設定位置 | 權限 | 設定值與作用 |
|---|---|---|
| @everyone | View Channels、Read Message History、Send Messages and Create Posts | 開啟，提供公開交流與讀取歷史的基礎權限。 |
| @everyone | Connect、Speak | 開啟，允許進入 lounge 與發言。 |
| @everyone | Create Events | 開啟，允許建立自己的活動。 |
| @everyone | Manage Events、Manage Server、Manage Roles、Manage Channels、Administrator | 關閉，不因加入 server 取得管理權。 |
| @everyone | Mention @everyone, @here, and All Roles | 關閉。 |
| start-here | Send Messages and Create Posts、Send Messages in Threads and Posts、Create Public Threads、Create Private Threads | 對 @everyone 設 Deny。 |
| welcome | 發訊息、討論串發文、建立公開與私人討論串 | 頻道本身也對 @everyone 設 Deny。 |
| onboard、rules、announcements | 分類權限 | 與 start-here 同步。 |
| management | View Channel | 對 @everyone 設 Deny。 |
| mod-log | 分類權限 | 與 management 同步，保持私有。 |

公開交流頻道允許一般加入者查看、發文、回覆及讀取歷史，lounge 允許進入與發言。start-here 的四個入口頻道不允許一般加入者發訊息、在討論串發文或建立公開、私人討論串；公告由具有效職責與平台能力的人發布，依 Repository 的技術維護安排接續。

management 與 mod-log 對 @everyone 拒絕 View Channel。管理者、角色及公告發布能力依憲政制度與有效 R&R 配置核對及交接，既有平台權限不構成永久職權；不將管理伺服器、管理角色、管理頻道、管理全部活動或 Administrator 開給一般加入者。一般加入者不能使用 @everyone、@here 或大量角色提及。

<a id="活動建立與管理權限"></a>

## 活動建立與參與

每場活動從籌備、公告、舉辦到同篇 forum 的會後摘要，依[活動籌備、舉辦與會後整理 SOP](<../03-SOP/[SOP]活動籌備、舉辦與會後整理.md>)接續；本節維護平台能力與頻道分工，不另訂第二套辦理流程。

所有 server 加入者均可建立自己的原生 Events 活動排程；不以組織成員資格或管理者身分作為條件。管理全部活動仍限具有效職責及對應平台能力的人，不增加出席或辦活動義務。

活動詳情與討論放 events，籌備工作號召放 collaborations。每場活動說明目的、時間、地點或會議連結及參與方式；若另有名額、審核或報名要求，須在該活動說清楚，Interested 不等於完成另行要求的報名。尚未發起的活動不填入虛構日期、地點或出席承諾。活動遵守[憲法](<../01-制度/憲法.md>)。

<a id="community-與安全設定"></a>

## Community、通知與安全設定

Community 及安全設定保護公開交流；平台驗證不取代組織申請與審查。

| 設定 | 採用值 |
|---|---|
| Community | 啟用。 |
| Rules or Guidelines Channel | rules。 |
| Community Updates Channel | mod-log。 |
| Safety Notifications Channel | mod-log。 |
| 發訊息驗證 | 要求已驗證信箱。 |
| 敏感媒體檢查 | 所有成員。 |
| Default Notification Settings | Only @mentions。 |
| System Messages Channel | chit-chat。 |
| 自動歡迎、歡迎貼圖提示、Boost 通知、server setup 提示 | 開啟，均使用系統訊息頻道。 |

AutoMod 採用下表設定；這些規則不自動禁言。

| 規則 | 狀態 | 阻擋條件／範圍 | 動作 | 警示目的地 |
|---|---|---|---|---|
| Block Mention Spam | 啟用 | 每則訊息最多提及二十個不同對象。 | Block message、Send alert。 | mod-log。 |
| Block Suspected Spam Content | 啟用 | 平台判定的可疑垃圾內容；此規則僅支援英文。 | Block message、Send alert。 | mod-log。 |

## 新人引導與 Next 接續

### Onboarding 的入口與預設頻道

Onboarding 與 Server Guide 均啟用，使用預設模式，不設定加入前或加入後的角色問卷。加入者不必先回答問卷才能找到公開頻道，也不會透過問卷自動取得組織成員資格。

| 設定 | 採用值 |
|---|---|
| Default Channels：文字與論壇 | welcome、onboard、rules、announcements、chit-chat、funding、discussions、collaborations、events，共九個。 |
| 語音入口 | lounge。 |
| 私有頻道 | mod-log 不列入新人預設入口。 |
| Resource Pages | 不設定；入口頻道保留在頻道列表。 |
| Server Guide 自訂 Banner、任務自訂縮圖 | 不設定。 |

### 歡迎訊息

Server Guide 的 Welcome Sign 由 waterball.pan 顯示，使用下列文字；[@username] 是平台代入新人名稱的位置：

> 歡迎 [@username]！這裡是 AI-Native Global Founders Speedrun Taiwan。我們共享創業知識、交流經驗、號召志工一起做事，也一起發起線上與實體活動。先閱讀 welcome、onboard 與 rules；有問題到 chit-chat 詢問。想加入組織，請依 repo 的申請制度以 PR 提交自介，審查通過並合併 PR 後成為成員。下方是入門導覽，不是額外入會門檻。

### New Member To Do 與完成條件

三個自訂任務依下表排列。每項都使用 **Member visits the channel** 作為完成條件；不採用傳送訊息或在論壇發文、回覆作為完成條件。

| 順序 | 任務文字 | 目的頻道 | 完成條件 | 依序瀏覽時的接續 |
|---|---|---|---|---|
| 第一項 | 閱讀加入方式與自介 PR 說明 | onboard | 進入 onboard。 | Next：看看正在號召的協作工作，導向 collaborations。 |
| 第二項 | 看看正在號召的協作工作 | collaborations | 進入 collaborations。 | Next：看看線上與實體活動及參與方式，導向 events。 |
| 第三項 | 看看線上與實體活動及參與方式 | events | 進入 events。 | 自訂任務至此結束，沒有第四個自訂任務。 |

Read the rules 是平台另提供的規則入口，對應 Community 的 rules 頻道，不是第四個自訂任務。Next 是 Discord 原生新人導覽按鈕，不是發在頻道中的訊息或自建 bot。

依序瀏覽的路徑為：Server Guide → onboard → Next → collaborations → Next → events。導覽任務可以從 Server Guide 直接選取，並不把前一個任務完成當成開放下一個公開頻道的權限門檻。

導覽完成只代表到過對應頻道，不代表已讀完文字、提出自介 PR、通過審查、認領工作或報名活動。這些行為依各自制度與活動說明辦理；導覽也不強制發言或出席。

### onboard SOP 與頻道說明的接合

onboard 以[釘選 SOP](https://discord.com/channels/1563453138810306612/1563456791050977341/1564254596208271400)承接第一項導覽。訊息依序帶新人閱讀組織說明、寫自介與 Contributions、在獨立 assignment 表自行選擇至少一個 R&R 當 Contributors ，資格依申請 PR 與後續有效紀錄核對、記得自行 Review 全文、提交自介 PR、等待審查並依意見補充。自介欄位與 GitHub 提交操作依 [members 的自介與 PR 說明](<../../members/README.md>)，資格判定依[申請制度](<../01-制度/[機制] 憲政制度.md>)，不在 Discord 建立第二套規則。

| 頻道 | 固定說明與接續 |
|---|---|
| welcome | 組織介紹、onboard 與 rules 入口，以及交流、募資、協作、活動、語音與公告的導覽。 |
| onboard | 釘選上述 SOP；操作有疑問到 chit-chat。 |
| rules | 現行交流規範與 repo 的憲法、制度入口。 |
| announcements | 由具有效公告職責與平台能力的人發布重要公告與已確認活動。 |
| lounge | 用語音頻道文字聊天的用途說明承接即時交流，活動詳情回 events、工作號召回 collaborations。 |

welcome 保留組織與頻道導覽；自動加入與其他系統訊息使用前述 chit-chat 設定。

## 邀請與伺服器介紹

| 設定 | 採用值 |
|---|---|
| 現行邀請 | https://discord.gg/xeWYqYaUvU |
| 邀請所屬頻道 | collaborations。 |
| 到期 | 不到期。 |
| Server Description | 共享創業知識、交流經驗與認識彼此，讓志工容易一起做事，也讓線上與實體活動容易發起及參與。 |
| Private Profile | 開啟。 |

邀請所屬頻道與 Server Guide 的導覽任務是不同設定；不將邀請指向 collaborations 解讀成略過 onboard SOP 或完成組織申請。
