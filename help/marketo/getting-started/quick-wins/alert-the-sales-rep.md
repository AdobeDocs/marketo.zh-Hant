---
unique-page-id: 2359424
description: 提醒銷售代表——行銷人員文檔——產品文檔
title: 提醒銷售代表
translation-type: tm+mt
source-git-commit: 09dbd3a141fed0525aec8bf1ca6d141be2a6ce46
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---


# 提醒銷售代表 {#alert-the-sales-rep}

## 任務：當某人填寫您網站上的表格時，提醒銷售代表 {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

若要自動傳送警報電子郵件給業務代表，您只需要寄送警報電子郵件和電子郵件促銷活動。 這是如何做到的。

>[!NOTE]
>
>**FYI**
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

>[!NOTE]
>
>**必要條件**
>
>* [具有表單的著陸頁面](landing-page-with-a-form.md)

>



## 步驟1:建立警報電子郵件 {#step-create-an-alert-email}

1. 前往「行銷 **活動** 」區。

   ![](assets/one-5.png)

1. 選 **擇在「Form** quick win」(帶有Form [quick win的登錄頁)中建立的Program](landing-page-with-a-form.md) （程式），然後在「 **New** 」(新建 **)「** New Local Asset」（本地資產）下面。

   ![](assets/two-6.png)

1. 按一下「 **電子郵件**」。

   ![](assets/three-5.png)

1. **將電子郵件命名** 「我的電子郵件警報」，選取範本，然後按一下「建 **立**」。

   ![](assets/four-4.png)

1. 輸入「來 **自名稱**」、「來自電子郵 **件」、「**&#x200B;回覆至」 **，以及您****** 希望銷售團隊查看的主旨。

   ![](assets/five-5.png)

1. 按兩下以編輯電子郵件文字。

   ![](assets/six-5.png)

1. 輸入電子郵件內容。

   ![](assets/seven-6.png)

1. 將游標置於要插入該人員聯繫資訊的位置，然後按一下「插入 **Token** 」表徵圖。

   ![](assets/eight-4.png)

1. 尋找並選取Token `{{SP_Send_Alert_Info}}` ，然 **後按一** 下Insert ****。

   ![](assets/image2014-9-24-13-3a10-3a0.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}}是警報電子郵件的特殊Token。 請參 [閱使用傳送警報資訊Token](../../product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) ，瞭解更多資訊。

1. 按一下 **儲存**。

   ![](assets/ten-5.png)

1. 關閉電子郵件編輯器頁籤／窗口。

   ![](assets/eleven-5.png)

1. 在「電子 **郵件動作** 」下，按 **一下「核准**」。

   ![](assets/twelve-4.png)

## 步驟2:建立警報觸發器促銷活動 {#step-create-an-alert-trigger-campaign}

1. 選擇 **先前建立的My Program** ，然後在**New **click **New Smart Campaign下方**。

   ![](assets/image2014-9-24-13-3a14-3a17.png)

1. **將促銷活動命名** 「我的警報促銷活動」，然後按一下「建 **立**」。

   ![](assets/image2014-9-24-13-3a14-3a28.png)

1. 在「智 **慧型清單** 」標籤下，尋找並拖曳「填 **** 色表單」觸發器至畫布。

   ![](assets/image2014-9-24-13-3a14-3a43.png)

1. 選取我們先前建立的表單。

   ![](assets/image2014-9-24-13-3a14-3a58.png)

1. 在「流 **量** 」標籤下，尋找並拖曳「傳送 **警報流量** 」動作至畫布。

   ![](assets/image2014-9-24-13-3a15-3a10.png)

1. 選擇 **My Alert Email** created arearly **，並保留** Send To **(發送至**)作為銷售者。

   ![](assets/eighteen-1.png)

1. 在「收件者其他電子郵件」欄 **位中輸入您的電子郵件地址** 。

   ![](assets/nineteen-2.png)

1. 前往「排 **程** 」標籤，然後按一下「啟動**」按鈕。

   ![](assets/twenty-2.png)

   >[!TIP]
   >
   >
   >將「資 **格規則** 」設 **定為每次** （透過編輯「智慧型促銷活動」），以允許同一人多次觸發警報。

1. 按一 **下確認畫面** 上的「啟動」。

   ![](assets/twenty-one-1.png)

## 步驟3:測試一下！ {#step-test-it-out}

1. 選取您的著陸頁面，然後按一 **下「檢視已核准頁面**」。

   ![](assets/image2014-9-24-13-3a17-3a8.png)

   >[!NOTE]
   >
   >**提醒**
   >
   >
   >不要忘記核准登陸頁面；他們要等到批准才上線。

1. 填寫表格，然後按一下「 **提交**」。

   ![](assets/image2014-9-24-13-3a17-3a41.png)

1. 您應該很快就會收到電子郵件。 在您確認一切都正常運作後，請從「傳送警報」流程中移除您的電子郵件地址（請參閱上述步驟2.7）。

   >[!NOTE]
   >
   >按一下Market **中的「人員資訊** 」標籤，以檢視連絡資訊。

## 任務完成！ {#mission-complete}

<br> 

[◄使命7:個人化電子郵件](personalize-an-email.md)[任務9:更新銷售線索資料►](update-person-data.md)