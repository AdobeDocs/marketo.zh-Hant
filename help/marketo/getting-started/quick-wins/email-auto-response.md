---
unique-page-id: 2359416
description: 電子郵件自動響應 — Marketo文檔 — 產品文檔
title: 電子郵件自動響應
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# 電子郵件自動響應 {#email-auto-response}

## 任務：當某人填寫表格時發送一封感謝電子郵件 {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [設定並添加人員](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;
>* [帶表單的登錄頁](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;


## 步驟1:建立電子郵件 {#step-create-an-email}

1. 轉至「市場營銷活動」區域。

   ![](assets/one-2.png)

1. 在左菜單中選擇「My Program（我的程式）」 ，按一下「New（新建）」下拉菜單，然後選擇「New Local Asset（新建本地資產）」。

   ![](assets/two-3.png)

1. 按一下「E-mail（電子郵件）」。

   ![](assets/three-2.png)

1. 將電子郵件命名為「自動響應電子郵件」，選擇模板並按一下「建立」。

   ![](assets/four-1.png)

   將在新窗口或頁籤中開啟電子郵件編輯器。 如果彈出窗口被阻止，請按一下 **編輯草稿** 訪問電子郵件。

1. 輸入主題行，然後按兩下電子郵件的可編輯區域。

   ![](assets/five-2.png)

   _將在電子郵件編輯器頂部開啟一個富格文本編輯器。_

1. 突出顯示現有電子郵件內容。

   ![](assets/six-2.png)

1. 鍵入您的電子郵件內容，然後按一下「保存」。

   ![](assets/seven-2.png)

1. 您所做的更改將自動保存。 關閉電子郵件編輯器頁籤/窗口。

   ![](assets/eight-1.png)

1. 選擇新電子郵件。 在「電子郵件操作」下，按一下「批准」。

   ![](assets/image2014-9-24-11-3a55-3a16.png)

## 步驟2:建立智慧市場活動 {#step-create-a-smart-campaign}

1. 按一下右鍵 **我的程式** 按一下 **新智慧營銷**。

   ![](assets/image2014-9-24-11-3a56-3a13.png)

1. **名稱** 您的智慧市場活動「自動響應市場活動」，然後按一下 **建立**。

   ![](assets/image2014-9-24-11-3a56-3a25.png)

1. 轉到 **智慧清單** 頁籤。

   ![](assets/image2014-9-24-11-3a56-3a38.png)

   我們將設定此市場活動以在人員填寫您在中建立的表單時運行 [**帶表單的登錄頁**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}。

1. 查找並拖動 **填出窗體** 觸發到左畫布。

   ![](assets/image2014-9-24-11-3a57-3a18.png)

1. 選擇 **我的表格** 的下界。 按一下 **流** 頁籤。

   ![](assets/image2014-9-24-11-3a57-3a29.png)

1. 拖動 **發送電子郵件** 向左畫布顯示流操作。

   ![](assets/image2014-9-24-11-3a57-3a41.png)

1. 選擇 **自動響應電子郵件** 去 **計畫** 頁籤。

   ![](assets/image2014-9-24-11-3a57-3a53.png)

1. 按一下 **編輯**。

   ![](assets/8.png)

1. 選擇 **每次** 按一下 **保存**。

   ![](assets/9.png)

1. 按一下 **激活**。

   ![](assets/10.png)

1. 按一下 **激活** 確認螢幕上。

   ![](assets/11.png)

>[!NOTE]
>
>一旦激活，此市場活動將在每次人員填寫指定表單時運行。 這個活動會一直進行到停用為止。

## 第3步：填寫表單 {#step-fill-out-the-form}

1. 選擇 **我的頁面**。 建立於 [帶表單的登錄頁](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}快速贏。

   ![](assets/image2014-9-24-12-3a0-3a8.png)

1. 按一下 **「查看已批准」頁**。

   ![](assets/image2014-9-24-12-3a0-3a18.png)

   您的「免費試用」登錄頁將在新頁籤中開啟。

1. 用您的名字、姓氏和電子郵件地址填寫表單，然後按一下 **提交**。

   ![](assets/image2014-9-24-12-3a0-3a28.png)

>[!NOTE]
>
>確保使用您的實際電子郵件地址，以便您能夠收到電子郵件。

## 任務完成 {#mission-complete}

您應在幾分鐘內在收件箱中看到自動響應電子郵件。 幹得好！

<br> 

[◄任務3:簡單計分](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[任務5:導入人員列►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
