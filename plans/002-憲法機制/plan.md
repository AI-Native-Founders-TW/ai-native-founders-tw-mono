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
- 「只要有正向意圖、是個良好的公民」算不算門檻、要不要有人判斷：「不是門檻，申請就能加入」——「正向意圖、良好的公民」是對每個人的期待，不是門檻，沒有人審核。……

2026-10-24 對本 Plan 的關鍵決策：

> 看一下 plan 002 另一個 agent 起草了憲法部分，你把關鍵決策寫進去 plan

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

條文從 Vision、創辦人的話與需求原文取出，逐字沿用；第 2 條的「這句不算商業意圖，目的本身可以容忍。」與第 6 條的第二段，是 AI 用創辦人的話與需求原文裡的字整理成的句子，不是逐字。順序：先寫 `specs/constitution.md`，再在 AGENTS.md 加「憲法」一節、在 plans 的章節表加「憲法檢查」，最後以 subagent 檢查整個 repo。

### 規格差異

1. 新增 [憲法](../../specs/constitution.md)：第 1 條到第 8 條與治理。第 2 條（value proposition）與第 3 條（其他的商業意圖怎麼區分）對應 [其他的商業意圖怎麼區分](#其他的商業意圖怎麼區分)；其餘對應 [是否有違反憲法中的每一條規則](#是否有違反憲法中的每一條規則)。

## 驗收

- [x] 1. 定位在 `specs/constitution.md`。動作是逐條對回出處。
    - 預期：每一條的規則都找得到出處；除了工程戰略註明的兩句，都是出處的原句；沒有出處裡沒有的詞。

## 關鍵決策

創辦人做的決策，以及寫進哪裡。原話見各 Plan 的需求原文。

- 2026-10-21：大家共同編輯協作，不用有拍板。寫進[第 5 條（大家共同編輯協作）](../../specs/constitution.md#第-5-條大家共同編輯協作)。
- 2026-10-23：憲法 specs/constitution 機制。AGENTS.md 強調憲法約束：AI 在產出完之後，尤其是 Deliver／Push 之前，必須以 subagent 以極度嚴格的角度去檢查是否有違反憲法中的每一條規則。寫進[憲法](../../specs/constitution.md)與 [AGENTS.md 的「憲法」](../../AGENTS.md#憲法)。
- 2026-10-23：「你可以參考 SpecKit」。參考了哪些、哪些不採用，是 AI 的決定，見[工程戰略](#工程戰略)。
- 2026-10-23：「如果這個組織能夠幫助我自己，還有我很棒的團隊做出能出海的 Business 的話，那一定也能幫助其他的台灣人。」這句不算商業意圖：「NPO 本來就要有 value proposition」，「value proposition 要定義清楚在憲法中，目的本身可以容忍」。寫進[第 2 條（value proposition）](../../specs/constitution.md#第-2-條value-proposition)。
- 2026-10-23：「只要有正向意圖、是個良好的公民」算不算門檻，他選 AI 擬的選項「不是門檻，申請就能加入」。寫進[第 6 條（不會限制任何門檻）](../../specs/constitution.md#第-6-條唯一的門檻是自介)。
- 2026-10-23：對建立憲法的過程，「另外上述迭代過程別紀錄，不想在 kickoff 時有這麼多複雜的脈絡」。
- 2026-10-24：其他的商業意圖怎麼區分，需求原文裡 AI 擬的四項，他全選。寫進[第 3 條（其他的商業意圖怎麼區分）](../../specs/constitution.md#第-3-條其他的商業意圖怎麼區分)。

其餘是 AI 的決定，不是創辦人的決策：從 Vision 與創辦人的話挑哪些句子當條文；治理的寫法，包含創辦人的話和憲法衝突時由創辦人自己改，以及建立憲法的 Plan 只留最後的版本；AGENTS.md 的檢查細節，例如「拿不準的算違反」。

## GitHub Organization 協作脈絡（2026-10-24，待釐清）

本節保存本次討論與外部能力查證，不是已採納的組織規則。使用者要把這些脈絡寫進「那個 project 中的 plan」（見本節需求原文最後一段），放進本 Plan 是 AI 的判斷；使用者沒有確認整體權限提案，也沒有要求修改憲法或實際設定 GitHub。現行承諾仍以 [憲法](../../specs/constitution.md) 為準；本次沒有 specs truth 變更。

### 本次需求原文

> 那如果我要做一個去中心化 NPO，在 github repo 上協作，權限部分我該怎麼描述核心的那一群有一些特別權限的人呢

> Council 給我中文定義 for this NPO

> 如果在 github org 上
> 我想讓一群人發 PR 審核通過之後當 member
> 然後有核心一小群人有特別的權限
> 這樣的 structure 怎麼善用 github org permissions/policy or teams 設計？

> 如果大家都可以開自己的 repository，我要怎麼讓所有 member 都可以開 repository？

> 那 team 呢？是兩個 teams?

> 把這些脈絡也寫進去 /sf-ai ai-native taiwan 那個 project 中的 plan

### Council 與 Stewards 的命名脈絡

討論從瑞士的 Federal Council（聯邦委員會）延伸到 NPO 的共同治理。Council 強調一群人共同議事、提供建議或作出決策；Stewards 強調受託照顧組織使命、資源與長期發展。兩個詞本身都不決定權限大小，也不保證去中心化。

使用者接著要求 Council 的中文定義，AI 提供的草稿為：

> Council（核心委員會）：在本 NPO 中，由共同承擔組織治理責任的成員組成，依公開規則共同討論與決策，並在明確界定的範圍內行使特別權限。

這是命名與定義草稿，並未授予任何人決策權；是否採用、特別權限涵蓋什麼，仍須與現行憲法一起釐清。

### GitHub 可用能力與討論中的對應

| 對象 | GitHub 對應 | 本次討論 |
|---|---|---|
| 申請者 | 尚未是 Organization Member | 公開 repo 可以接受 fork 後提交的 PR；審核後入會是本次提出的想法，與現行憲法衝突，尚不可執行 |
| 一般成員 | Organization Member | 使用者希望所有 Member 都能建立 repository；可由組織的 Member privileges 設定允許，不必升為 Owner |
| Members（一般成員）Team | 自訂 Team | 可包含全部成員，也包含 Council 成員，用於共同 repo 權限與團隊提及；沒有這些需求時可不建立 |
| Council（核心委員會）Team | 自訂 Team，成員仍可保持 Organization Member | 用於分配特別權限的候選設計；不等於 Organization Owner，也尚未決定有哪些特別權限 |
| Organization Owner | GitHub 組織管理角色 | 管理組織設定與邀請；Council 不必全部擔任 Owner。人選與人數未決定 |

兩個 Teams 的候選安排為平行建立，Council 成員同時加入 Members（一般成員）與 Council（核心委員會）；這不是必需兩個 Teams，也不是由 Team 決定誰能建立 repository。

所有 Member 建立 repository 的設定位置：Organization → Settings → Access → Member privileges → Repository creation，選擇允許的 Public／Private 類型並儲存。建立時 Owner 選 Organization，repo 歸組織所有；Owner 選個人帳號，才歸個人所有。允許的可見性類型尚未選定。

Base permissions 與建立 repository 的權限是兩件事；前者可以維持 None，再由 Teams 授予需要的 repo 存取權，不必為了開 repo 而給所有成員全組織 repo 的 Write。這是 AI 的設定建議。

### PR、邀請與審核的候選安排

AI 曾提出「申請 PR → Council 審核 → 合併 → 發出 Organization 邀請 → 接受邀請 → Member／加入 Team」的候選流程。PR 核准或合併本身不會自動建立 GitHub 成員身分，仍需要邀請與接受邀請；可以人工操作，也可以另外建 GitHub App 自動化，兩者尚未選定。

AI 曾建議治理 repo 的 Council Team 取得 Write、配合 CODEOWNERS（審核負責設定）與 Rulesets 要求 PR、兩個有效 Approvals、Code Owner 核准、修改後重新審核，以及禁止 force push／刪除主要分支。以上都是候選，尤其「兩個 Approvals」是 AI 舉的數字，也不保證是兩位 Council；一般 Code Owner 條件只要求符合條件的其中一位核准。若要精確驗證 Council 核准人數，需要依實際權限配置另行設計。

Code Owner 的 Team 必須可見且具有該 repo 的 Write 權限。公開 repo 可使用 GitHub Free 的 Rulesets；Organization 私有 repo 使用相關保護需依 GitHub Team／Enterprise Cloud 的方案能力。Organization Owner 仍具有修改組織設定與權限的能力，Teams 與 PR 規則不能單獨保證 Owner 的操作也經多人同意。

### 與現行憲法的衝突及未決範圍

- [第 6 條（不會限制任何門檻）](../../specs/constitution.md#第-6-條唯一的門檻是自介)明定「沒有人審核；申請就能加入」。本次「PR 審核通過之後當 member」若成為入會前提，會與此條衝突。本節只保存這個想法，不把它設為生效流程，也不自行把「加入團體」與「GitHub Member」重新解讀成不同資格來放行。
- [第 5 條（大家共同編輯協作）](../../specs/constitution.md#第-5-條大家共同編輯協作)明定「大家共同編輯協作，不用有拍板」。Council 是否取得內容核准、合併或否決權，須先釐清；不能因 Team 名稱已提出，就把共同編輯改成必須經 Council 拍板。
- 尚未決定：Council 名稱與定義是否採用、特別權限範圍、成員產生與撤換方式、是否實際需要兩個 Teams、repo 可見性、PR 審核條件、Owner 人選、邀請是否自動化。
- 若後續要修改憲法，依現行「治理」的修改憲法規則處理。本輪只保存脈絡，不改憲法、既有 To-Be 或已採納的規格差異，不標記整體提案已確認、已就緒或已 Deliver。

### 外部能力來源

以下於 2026-10-24 查閱；說明 GitHub 能力，不代表已選定此組織政策或已完成設定。

- [Organization roles](https://docs.github.com/en/organizations/managing-peoples-access-to-your-organization-with-roles/roles-in-an-organization)
- [Repository roles](https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/repository-roles-for-an-organization)
- [Repository creation](https://docs.github.com/en/organizations/managing-organization-settings/restricting-repository-creation-in-your-organization)
- [Base permissions](https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/setting-base-permissions-for-an-organization)
- [Organization invitation API](https://docs.github.com/en/rest/orgs/members#create-an-organization-invitation)
- [CODEOWNERS（審核負責設定）](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-code-owners)
- [Rulesets 支援範圍](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-rulesets/about-rulesets)
- [Rulesets 審核條件](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-rulesets/available-rules-for-rulesets)

## 憲法檢查

範圍：`specs/constitution.md`、`AGENTS.md`、`plans/002-憲法機制/plan.md`、`plans/002-憲法機制/decisions.md`，含還沒 push 的 commit（2026-10-24）。第 5 條（大家共同編輯協作）、第 6 條（不會限制任何門檻）、第 8 條（Open-Minded）與治理「原話不改寫」違反，本 Plan 還不能 Deliver。

| 條文 | 結論 | 依據 |
|---|---|---|
| 第 1 條　公益性質的非營利組織 | 沒有違反 | 四份產出都沒有營利或商業目的；提到 GitHub 付費方案只是說明能力。 |
| 第 2 條　value proposition | 沒有違反 | 四份產出都沒有限縮或否定第 2 條（value proposition）列的 value。 |
| 第 3 條　其他的商業意圖怎麼區分 | 沒有違反 | 沒有收費、置入或分配收入；提到 GitHub、SpecKit 與 decisions.md 指向的格式，都不是推銷。 |
| 第 4 條　附上所有資訊貢獻者 | 沒有違反 | 引用的 GitHub 文件與 SpecKit 都有列名，沒有產出拿掉留名。 |
| 第 5 條　大家共同編輯協作 | 違反（拿不準） | `plans/002-憲法機制/plan.md`「GitHub Organization 協作脈絡（2026-10-24，待釐清）」裡 AI 的 Council 定義草稿與審核設定建議，讓 Council 共同決策、行使特別權限，並要求兩個 Approvals 與 Code Owner 核准，和「不用有拍板」衝突；它標成候選，但憲法只寫需求原文的引用不做檢查。 |
| 第 6 條　不會限制任何門檻 | 違反（拿不準） | 同一節「PR、邀請與審核的候選安排」裡 AI 提的「申請 PR → Council 審核 → 合併 → …→ Member」，把審核放在入會前，和「沒有人審核；申請就能加入」衝突。 |
| 第 7 條　不會要求你一定要幫忙 | 沒有違反 | AI 流程寫的是「申請 PR」，沒有要求先貢獻才能加入，四份產出都沒有要求成員一定要幫忙。 |
| 第 8 條　Open-Minded | 違反（拿不準） | `plans/002-憲法機制/decisions.md` 檔頭指向的格式不在這個 repo 裡，外人拿不到。 |
| 治理：都受憲法約束 | 沒有違反 | 和第 5 條（大家共同編輯協作）、第 6 條（不會限制任何門檻）衝突的內容，已在那兩列判為違反；沒有用重新解讀條文放行，也沒有為了產出改憲法。 |
| 治理：原話不改寫 | 違反 | `plans/002-憲法機制/decisions.md` 決策 001（補入協作脈絡）的完整語意寫「沿用 AI-native Taiwan 的憲法機制 Plan」，把放進本 Plan 寫成使用者的決定；他的原話是「那個 project 中的 plan」；decisions.md 只能 append，AI 不能替他寫決策。 |
| 治理：修改憲法 | 沒有違反 | 憲法只在 Plan 002（憲法機制）建立時改過，git 裡只有一個版本；GitHub 一節明寫不改憲法。 |
| 治理：怎麼檢查 | 沒有違反 | 由 subagent 依 AGENTS.md 逐條檢查四份產出全文與 diff，結論寫在本節。 |
