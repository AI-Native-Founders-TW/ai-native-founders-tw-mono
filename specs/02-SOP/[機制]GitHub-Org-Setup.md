# Problem

自介審查通過後，需要讓本人取得 GitHub organization 的 Member 身分；審查人與執行邀請的人必須知道邀請誰、給哪些權限，以及何時才算完成。organization 角色、Team 與 repository 權限若混在一起，可能讓「加入組織」被誤解成取得所有 repo 的管理權，也可能把尚未接受邀請的人誤記為已加入。

# Specs

## Organization 與權限的區分

目標為 [AI-Native-Founders-TW](https://github.com/AI-Native-Founders-TW)。本規格記錄 GitHub org 加入方式與目前相關設定，作為[自介 PR 審查 SOP](./[機制]自介PR審查SOP.md)的接續依據；組織資格仍依[申請制度](../01-制度/[機制]申請制度.md)。

| 對象 | 意義與接合 |
|---|---|
| 組織成員 | 自介依申請制度審查通過後取得的資格。 |
| GitHub org Member | 接受該 org 的 Member 邀請後生效的平台身分；不因 PR comment 或合併而自動產生。 |
| GitHub org Owner | 平台管理角色，可執行 org 邀請；不因自介通過而授予 Owner。 |
| Members team | 既有 GitHub Team；與 org Member 是不同對象。加入此 Team 會取得其 repository 權限。 |
| Council team | 既有 Members 的子 Team；自介審查權依[自介審查制度](../01-制度/[機制]自介審查.md)授予，不擴張為其他治理權。 |
| R&R 的 Leader／Contributors | 依成員參與制度自行維護；不自動轉成 org Owner、Team maintainer 或 repo 管理權。 |

## 現行設定

以下為 2026-10-27 由 GitHub 設定頁讀取的現況；這次沒有修改平台設定。新通過者只邀請為 org Member，不加入 Members team；既有 Team 設定維持。

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

自介正式通過後，邀請該申請者成為 org **Member**。邀請執行者須具有 GitHub 平台所需的權限；這項平台能力不取代組織的審查裁決權。依[審查制度](../01-制度/[機制]自介審查.md)，先由有權限的人完成 PR 合併，再由 org Owner 發 Member 邀請；不選擇 Members、Council 或其他 Team，後續使用 Fork／PR。既有成員的 Team 與個別權限不由本流程改動。

| 實際狀態 | 處理與可回報的結果 |
|---|---|
| 尚未有正式通過結果 | 不因資料核對完成就邀請。 |
| 已通過，尚未發邀請 | 核對 PR 作者、自介 GitHub 帳號、正式審查紀錄及目前 org 狀態，確保邀請正確的人。 |
| 已是 org Member | 不重複邀請，回報已確認存在；不能藉此補推歷史自介已通過。 |
| 已有相同對象的 pending invitation | 先核對邀請的角色與狀態，不盲目重送；尚未接受不能寫成加入完成。 |
| 已送出邀請 | 回報邀請已送出，請本人接受；以 GitHub 實際狀態確認後續。 |
| 已接受並出現在 Members | 才能回報 GitHub org 加入完成。 |
| 邀請失效或操作失敗 | 保留已通過結果，如實記錄未完成原因；重試前重新核對對象與目前邀請，避免重複操作。 |

GitHub 的一般 org 邀請需本人接受，未接受的邀請七天後失效；平台要求的信箱驗證、雙因素驗證或可用席次可能影響接受與發送。這些是平台條件，不新增組織的背景或能力門檻。詳見 [GitHub 邀請說明](https://docs.github.com/en/organizations/managing-membership-in-your-organization/inviting-users-to-join-your-organization)。

邀請使用經核對的 GitHub username；不在公開 comment 放私人 email、邀請憑證或其他敏感資料。GitHub 自動發送的系統邀請與人工另寄 email 分開處理。

本規格採人工審查與平台操作，不啟用 bot、自動核准、自動合併或自動邀請。審查與操作中斷後依[自介 PR 審查 SOP](./[機制]自介PR審查SOP.md)接續；權限不足時交接給有權限的人，不自動提高權限。
