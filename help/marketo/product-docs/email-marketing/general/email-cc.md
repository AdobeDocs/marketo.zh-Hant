---
unique-page-id: 17727995
description: Email CC - Marketo檔案 — 產品檔案
title: Email CC
exl-id: 00550e98-916d-4e66-91f8-7394c242a29b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# Email CC {#email-cc}

電子郵件CC可讓透過Marketo傳送的指定電子郵件包含CC收件者。

無論電子郵件的傳送方式（批次或觸發促銷活動）為何，所有Marketo電子郵件資產都可使用此功能。 CC收件者會收到傳送給所選Marketo人員之電子郵件的完整副本。 因此，任何參與活動（開啟、點按等） 會記錄至電子郵件「收件人」行中Marketo人員的活動記錄。 不過，傳送活動（傳送、傳送、硬退信等） _除了「軟跳出」_ will **not** 註冊，因為Marketo無法區分Marketo人員與CC收件者的傳送事件。 Marketo一次只能容納10萬人。 如果您的智慧清單超過10萬，而且每個人必須獲得CC&#39;d，建議您將清單分解。

>[!NOTE]
>
>Email CC的設計不用於A/B測試。 如果您願意，也可以使用它，但由於技術上不支援，Marketo支援將無法協助進行任何疑難排解。

## 設定電子郵件CC {#set-up-email-cc}

1. 在「我的Marketo」中，按一下 **管理**.

   ![](assets/one.png)

1. 在樹中，選擇 **電子郵件**.

   ![](assets/two.png)

1. 按一下 **編輯電子郵件CC設定**.

   ![](assets/three.png)

1. 選取最多25個Marketo銷售機會或公司欄位（「電子郵件」類型），即可在電子郵件中當作CC地址使用。 按一下 **儲存** 時才能使用。

   ![](assets/four.png)

## 使用電子郵件CC {#using-email-cc}

1. 選取您的電子郵件，然後按一下 **編輯草稿**.

   ![](assets/five.png)

1. 按一下 **電子郵件設定**.

   ![](assets/six.png)

1. 選擇最多5個用於CC People的欄位。 在此示例中，我們只需要Lead Owner CC&#39;d。按一下 **儲存** 時才能使用。

   ![](assets/seven.png)

   就這樣簡單！ 在上述範例中，當您傳送電子郵件時，您所選收件者的「主要擁有者」將會是「CC&#39;d」。

   >[!NOTE]
   >
   >如果「抄送」欄位中包含無效的電子郵件地址，系統會略過該地址。

   為了快速識別，「電子郵件摘要」檢視會顯示是否已選取/選取了哪些電子郵件CC欄位。

   ![](assets/eight.png)

   如果電子郵件已核准，但Marketo管理員在傳送電子郵件前會停用一或多個CC欄位， **那些人不會收到電子郵件**. 在該案例中，「電子郵件摘要」檢視會將核准後但預先傳送的任何已停用欄位清除：

   ![](assets/removal.png)

   >[!NOTE]
   >
   >您也會在電子郵件草稿的「電子郵件設定」區段中看到上述錯誤。

## 傳送後 {#after-the-send}

* 如果CC收件者點按了電子郵件中的追蹤連結，點按活動（如同所有其他參與活動）將會與電子郵件的主要收件者相關聯。 此外，使用者可點進含有Marketo網頁追蹤代碼(munchkin.js)的頁面，使其成為主要收件者。

>[!TIP]
>
>您可以選擇 [停用部分或全部追蹤連結](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/disable-tracking-for-an-email-link.md) 在電子郵件中。

* 執行電子郵件促銷活動後，「傳送電子郵件」活動將包含郵件每位收件者的所有CC位址清單。 如果因取消訂閱而略過任何CC位址，也會在活動中注明。
* 取消訂閱的連結和頁面可在電子郵件中正常運作。 這可讓CC收件者在有意願時（遵守反垃圾訊息法規）成功取消訂閱，而此動作的記錄會儲存在Marketo資料庫中。
* 在您的Marketo資料庫中列為取消訂閱的人員將 **not** 透過CC接收電子郵件。
