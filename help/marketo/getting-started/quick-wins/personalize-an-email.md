---
unique-page-id: 2359422
description: 個人化電子郵件——行銷人員檔案——產品檔案
title: 個人化電子郵件
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---


# 個人化電子郵件 {#personalize-an-email}

## 任務：新增資料Token，讓您的電子郵件個人化 {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!NOTE]
>
>**FYI**
>
>Marketo現在正在標準化所有訂閱的語言，因此您可能會在您的訂閱中看到潛在客戶／潛在客戶，並在docs.marketo.com中看到個人／人員。 這些術語意義相同；它不會影響文章指示。 還有一些其他變化。 [進一步瞭解](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)。

>[!NOTE]
>
>**必要條件**
>
>* [設定並新增人員](get-set-up-and-add-a-person.md)
>* [傳送電子郵件爆炸](send-an-email.md)
>* [滴水，滴水，培養](drip-drip-nurture.md)


## 步驟1:選擇要個人化的電子郵件 {#step-select-an-email-to-personalize}

1. 選擇前一個快速贏取中建立的後繼電子郵件 [，然後按一下](drip-drip-nurture.md) 「編 **輯草稿」**。

   ![](assets/one-4.png)

   >[!NOTE]
   >
   >這會建立電子郵件的草稿副本。 您必須核准變更的草稿才能上線。

   **編輯草稿**

如果您尚未啟用快顯封鎖程式，電子郵件編輯器將會在新的標籤／視窗中開啟。 否則，請按兩下。

## 步驟2:讓銷售人員成為發件人 {#step-make-the-salesperson-the-sender}

1. 選擇「 **從** 」欄位，反白 **標示並** 刪除目前名稱。

   ![](assets/two-5.png)

1. 按一 **下** 「寄件者」欄位右側的 **Token圖示** 。

   ![](assets/three-4.png)

1. 尋找並選取 **`{{lead.Lead Owner First Name}}`** Token。

   ![](assets/four-3.png)

1. 輸入您的公司名稱及預設值破折號 **** ，以確保在銷售代表的名字無法使用時，會顯示某些內容。 按一 **下插入**。

   ![](assets/five-4.png)

1. 按一下「從」欄 **位中的空格列** ，確定游標在剛插入的Token後閃爍一個空格。 然後再按一 **下Token** 圖示。

   ![](assets/six-4.png)

1. 尋找並選取 **`{{lead.Lead Owner Last Name}}`** Token。

   ![](assets/seven-5.png)

1. 鍵入「Sales」作為預設 **值** ，然後按一下 **Insert**。

   ![](assets/eight-3.png)

## 步驟3:將銷售線索的名稱新增至電子郵件 {#step-add-the-leads-name-to-the-email}

1. 選擇頂部的可編輯部分，按一下齒輪表徵圖並選擇「編 **輯」**。

   ![](assets/nine-2.png)

1. 在&quot;Hello&quot;後面加上空格，將游標置於逗號前面，然後按一下「插入 **Token** 」圖示。

   ![](assets/ten-4.png)

1. 尋找並選取 **`{{lead.First Name}}`** Token。

   ![](assets/eleven-4.png)

1. 在「預設值」欄位中輸入「朋友」（或您想要的任何標籤）, **然後按一下** 「插入 **」**。

   ![](assets/twelve-3.png)

   >[!TIP]
   >
   >一律包含Token的預設值；這可確保在遺失部分個人資訊時，會在電子郵件中顯示預設值。

1. 按一下 **儲存**。

   ![](assets/thirteen-3.png)

1. 關閉電子郵件編輯器頁籤／窗口。

   ![](assets/fourteen-3.png)

1. 在「電 **子郵件動作**」下，選 **取「核准草稿」**。

   ![](assets/fifteen-3.png)

>[!TIP]
>
>需要快速複習一下如何自己傳送電子郵件？ 請參 [閱傳送電子郵件爆炸](send-an-email.md)。

### 觀看影片 {#watch-a-video}

`<iframe width="630" height="470" src="//play.vidyard.com/iRnqxMyJg6VKyuPeuxmHFb.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`

### 任務完成 {#mission-complete}

恭喜您，您的電子郵件已個人化！

<br> 

[◄使命6:滴滴，滴滴，培養](drip-drip-nurture.md) 8 [號任務：通知銷售代表►](alert-the-sales-rep.md)