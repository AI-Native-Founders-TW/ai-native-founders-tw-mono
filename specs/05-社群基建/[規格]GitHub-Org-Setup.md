# Problem

正式成員需要接續取得 GitHub organization 的 Member 身分；審查人與執行邀請的人必須知道邀請誰、給哪些權限，以及何時才算完成。organization 角色、Team 與 repository 權限若混在一起，可能讓「加入組織」被誤解成取得所有 repo 的管理權，也可能把尚未接受邀請的人誤記為已加入。

# Specs

## Organization 與權限的區分

目標為 [AI-Native-Founders-TW](https://github.com/AI-Native-Founders-TW)。本規格記錄 GitHub org 加入方式與目前相關設定，作為[自介 PR 審查 SOP](<../03-SOP/[SOP]自介PR審查SOP.md>)的接續依據；組織資格仍依[申請制度](<../01-制度/[機制] 憲政制度.md>)。

| 對象 | 意義與接合 |
|---|---|
| 組織成員 | 依憲政制度有效取得的資格；一般申請、首屆任命及恢復的依據分開保存。 |
| GitHub org Member | 接受該 org 的 Member 邀請後生效的平台身分；不因 PR comment 或合併而自動產生。 |
| GitHub org Owner | 平台管理角色，可執行 org 邀請；不因自介通過而授予 Owner。 |
| Members team | 既有 GitHub Team；與 org Member 是不同對象。加入此 Team 會取得其 repository 權限。 |
| Council team | 既有 Members 的子 Team；平台名稱與實際權限須分開核對，不以此 Team 名單自行決定治理或審查資格。 |
| R&R 的 Leader／Contributors | 依憲政制度與 R&R 權限配置維護；Leader 具有 Council 身分，但不自動取得 org Owner、Team maintainer 或所有 repo 管理權。 |

## 維護與權限交接

[Repository Leader](<../02-R&R/[Role]基建-Repository維護.md>)承接 GitHub 技術設定與有效決定的執行；第二位接續 Leader 必須在自己的有效 R&R 中明列 GitHub 接續範圍與權限。職位本身不表示帳號已有平台權限，Org Owner 或 Team 名稱也不取代有效任職。

操作前核對共同制度的決定與生效時間，依 Repository 的權限接續步驟執行並回讀實際設定。撤任只收回已失去職責所需權限，保留其他有效職位與一般權益；不得因普通成員仍能公開讀取 repo 而宣稱撤權失敗，也不得把 org Member 當成治理票權。權限交接、緊急處置及能力不足的處理依[憲政制度](<../01-制度/[機制] 憲政制度.md>)。

## 現行設定

以下為 2026-10-27 由 GitHub 設定頁讀取的現況；這次沒有修改平台設定。此表是該日觀察，不能作為永久保留既有權限的依據。一般成員平台加入只邀請為 org Member，不加入 Members team；後續有效任免、撤權或設定變更仍依憲政制度執行。

| 設定位置 | 現行值 | 作用 |
|---|---|---|
| Org 顯示名稱 | AI-Native Founders Summit Taiwan | GitHub 平台顯示名稱；本文件不以此改寫憲法中的組織名稱。 |
| Org Base permissions | No permission | 不透過 org 基礎權限授予 repo 存取；public repo 的公開讀取不因此消失。 |
| Repository creation | Public 開啟；Private 關閉 | org Member 可建立 public repo，不能以此設定建立 private repo。 |
| Members team | mono repo：Write | Team 對指定 repo 的權限，不能由 Base permissions 的 No permission 推定沒有 Write。 |
| Council team | Members 的子 Team | 保留現行結構，不由名稱推定額外治理權或所有 repo 的 Admin。 |
| Projects base permissions | Write | 與 repository Base permissions 是不同設定。 |
| Pages creation | Public 開啟 | 允許公開 Pages；private 選項在頁面不可用。 |
| Team creation | 開啟 | org Member 可建立 Teams。 |
| 私有 repo fork | 關閉 | 不開放 private repo fork。 |
| Repository discussions | 允許 Read 使用者建立 | 在啟用 Discussions 的 repo，Read 使用者可建立及回覆討論。 |
| App access requests | Members and outside collaborators | 允許提出 app 使用申請，不表示 app 已獲安裝授權。 |
| Repo 管理員安裝 GitHub Apps | 開啟 | 依平台欄位限制，僅限不要求 org／repo administration permissions 的 App。 |
| Issue 刪除 | 不允許 repo 管理員執行 | org Owner 管理該項操作。 |
| 受 org rules 保護的分支更名 | 允許 repo 管理員執行 | 仍受 GitHub 頁面所示 rules 覆蓋或 bypass 條件限制，不表示所有規則可繞過。 |
| Repo 可見性變更 | 不允許一般 repo 管理員變更 | org Owner 管理該項變更。 |
| Repo 刪除／轉移 | 不允許一般 repo 管理員執行 | org Owner 管理該項操作。 |

設定來源：[Member privileges](https://github.com/organizations/AI-Native-Founders-TW/settings/member_privileges)、[Members team 的 repository 權限](https://github.com/orgs/AI-Native-Founders-TW/teams/members/repositories)、[Members 的子 Teams](https://github.com/orgs/AI-Native-Founders-TW/teams/members/teams)。登入管理者才能看見的設定不以公開首頁推定。

## 審查通過後的 GitHub org 加入

自介正式通過後，邀請該申請者成為 org **Member**。邀請執行者須具有 GitHub 平台所需的權限；這項平台能力不取代組織的審查裁決權。依[審查制度](<../01-制度/[機制] 憲政制度.md>)，先由有權限的人完成 PR 合併，再由 org Owner 發 Member 邀請；不選擇 Members、Council 或其他 Team，後續使用 Fork／PR。此一般加入流程不自行增減其他職責的 Team 與個別權限；另有有效權限變更決定時，依其範圍另外執行，不能以本流程為由拒絕撤權。

首屆任命及恢復資格的成員不需偽造一般審查或重做入會。平台接續由 Onboard 核對有效資格依據、本人帳號及生效時間，交 Repository 的合格操作人執行相同 Member 邀請程序：

| 資格來源 | 邀請前核對 | 紀錄位置 |
|---|---|---|
| 一般自介審查 | 正式通過結果與已合併 PR；一般新申請以 PR 合併時取得資格，合併前僅審查通過尚未生效。修訂前已有效成立的資格依憲政制度過渡規則保留，平台加入仍依本流程接續 | 原自介 PR |
| 首屆有效任命 | 公布的任命文件、本人接受、自介及 Contributors 等成立條件、共同生效時間、已核對 GitHub 帳號；不要求另外一份一般審查通過 PR | 首屆任命紀錄及相關 PR／Issue |
| 有效恢復 | 原有效資格與退出依據、原已驗證帳號、完整恢復聲明及有效 Contributors 選擇；不要求重寫自介或等待名冊合併才邀請 | 恢復案件與相關 PR／Issue |

三種來源均先確認目前 Members／Invitations；已存在不重送，缺少 Member 時才邀請，不選 Team，發送後與接受後分別記錄。首屆與恢復的歡迎訊息應如實說明資格來源，不套用「自介已審查通過並合併」的文字。資料不足時記錄待核對的具體依據，不把平台加入完成當成補足資格。

| 實際狀態 | 處理與可回報的結果 |
|---|---|
| 尚未有有效資格依據 | 不因資料初步核對或平台已有帳號就邀請。 |
| 資格已生效，尚未發邀請 | 依上表核對對應資格來源、本人 GitHub 帳號及目前 org 狀態，確保邀請正確的人。 |
| 已是 org Member | 不重複邀請，回報已確認存在；不能藉此補推歷史自介已通過。 |
| 已有相同對象的 pending invitation | 先核對邀請的角色與狀態，不盲目重送；尚未接受不能寫成加入完成。 |
| 已送出邀請 | 回報邀請已送出，請本人接受；以 GitHub 實際狀態確認後續。 |
| 已接受並出現在 Members | 才能回報 GitHub org 加入完成。 |
| 邀請失效或操作失敗 | 保留有效資格結果，如實記錄未完成原因；重試前重新核對對象與目前邀請，避免重複操作。 |

GitHub 的一般 org 邀請需本人接受，未接受的邀請七天後失效；平台要求的信箱驗證、雙因素驗證或可用席次可能影響接受與發送。這些是平台條件，不新增組織的背景或能力門檻。詳見 [GitHub 邀請說明](https://docs.github.com/en/organizations/managing-membership-in-your-organization/inviting-users-to-join-your-organization)。

邀請使用經核對的 GitHub username；不在公開 comment 放私人 email、邀請憑證或其他敏感資料。GitHub 自動發送的系統邀請與人工另寄 email 分開處理。

本規格採人工審查與平台操作，不啟用 bot、自動核准、自動合併或自動邀請。審查與操作中斷後依[自介 PR 審查 SOP](<../03-SOP/[SOP]自介PR審查SOP.md>)接續；權限不足時交接給有權限的人，不自動提高權限。
