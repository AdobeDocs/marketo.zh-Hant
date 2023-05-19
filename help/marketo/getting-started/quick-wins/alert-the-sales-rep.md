---
unique-page-id: 2359424
description: 通知銷售代表 — Marketo文檔 — 產品文檔
title: 通知銷售代表
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
source-git-commit: 80512816eaf0a70a3f10a50c34aeea14edd9046b
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# 通知銷售代表 {#alert-the-sales-rep}

## 任務：當某人填寫您網站上的表單時，通知銷售代表 {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

要自動向銷售代表發送警報電子郵件，您只需要一封警報電子郵件和一次電子郵件活動。 這是如何做到的。

>[!PREREQUISITES]
>
>[帶表單的登錄頁](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## 步驟1:建立警報電子郵件 {#step-create-an-alert-email}

1. 轉到 **[!UICONTROL 營銷活動]** 的子菜單。

   ![](assets/alert-the-sales-rep-1.png)

1. 選擇 **我的程式** 在 [帶表單的登錄頁](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} 快贏，然後下 **[!UICONTROL 新建]** 按一下 **[!UICONTROL 新建本地資產]**。

   ![](assets/alert-the-sales-rep-2.png)

1. 按一下 **[!UICONTROL 電子郵件]**。

   ![](assets/alert-the-sales-rep-3.png)

1. **名稱** 電子郵件「我的電子郵件警報」，選擇模板，然後按一下 **[!UICONTROL 建立]**。

   ![](assets/alert-the-sales-rep-4.png)

1. 輸入 **從名稱**。 **從電子郵件**。 **[!UICONTROL 回復]**, **[!UICONTROL 主題]** 你希望你的銷售團隊能看到。

   ![](assets/alert-the-sales-rep-5.png)

1. 按兩下可編輯電子郵件文本。

   ![](assets/alert-the-sales-rep-6.png)

1. 鍵入電子郵件內容。

   ![](assets/alert-the-sales-rep-7.png)

1. 將游標置於要插入人員聯繫資訊的位置，然後按一下 **插入標籤** 表徵圖

   ![](assets/alert-the-sales-rep-8.png)

1. 查找並選擇 `{{SP_Send_Alert_Info}}` **[!UICONTROL 令牌]** 按一下 **[!UICONTROL 插入]**。

   ![](assets/alert-the-sales-rep-9.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} 是警報電子郵件的特殊令牌。 請參閱 [使用發送警報資訊令牌](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"}{target="_blank"} 來瞭解更多資訊。

1. 按一下 **[!UICONTROL 保存]**。

   ![](assets/alert-the-sales-rep-10.png)

1. 按一下 **[!UICONTROL 電子郵件操作]** 下拉並選擇 **[!UICONTROL 批准和關閉]**。

   ![](assets/alert-the-sales-rep-11.png)

## 步驟2:建立警報觸發市場活動 {#step-create-an-alert-trigger-campaign}

1. 選擇 **我的程式** 先前建立，然後在 **[!UICONTROL 新建]** 按一下 **[!UICONTROL 新智慧營銷]**。

   ![](assets/alert-the-sales-rep-12.png)

1. **名稱** 市場活動「我的警報市場活動」，然後按一下 **[!UICONTROL 建立]**。

   ![](assets/alert-the-sales-rep-13.png)

1. 在 **[!UICONTROL 智慧清單]** 頁籤，查找並拖動 **[!UICONTROL 填出窗體]** 觸發到畫布。

   ![](assets/alert-the-sales-rep-14.png)

1. 選擇我們先前建立的窗體。

   ![](assets/alert-the-sales-rep-15.png)

1. 在 **[!UICONTROL 流]** 頁籤，查找並拖動 **[!UICONTROL 發送警報]** 將操作流到畫布。

   ![](assets/alert-the-sales-rep-16.png)

1. 選擇 **[!UICONTROL 我的警報電子郵件]** 建立時間早於 **[!UICONTROL 發送到]** 如 **[!UICONTROL 銷售所有者]**。

   ![](assets/alert-the-sales-rep-17.png)

1. 在 **[!UICONTROL 到其他電子郵件]** 的子菜單。

   ![](assets/alert-the-sales-rep-18.png)

1. 轉到 **[!UICONTROL 計畫]** ，然後按一下 **[!UICONTROL 激活]** 按鈕

   ![](assets/alert-the-sales-rep-19.png)

   >[!TIP]
   >
   >設定 **[!UICONTROL 資格規則]** 至 **[!UICONTROL 每次]** （通過編輯智慧市場活動），允許同一人多次觸發警報。

1. 按一下 **[!UICONTROL 激活]** 確認螢幕上。

   ![](assets/alert-the-sales-rep-20.png)

## 第3步：Test! {#step-test-it-out}

1. 選擇登錄頁並按一下 **[!UICONTROL 「查看已批准」頁]**。

   ![](assets/alert-the-sales-21.png)

   >[!NOTE]
   >
   >不要忘記批准登錄頁；除非獲得批准，否則他們不會活下去。

1. 填寫表單，然後按一下 **[!UICONTROL 提交]**。

   ![](assets/alert-the-sales-22.png)

1. 您應盡快收到電子郵件。 在您驗證所有內容都按應用方式運行後，請從「發送警報」流中刪除您的電子郵件地址（請參閱上面的步驟2.7）。

   >[!NOTE]
   >
   >按一下 **[!UICONTROL 人員資訊]** 的子菜單。

## 任務完成！ {#mission-complete}

<br> 

[◄任務7:個性化電子郵件](/help/marketo/getting-started/quick-wins/personalize-an-email.md)

[任務9:更新人員數►](/help/marketo/getting-started/quick-wins/update-person-data.md)
