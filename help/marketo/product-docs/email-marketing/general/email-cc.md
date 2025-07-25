---
unique-page-id: 17727995
description: 電子郵件副本 — Marketo檔案 — 產品檔案
title: 電子郵件副本
exl-id: 00550e98-916d-4e66-91f8-7394c242a29b
feature: Email Editor
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 電子郵件副本 {#email-cc}

電子郵件副本可允許透過Marketo傳送的指定電子郵件包含副本收件人。

此功能適用於所有Marketo電子郵件資產，無論電子郵件的傳送方式（批次或觸發行銷活動）為何。 副本抄送收件者將收到寄給選定Marketo人員之電子郵件的完整副本。 因此，任何參與活動（開啟、點按等）都會記錄到電子郵件「收件者」行中Marketo人員的活動記錄。 但是，「軟退信」以外的傳遞活動（已傳送、已傳遞、硬退信等）_將_&#x200B;不會&#x200B;**註冊，因為Marketo無法區分「Marketo人員」的傳遞事件和「副本抄送收件者」。** Marketo一次最多只能副本10萬人。 如果您的智慧清單超過100,000且清單上的每個人都必須收到副本，我們建議您分拆清單。

>[!NOTE]
>
>電子郵件CC的設計不適用於A/B測試。 您仍然可以視需要使用，但由於技術上不支援，Marketo支援將無法協助進行任何疑難排解。

## 設定電子郵件副本 {#set-up-email-cc}

1. 在「我的Marketo」中，按一下&#x200B;**[!UICONTROL Admin]**。

   ![](assets/one.png)

1. 在樹狀結構中，選取&#x200B;**[!UICONTROL Email]**。

   ![](assets/two.png)

1. 按一下「**[!UICONTROL Edit Email CC Settings]**」。

   ![](assets/three.png)

1. 選取最多25個Marketo銷售機會或公司欄位（型別為「電子郵件」），以在電子郵件中作為副本地址使用。 完成時，按一下&#x200B;**儲存**。

   ![](assets/four.png)

## 使用電子郵件副本 {#using-email-cc}

1. 選取您的電子郵件並按一下&#x200B;**[!UICONTROL Edit Draft]**。

   ![](assets/five.png)

1. 按一下「**[!UICONTROL Email Settings]**」。

   ![](assets/six.png)

1. 選取您要用來寄送副本給人員的欄位。 _每封電子郵件限為5封_。 在此範例中，我們只希望Lead Owner抄送。完成時，按一下&#x200B;**儲存**。

   ![](assets/seven.png)

   事情就是這麼簡單！ 在上述範例中，當您傳送電子郵件時，您所選收件者的潛在客戶擁有者將會是「副本」。

   >[!NOTE]
   >
   >如果「副本抄送」欄位中有無效的電子郵件地址，則會略過該地址。

   為了快速識別，「電子郵件摘要」檢視會顯示是否/選取了哪些電子郵件副本欄位。

   ![](assets/eight.png)

   如果電子郵件已核准，但Marketo管理員在傳送電子郵件前停用一或多個「副本」欄位，**這些人員將不會收到電子郵件**。 在該案例中，「電子郵件摘要」檢視會將任何在核准後但預先傳送中停用的欄位變成灰色：

   ![](assets/removal.png)

   >[!NOTE]
   >
   >您也會在電子郵件草稿的電子郵件設定區段中看到上述錯誤。

## 傳送後 {#after-the-send}

* 如果副本收件者按一下電子郵件中的追蹤連結，則點選活動（如所有其他參與活動）將與電子郵件的主要收件者相關聯。 此外，他們可能會點進包含Marketo網頁追蹤程式碼(munchkin.js)的頁面，導致他們被當作主要收件者來處理。

>[!TIP]
>
>您有[停用電子郵件中部分或全部追蹤連結](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/disable-tracking-for-an-email-link.md)的選項。

* 執行電子郵件行銷活動後，「傳送電子郵件」活動將包含每個郵寄收件者所包括的所有CC位址清單。 如果因取消訂閱而略過任何CC位址，活動也會記錄該位址。
* 取消訂閱連結和頁面在副本電子郵件中正常運作。 這可讓CC收件者依需求成功取消訂閱（遵循反垃圾郵件法規），而且此動作的記錄會儲存在Marketo資料庫中。
* 在您的Marketo資料庫中列為已取消訂閱的人員將&#x200B;**不會**&#x200B;透過CC接收電子郵件。
