# 自我介紹與 PR 提交說明

加入方式依[申請制度](<../specs/01-制度/[機制] 憲政制度.md#申請與成員資格>)。一般申請以自介 PR 為基礎門檻；資格生效、首屆任命例外及退出恢復均依[憲政制度](<../specs/01-制度/[機制] 憲政制度.md>)。Discord 邀請、Star 及活動留言不取代自介審查。

## 自介參考範例

每個人都要在自介附上一張本人的真人照片。照片放在 `members/assets/`，自介以相對連結引用。

下方格式可自由調整。請寫清楚你是誰、為什麼加入、想要獲得什麼、想分享什麼，以及自己的 Contributions：可以幫什麼忙、想要幫什麼忙。

自介看的是參與真誠，不看背景、實力或經歷。沒有專案、仍在探索創業志向，也可以如實說明。Contributions 必須在提交前寫清楚，不能留待之後補充；寫得越清楚，未來大家有志辦活動時，越能善用 AI 找到相關可以幫忙的志工。這不表示承諾接受任何指定工作。

```markdown
# <你的名字或慣用稱呼>

![<你的名字或慣用稱呼>的真人照片](assets/<你的 GitHub 帳號>.<副檔名>)

## 我是誰

<介紹目前在做什麼、關注什麼。正在創業、做產品、工作、就學或仍在探索，都可以如實寫。>

Member ID：待配置
GitHub：<你的 GitHub 帳號>
其他聯絡方式或作品連結：<填寫你願意公開的聯絡方式或作品連結，選填。>

## 為什麼想加入

<是什麼讓你想加入這個組織？可以從最近遇到的問題、一次經驗，或想嘗試的事情說起。如果還不確定自己的創業志向，也可以說明目前想探索什麼。>

## 想要獲得什麼

<你目前最想釐清什麼問題、學到什麼，或認識能交流哪些事情的人？請盡量具體，讓大家知道可以跟你聊什麼、在哪裡提供協助。>

## 想分享什麼

<有哪些經驗、故事、知識、做法或正在嘗試的事情，願意和大家分享？尚未有完整成果也可以如實寫。>

## 我的 Contributions：可以幫什麼忙、想要幫什麼忙

Contributions 必須在提交前寫清楚，不能留待之後補充。寫得越清楚越好：未來大家有志要辦任何活動，都可以善用 AI，透過 Contributions 尋找相關可以幫忙的志工。

### 可以幫什麼忙

<具體寫出你目前可以協助的事情，以及能協助到什麼程度，讓發起活動的人與 AI 知道哪些事情可以找你。>

### 想要幫什麼忙

<具體寫出你有意願參與哪些活動或工作、想協助哪個部分。可以是你想一起嘗試或邊做邊學的事情，請說明清楚。>
```

## 提交 PR

1. 登入 GitHub，Fork [本 Repo](https://github.com/AI-Native-Founders-TW/ai-native-founders-tw-mono)。
2. 在自己的 Fork 建立分支，在 `members/` 新增一份 Markdown 自介。初次申請使用 `pending-<小寫GitHub帳號>.md`，Member ID 保留「待配置」，不自行選編號；已有編號者直接更新原自介。正式檔名與識別規則依[成員識別與資料](<../specs/01-制度/[規格]成員識別與資料.md>)，由合併人員在合併前配置。同時將本人的真人照片上傳至 `members/assets/`，例如 `<你的 GitHub 帳號>.jpg`，並在自介引用相同檔名。不要修改別人的自介或照片。
3. 將範例中的 `<...>` 替換成自己的內容。可以用 AI 協助整理，但提交前務必由本人親自 review 全文：確認照片是本人的真人照片且可公開、圖片正常顯示，以及經歷、連結、動機、期待與 Contributions 真實，沒有 AI 編造的內容或參與承諾，也沒有不願公開的個資。
4. 依[成員參與制度](<../specs/01-制度/[機制] 憲政制度.md#rr-assignment>)，從 [R&R assignment 表](r-and-r-assignment.md)選至少一個 R&R，將自己列入 Contributors，可選多個。同步更新 [members 總表](members.md)中的自介連結及 R&Rs；申請尚未通過時，列於「申請中」區的本人小節，自介 PR 欄位先標示待建立。兩表都連到自己的自介，填寫目前 GitHub 帳號；尚未配置編號時填「待配置」，不修改其他人的 assignment。
5. Commit 變更後，從自己的分支開啟 Pull Request，目標為本 Repo 的 `main`。確認變更只有自己的自介、照片，以及兩表中與自己有關的資料，再按 **Create pull request**。建立後，將 PR 連結補入「申請中」本人小節的自介 PR 欄位，Commit 到同一分支以更新同一個 PR。可參考 [GitHub 官方 PR 說明](https://docs.github.com/en/pull-requests/how-tos/create-pull-requests/creating-a-pull-request-from-a-fork)。
6. PR 是申請，審查通過後才成為成員。若需要補充，依 PR 上的審查意見修正。有不熟悉的操作或問題，可以在 Discord 中發問或回覆。

審查依現行[申請制度](<../specs/01-制度/[機制] 憲政制度.md#申請與成員資格>)辦理，執行安排見[自介審查](<../specs/01-制度/[機制] 憲政制度.md#自介審查>)。Onboard Leader 依制度審查，異議交非涉案覆核人；通過後只邀請成為 GitHub org Member，不加入 Members team，後續繼續使用 Fork／PR。具體處理見[自介 PR 審查 SOP](<../specs/03-SOP/[SOP]自介PR審查SOP.md>)，收件、排隊、承接後處理目標依憲政制度；處理目標不保證任何時候都有可承接人力。

## Traceability matrix

Contributions 描述個人可以幫什麼忙、想要幫什麼忙；R&R assignment 記錄成員選擇參與的分工。兩者分開維護，不從自介內容自動推定 assignment。

| 資料 | 維護位置 | Traceability 與更新方式 |
|---|---|---|
| 加入與自介審查規則 | [申請制度](<../specs/01-制度/[機制] 憲政制度.md#申請與成員資格>) | 自介與成員名冊依此判定資格；合併資料或加入 Discord 不能代替審查。 |
| Leader、Contributors 與每人至少選一個 R&R 的規則 | [成員參與制度](<../specs/01-制度/[機制] 憲政制度.md#rr-assignment>) | assignment 表依此記錄，不在表格另訂制度。 |
| 各 R&R 的責任、routine／non-routine 與 SOP | [R&R package](<../specs/02-R&R/README.md>) | 責任定義與人員分開；assignment 連回對應文件，不複製責任或執行紀錄。 |
| Member ID 與目前 GitHub 帳號 | 個人自介，規則依[成員識別與資料](<../specs/01-制度/[規格]成員識別與資料.md>) | 總表抄錄為索引，assignment 以編號核對；配置或帳號變更在同一 PR 同步。 |
| 個人介紹、照片與 Contributions | 各成員自介檔案；照片在 [assets](assets/README.md) | [members 總表](members.md)連回每份自介。能力與意願由本人維護。 |
| 每個 R&R 的 Leader 與 Contributors | [R&R assignment 表](r-and-r-assignment.md) | assignment 的唯一維護來源；每個人連回自己的自介。初始 R&R 的原始依據另連會議記錄，不將歷史認領當成新 assignment。 |
| 所有成員、自介連結與個人 R&Rs | [members 總表](members.md) | R&Rs 是 assignment 表的按人分節索引，連到各 R&R；不能單獨在總表指派工作。申請中另區，不混入成員區。 |

調整自己的 Contributors 選擇時，在同一個 PR 更新 assignment 表與 members 總表；Contributions 有變時一起修訂自介。新增成員時，核對審查通過紀錄再將「申請中」資料移入成員區；沒有有效資格依據時不先標成成員；首屆任命與退出恢復依憲政制度提供對應證據，不虛構一般審查。每次 review 核對兩表能雙向找到同一人、同一 R&R，以及所有成員都至少有一個 Contributors assignment。

## 多人編輯格式

assignment 每項 R&R 獨立一節，Leader 與 Contributors 分開，每位 Contributor 一行；members 總表每人一節、每個欄位與每項 R&R 一行。新增自己的資料時保留其他人的行與順序，避免多人修改同一行造成合併衝突。兩份文件仍維持原有資料責任與同步要求。

## 編號與帳號維護

識別規則以[成員識別與資料](<../specs/01-制度/[規格]成員識別與資料.md>)為準。準備合併時由有權限者配置編號並同步自介與兩表；申請者不需競爭下一個號碼。改帳號請在 PR 說明原帳號、新帳號與本人對應依據，保留編號；退出恢復沿用原自介。對應尚未核對時不自行改成另一個人，也不以公開私人證件為預設要求。
