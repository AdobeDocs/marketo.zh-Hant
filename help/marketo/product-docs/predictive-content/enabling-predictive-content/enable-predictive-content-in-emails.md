---
unique-page-id: 11385020
description: 啟用電子郵件中的預測性內容 — Marketo文檔 — 產品文檔
title: 啟用電子郵件中的預測性內容
exl-id: 7eaefee1-23e8-47ee-afff-adcf49096aa7
source-git-commit: 4b1b91a933a7a6d103fe0d44ece9ea95759edc5f
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# 啟用電子郵件中的預測性內容 {#enable-predictive-content-in-emails}

在電子郵件中預測一個或多個影像，為每個收件人定制體驗。

>[!NOTE]
>
>建議在測試和使用預測性內容之前，先按類別和每個源啟用五個以上的內容（電子郵件、富媒體、欄）。 更多內容將為您提供更好的預測結果。

>[!PREREQUISITES]
>
>在啟用預測性內容之前，必須：
>
>* **準備預測性內容**
   >
   >   * [編輯電子郵件的預測內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md){target=&quot;_blank&quot;或
   >   * [編輯富媒體的預測內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md){target=&quot;_blank&quot;或
   >   * [編輯建議欄的預測內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md){target=&quot;_blank&quot;
>
>* [批准預測內容的標題](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md){target=&quot;_blank&quot;


## 使用E-mail 2.0編輯器添加預測性內容 {#adding-predictive-content-using-the-email-editor}

1. 按一下 **營銷活動**。

   ![](assets/one.png)

1. 選擇您的電子郵件，然後按一下 **編輯草稿**。

   ![](assets/two.png)

1. 按一下要進行預測的影像。 當齒輪表徵圖出現時，按一下它並選擇 **啟用內容AI** （ContentAI是「預測內容」的前一個名稱）。

   ![](assets/three.png)

1. 要選擇一個或多個類別，請按一下 **類別** 下拉框，進行選擇，然後按一下 **應用**。

   ![](assets/four.png)

   >[!NOTE]
   >
   >選擇特定類別或更改預測佈局是可選的。

1. 您的影像現在具有預測性。 對其他影像重複步驟3和4（如果需要）。

   ![](assets/five.png)

1. 要預覽電子郵件，請按一下 **預覽** 在右上角。

   ![](assets/six.png)

1. 要查看不同的可能影像，請按一下 **刷新**。

   ![](assets/seven.png)

   >[!NOTE]
   >
   >未選擇影像 **_直到收件人開啟電子郵件_**。 所以你在預覽中看到的只是一個例子，不一定是收件人看到的影像。

1. 預覽完電子郵件後，按一下 **預覽操作** 下拉並選擇 **批准和關閉**。 或者，如果仍需編輯，請按一下 **編輯草稿** 右邊。

   ![](assets/eight.png)

   >[!NOTE]
   >
   >發送樣本時，將選擇隨機影像。

在您批准您的電子郵件後，它將配備預測性內容並準備發送！

>[!CAUTION]
>
>收件人開啟電子郵件後，預測性影像將被鎖定。 如果稍後刪除內容，則收件人將看到內容所在的損壞影像。

## 不使用E-mail 2.0編輯器時添加預測性內容 {#adding-predictive-content-when-not-using-the-email-editor}

如果不使用 [電子郵件2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md){target=&quot;_blank&quot;}模板，只需將模板中的影像標籤為Marketo可編輯的影像元素即可將預測內容添加到電子郵件中。

瞭解 [Marketo語法](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md#elements){target=&quot;_blank&quot;}。

下面是代碼應顯示的示例（這只是一個示例，不要完全複製下面的代碼）。

**示例**

```example
<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com">  
<a><img style="border:10px solid red;"></a>  
</div>
```
