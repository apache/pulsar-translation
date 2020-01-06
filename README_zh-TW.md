# 翻譯工作流程與規範(zh-TW)

歡迎加入 Pulsar 文件翻譯專案！開始翻譯之前，請先閱讀[翻譯工作流程](#翻譯工作流程)和[翻譯規範](#翻譯規範)。

## 翻譯工作流程

Pulsar 的翻譯專案放在 [Apache Pulsar Crowdin](https://crowdin.com/project/apache-pulsar) 上。想要進一步了解 Crowdin 功能，參閱 [Crowdin 網站](https://crowdin.com/) 。
我們的翻譯流程主要有以下步驟。

### 註冊 Crowdin 賬號，加入 Pulsar 翻譯專案群組

登錄 [Apache Pulsar Crowdin project](https://crowdin.com/project/apache-pulsar) 頁面。如果沒有 Crowdin 賬戶，點擊右上角 **SIGN UP**，輸入個人信息創建賬戶。如果你已經有 Github、Facebook，Google，Twitter，Gitlab 賬號，直接在註冊頁面關聯以上任意賬號即可。

登錄成功後，在右上角選擇 **Join（加入）**。
> **注意**
> Pulsar 的源文件為英文，現在正在進行的翻譯項目分為簡體中文、繁體中文、法語和日語。  
> 選擇翻譯目標語言，點擊進入瀏覽。本文以“繁體中文翻譯項目”為例。

### 選擇翻譯文件，提 PR

點開 “Chinese Traditional” ，進入 **master > docs** 目錄中，查看每個文件的翻譯進度。 **master > docs** 目錄中的文件是 Pulsar 官網最新版本的源文件，只需要翻譯這個目錄中的 markdown 文件即可。其中：

- 綠色：翻譯並通過審閱  
- 藍色：翻譯未審閱
- 灰色：未翻譯

![翻譯狀態](media/translation-status.jpg)

根據自己對 Pulsar 及相關技術的理解，優先選擇自己熟悉、尚未翻譯的內容進行翻譯。

選擇要翻譯的文件後，查看 [Translation schedule](https://github.com/apache/pulsar-translation/blob/master/schedule_zh-TW.md) 中是否有其他人在翻譯這個文件。如果已經有，可以重新選擇；如果沒有，創建一個 PR，把自己要翻譯的文件和姓名分別添加進[Translation schedule](https://github.com/apache/pulsar-translation/blob/master/schedule_zh-TW.md)，提交 PR。

### 打標籤

- Reviewers：無需設置，負責人會自動收到您提交的 PR 申請，會安排人員處理。
- Assignees：選擇你自己，方便你後續收到進度通知。
- Label：選擇 `translation`。

### 翻譯

譯者開始翻譯。在打開的翻譯界面，文件 id 不需要翻譯。翻譯中的 tag 和源文件保持一致。
> **重要  
> 一定不要修改、遺漏 tag，或者在 tag 後面加空格。 tag 遺漏或錯位會造成中文網站內容顯示錯亂。**

![id-tag](media/id-tag.jpg)

如果看到有翻譯需要修改的地方，直接在翻譯界面修改、保存。你的翻譯結果會自動出現在翻譯列表的最上方，Crowdin 會自動記載不同譯者的翻譯版本。右下方的 **TM AND MT TRANSLATION** 中會提供 Pulsar、Crowdin 和網站上其他的術語庫，翻譯時可供參考。

![翻譯界面](media/translation-interface.jpg)

翻譯過程中，如需參考或者追加 Pulsar 文檔術語庫，可以使用 [Pulsar 文檔翻譯術語庫](https://shimo.im/sheets/5jozGy5WIUQQf5JV/MODOC)。

### 審閱

翻譯完成後，在你提交的 PR 頁面留言告知：
“I've finished translation, could you please help review?”

Reviewer 收到通知後，開始審閱翻譯內容。審閱完成後，在 PR 中告知譯者，並做簡單點評反饋。如有需要討論的地方，可以直接在 PR 中交流討論。

審閱無誤後，reviewer 批准該 PR，並進行合併。

下圖給出了文件翻譯工作流程。工作流程圖的源文件在以下位置共享 [lucidchat](https://www.lucidchart.com/invitations/accept/0ebad9d8-ddf3-4a92-8ee6-e813a9bc58ff)。
Masakazu 分享更詳細的工作流程[泳道](https://swimlanes.io/d/8L04SRASw)圖。

![翻譯工作流程](media/translation-workflow.jpg)

## 翻譯規範

本規範主要列出了一些常見的翻譯問題，並提供了一些指導意見和建議。開始翻譯前，請認真閱讀並儘量遵守本文的規範，這能有效提高 Pulsar 翻譯文件質量，統一翻譯風格。

### 1. 專有名詞

涉及到 Pulsar、Pulsar Functions、BookKeeper、ZooKeeper，按照上述大小寫格式，保留英文不翻譯。
涉及到 broker，bookie，proxy 等，在句中保持英文小寫形式，不用翻譯。

涉及到 topic，producer，consumer 等，翻譯成“主題”，“生產者”，“消費者”。

更多有關 Pulsar 文檔術語庫，參考 [Pulsar 文檔翻譯術語庫](https://shimo.im/sheets/5jozGy5WIUQQf5JV/MODOC)。歡迎在這個文檔補充和修改術語庫。

### 2. 漢字與英文、數字之間需空格

漢字與英文或數字之間以空格隔開，以增強中英文混排的美觀性和可讀性。

- Apache Pulsar是一個開源的分佈式發布-訂閱信息系統，由Apache軟件基金會管理，並於2018年9月成為Apache頂級開源項目。❌

- Apache Pulsar 是一個開源的分佈式發布-訂閱消息系統，由 Apache 軟件基金會管理，並於 2018 年 9 月成為 Apache 頂級開源項目。✅

**注意：**中文標點符號前後不需要跟空格，即使前後挨著的是英文單詞。

### 3. 中文標點符號

中文裡面請使用中文標點符號。英文中沒有頓號，應該使用頓號的地方在英文中一般使用的是逗號，在翻譯時應注意將其翻譯為頓號。比如 “Kubernetes, Mesos, Docker“ 應該翻譯成 “Kubernetes、Mesos、Docker“。

在涉及到多个 items 时，如果是短语，后面用分号（；）结束，最后一个 item 以句号（。）结尾。

如果每個 item 是個句子，或者已經使用過分號（；），每個 item 以句號結尾。

![頓號範例](media/example-comma.jpg)

上面這個例子中，使用句號（。）給每條實踐結尾。

### 4. “you“翻譯為“你“

為了風格統一，在翻譯“you”時，可以省略時，盡量省略不用；必須使用時，用“你”，而不是“您”。

### 5. 範例代碼及註釋

範例代碼中的註釋最好能夠翻譯，當然也可以不翻譯（當註釋很簡單時）。

### 6. 意譯優於直譯

翻譯時盡量避免翻譯腔，即把原文一字不漏地、逐句翻譯出來。這樣並不代表翻譯更準確，有時候讀著會很彆扭。翻譯完後，自己多讀幾遍，看看是否符合原意、是否繞口、是否簡潔。在充分理解原文的基礎上，可以適當採用意譯的方式來翻譯。有時候為了簡化句子，有些數量詞、助詞、主語都可以省略。

#### 6.1 ...的...的...的

比如英文中經常會用 ‘s 來表達從屬關係，一字不落地都將其翻譯成 “的“ 會有翻譯腔。在中文裡面有些 “的“ 完全可以去掉，不會影響表達的意思，還能簡潔很多，看下面的例子。

- Pulsar‘s documentation is located in the docs folder in Pulsar’s source code repository.

當然，你可以將“的“字都翻譯出來，但是讀起來很不順暢：

- Pulsar 的文檔位於 Pulsar 的源碼倉庫的 docs 文件夾中。 ❌

去掉不必要的“的“字，就會簡潔很多：

- Pulsar 文檔位於 Pulsar 源碼倉庫的 docs 文件夾中。 ✅

#### 6.2 一個……

英文一般比較嚴謹，當代表多個時，會使用複數名詞，在翻譯成中文時，一般不需要刻意把這些複數翻譯出來。

在英文裡，當單數為可數名詞時，前面一般會有 ”a“ 或 ”an“；中文中，我們一般不需要把”一個...“翻譯出來。比如下面這個例子：

- Using a Pulsar client with the proxy

我們可以把”a“翻譯成”一個“：

- 使用有 proxy 的一個 Pulsar 客戶端   ❌  

雖然看起來沒什麼問題，但是這裡的”一個“是多餘的，去掉之後不但不會影響翻譯效果，而且更加簡潔。

- 使用有 proxy 的 Pulsar 客户端   ✅

### 7. 盡量少用被動句

英文文檔中，有時以物為主語，中文翻譯過程中，不需要把”被“字翻譯出來。例如：

- 英文：Once the message above has been successfully published to the topic, you should see it in the standard output: Hello Pulsar.
- 原翻譯：一旦上面的信息被成功發佈到Topic中，您會在標準輸出中看到它：Hello Pulsar。  ❌
- 翻譯調整：上面的信息成功發佈到主題後，你會在標準輸出中看到: Hello Pulsar。    ✅

### 8. Will 未來時態

英文中有 “will” 時，不用翻譯成 “將要......”，直接轉換成一般現在時態翻譯就行。例如：

- 英文：This will publish a single message to the Pulsar topic.
- 原翻譯：這將向Pulsar的Topic發送單條信息。   ❌
- 翻譯調整：（......）給 Pulsar 主題發布一條信息。   ✅

### 9. 範例

在英文中遇到 “Here‘s sth”，根據上下文語義做調整。例如：

- 英文：Here's an example.
- 原翻譯：這裡有一個範例。   ❌
- 翻譯調整：下面是一個範例。     ✅

### 10. 語言簡潔、流暢

語言盡量簡單、通順，翻譯完後，讀一遍，適合繁體中文人士的閱讀習慣。英語中有時會用從句，翻譯中文時，盡量拆成幾個簡單的句子。

## 成為貢獻者

當你的第一個 pull request 被合併後, 把你的名字加進[貢獻者名單](https://github.com/apache/pulsar-translation/blob/master/CONTRIBUTORS.md)中。
