---
unique-page-id: 11385020
description: 啟用電子郵件中的預測性內容 — Marketo檔案 — 產品檔案
title: 啟用電子郵件中的預測內容
exl-id: 7eaefee1-23e8-47ee-afff-adcf49096aa7
source-git-commit: 4b1b91a933a7a6d103fe0d44ece9ea95759edc5f
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# 啟用電子郵件中的預測內容 {#enable-predictive-content-in-emails}

在電子郵件中建立一或多個影像預測性，為每個收件者量身打造體驗。

>[!NOTE]
>
>建議您在測試和使用預測內容之前，先為每個類別和每個來源（電子郵件、多媒體、長條）啟用超過5個內容片段。 更多內容可讓您獲得更好的預測結果。

>[!PREREQUISITES]
>
>啟用預測內容之前，您必須：
>
>* **準備預測內容**
   >
   >   * [編輯電子郵件的預測內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-emails.md){target=&quot;_blank&quot;}或
   >   * [編輯多媒體的預測內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-rich-media.md){target=&quot;_blank&quot;}或
   >   * [編輯建議列的預測內容](/help/marketo/product-docs/predictive-content/working-with-predictive-content/edit-predictive-content-for-the-recommendation-bar.md){target=&quot;_blank&quot;}
>
>* [核准預測內容的標題](/help/marketo/product-docs/predictive-content/working-with-all-content/approve-a-title-for-predictive-content.md){target=&quot;_blank&quot;}


## 使用電子郵件2.0編輯器新增預測內容 {#adding-predictive-content-using-the-email-editor}

1. 按一下 **行銷活動**.

   ![](assets/one.png)

1. 選取您的電子郵件，然後按一下 **編輯草稿**.

   ![](assets/two.png)

1. 按一下您要預測的影像。 出現齒輪表徵圖時，按一下它並選取 **啟用ContentAI** （ContentAI是「預測內容」的前一個名稱）。

   ![](assets/three.png)

1. 若要選取一或多個類別，請按一下 **類別** 下拉式清單中，選取項目，然後按一下 **套用**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >選擇特定類別或變更預測配置為選用。

1. 您的影像現在可預測。 對其他影像重複步驟3和4（如果需要）。

   ![](assets/five.png)

1. 若要預覽電子郵件，請按一下 **預覽** 在右上角。

   ![](assets/six.png)

1. 要查看不同的可能影像，請按一下 **重新整理**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >未選擇影像 **_直到收件者開啟電子郵件_**. 因此，您在預覽中看到的只是一個範例，不一定是收件者看到的影像。

1. 預覽完電子郵件後，按一下 **預覽動作** 下拉式清單並選取 **核准並關閉**. 或者，如果您仍需要編輯，請按一下 **編輯草稿** 在右邊。

   ![](assets/eight.png)

   >[!NOTE]
   >
   >傳送範例時，會選取隨機影像。

您核准電子郵件後，電子郵件就會具備預測性內容，且可供傳送！

>[!CAUTION]
>
>收件者開啟電子郵件後，就會鎖定預測影像。 如果稍後移除內容，收件者會看到內容所在的影像損毀。

## 不使用電子郵件2.0編輯器時新增預測內容 {#adding-predictive-content-when-not-using-the-email-editor}

如果您沒有使用 [電子郵件2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md){target=&quot;_blank&quot;}範本，只要將範本中的影像標籤為Marketo可編輯的影像元素，即可將「預測內容」新增至電子郵件。

了解 [Marketo特定語法於此處](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md#elements){target=&quot;_blank&quot;}。

以下是程式碼看起來的範例（這只是範例，請勿精確複製下方的程式碼）。

**範例**

```example
<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com">  
<a><img style="border:10px solid red;"></a>  
</div>
```
