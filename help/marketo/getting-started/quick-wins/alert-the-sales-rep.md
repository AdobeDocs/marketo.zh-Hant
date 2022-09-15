---
unique-page-id: 2359424
description: 提醒銷售代表 — Marketo文檔 — 產品文檔
title: 通知銷售代表
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
source-git-commit: 1127928b43762086ed4d157719ff80d6c3de9ee3
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# 通知銷售代表 {#alert-the-sales-rep}

## 任務：當有人填寫您網站上的表格時，提醒銷售代表 {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

若要自動傳送警報電子郵件給銷售代表，您只需要一封警報電子郵件和一封電子郵件促銷活動。 這是怎麼做的。

>[!PREREQUISITES]
>
>[具有表單的登陸頁面](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}

## 步驟1:建立警報電子郵件 {#step-create-an-alert-email}

1. 前往 **行銷活動** 的上界。

   ![](assets/alert-the-sales-rep-1.png)

1. 選擇 **我的計畫** 在 [具有表單的登陸頁面](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}快速贏取，然後在 **新增** 按一下 **新本機資產**.

   ![](assets/alert-the-sales-rep-2.png)

1. 按一下 **電子郵件**.

   ![](assets/alert-the-sales-rep-3.png)

1. **名稱** 電子郵件「我的電子郵件警報」，請選取範本，然後按一下 **建立**.

   ![](assets/alert-the-sales-rep-4.png)

1. 輸入 **從名稱**, **從電子郵件**, **回覆**，和 **主旨** 你希望你的銷售團隊能看到。

   ![](assets/alert-the-sales-rep-5.png)

1. 按兩下以編輯電子郵件文本。

   ![](assets/alert-the-sales-rep-6.png)

1. 輸入電子郵件內容。

   ![](assets/alert-the-sales-rep-7.png)

1. 將游標置於要插入人員聯繫資訊的位置，然後按一下 **插入代號** 表徵圖。

   ![](assets/alert-the-sales-rep-8.png)

1. 尋找並選取 `{{SP_Send_Alert_Info}}` **代號** 按一下 **插入**.

   ![](assets/alert-the-sales-rep-9.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} 是警報電子郵件的特殊代號。 請參閱 [使用傳送警報資訊Token](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target=&quot;_blank&quot;}{target=&quot;_blank&quot;}以了解更多資訊。

1. 按一下 **儲存**.

   ![](assets/alert-the-sales-rep-10.png)

1. 按一下 **電子郵件動作** 下拉式清單並選取 **核准並關閉**.

   ![](assets/alert-the-sales-rep-11.png)

## 步驟2:建立警報觸發促銷活動 {#step-create-an-alert-trigger-campaign}

1. 選擇 **我的計畫** 先前建立，然後在下 **新增** 按一下 **新智慧型行銷活動**.

   ![](assets/alert-the-sales-rep-12.png)

1. **名稱** 促銷活動「我的警報促銷活動」，然後按一下 **建立**.

   ![](assets/alert-the-sales-rep-13.png)

1. 在 **智慧清單** 標籤，查找並拖動 **填寫表單** 觸發至畫布。

   ![](assets/alert-the-sales-rep-14.png)

1. 選取先前建立的表單。

   ![](assets/alert-the-sales-rep-15.png)

1. 在 **流量** 標籤，查找並拖動 **傳送警報** 流動動作至畫布。

   ![](assets/alert-the-sales-rep-16.png)

1. 選擇 **我的警報電子郵件** 先建立後保留 **傳送至** as **銷售負責人**.

   ![](assets/alert-the-sales-rep-17.png)

1. 在 **轉至其他電子郵件** 欄位。

   ![](assets/alert-the-sales-rep-18.png)

1. 前往 **排程** ，然後按一下 **啟動** 按鈕。

   ![](assets/alert-the-sales-rep-19.png)

   >[!TIP]
   >
   >設定 **資格規則** to **每次都** （透過編輯「智慧型促銷活動」）來允許同一人觸發警報多次。

1. 按一下 **啟動** 在確認畫面上。

   ![](assets/alert-the-sales-rep-20.png)

## 步驟3:測試出來！ {#step-test-it-out}

1. 選取您的登錄頁面，然後按一下 **「查看已批准」頁**.

   ![](assets/alert-the-sales-21.png)

   >[!NOTE]
   >
   >別忘了核准登錄頁面；直到批准才能上線。

1. 填寫表單，然後按一下 **提交**.

   ![](assets/alert-the-sales-22.png)

1. 您應該很快會收到電子郵件。 在您確認一切皆正常運作後，請從「傳送警報」流程中移除您的電子郵件地址（請參閱上述步驟2.7）。

   >[!NOTE]
   >
   >按一下 **人員資訊** 頁簽，查看聯繫資訊。

## 任務完成！ {#mission-complete}

<br> 

[◄任務7:個人化電子郵件](/help/marketo/getting-started/quick-wins/personalize-an-email.md)

[任務9:更新人員資料►](/help/marketo/getting-started/quick-wins/update-person-data.md)
