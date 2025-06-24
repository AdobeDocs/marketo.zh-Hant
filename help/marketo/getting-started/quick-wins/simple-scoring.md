---
unique-page-id: 2359414
description: 簡單評分 — Marketo檔案 — 產品檔案
title: 簡單分數
exl-id: 6129d46a-e6d2-4819-9b6c-ccbf37060712
feature: Getting Started
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---

# 簡單分數 {#simple-scoring}

>[!PREREQUISITES]
>
>* [設定並新增人員](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [含有表單的登陸頁面](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## 步驟1：建立評分行銷活動 {#step-create-a-scoring-campaign}

1. 移至&#x200B;**[!UICONTROL Marketing Activities]**&#x200B;區域。

   ![](assets/simple-scoring-1.png)

1. 用滑鼠右鍵按一下您的&#x200B;**學習**&#x200B;資料夾，然後按一下&#x200B;**[!UICONTROL New Campaign Folder]**。

   ![](assets/simple-scoring-2.png)

1. 將行銷活動資料夾命名為「評分」，然後按一下&#x200B;**[!UICONTROL Create]**。

   ![](assets/simple-scoring-3.png)

   >[!NOTE]
   >
   >如果您已經有評分資料夾，請為這個資料夾命名不同的名稱，例如評分1。 資料夾名稱必須是唯一的。

1. 用滑鼠右鍵按一下您的&#x200B;**評分**&#x200B;資料夾，然後選取&#x200B;**[!UICONTROL New Smart Campaign]**。

   ![](assets/simple-scoring-4.png)

1. 將行銷活動命名為「Change Score」，然後按一下&#x200B;**[!UICONTROL Create]**。

   ![](assets/simple-scoring-5.png)

1. 按一下「**[!UICONTROL Smart List]**」標籤。

   ![](assets/simple-scoring-6.png)

   我們希望每當有人填寫您的&#x200B;**試用申請表單**&#x200B;時，就會執行此行銷活動。

1. 尋找&#x200B;**[!UICONTROL Fills Out Form]**&#x200B;觸發程式並將其拖曳至左側畫布。

   ![](assets/simple-scoring-7.png)

1. 選取&#x200B;**我的表單**。

   ![](assets/simple-scoring-8.png)

   >[!NOTE]
   >
   >如果您以表單[&#128279;](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}快速成功完成登陸頁面，您應該有表單。 如果您的表單使用不同的名稱，請選取該名稱。

1. 按一下「**[!UICONTROL Flow]**」標籤。

   ![](assets/simple-scoring-9.png)

1. 將&#x200B;**[!UICONTROL Change Score]**&#x200B;流程動作拖曳至左側畫布。

   ![](assets/simple-scoring-10.png)

1. 您可以輸入任何值以新增至人員分數。 讓我們在&#x200B;**[!UICONTROL Change]**&#x200B;欄位中輸入&quot;+5&quot;。

   ![](assets/simple-scoring-11.png)

   >[!TIP]
   >
   >良好的評分行銷活動是為銷售人員提供高品質人員的關鍵。 閱讀&#x200B;[**引導評分的最終指南**](https://www.marketo.com/definitive-guides/lead-scoring/){target="_blank"}。

1. 按一下「**[!UICONTROL Schedule]**」標籤與「**[!UICONTROL Activate]**」按鈕。

   ![](assets/simple-scoring-12.png)

1. 按一下確認畫面上的&#x200B;**[!UICONTROL Activate]**。

   ![](assets/simple-scoring-13.png)

>[!NOTE]
>
>一旦啟用，此行銷活動就會在每次有人填寫表單時執行。 行銷活動將持續執行直到其停用。

## 步驟2：填寫表單 {#step-fill-out-the-form}

1. 選取您在[登陸頁面（含表單](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}快速入門）中建立的登陸頁面。

   ![](assets/simple-scoring-14.png)

1. 按一下&#x200B;**[!UICONTROL Preview]**。 登入頁面將在新標籤中開啟。

   ![](assets/simple-scoring-15.png)

1. 填寫您的名字、姓氏和電子郵件地址，然後按一下&#x200B;**[!UICONTROL Submit]**。

   ![](assets/simple-scoring-16.png)

   >[!NOTE]
   >
   >請使用您第一次以個人身份輸入時使用的相同名稱和電子郵件地址，以套用「+5」分數增加。

## 步驟3：檢視人員資訊 {#step-view-the-person-info}

1. 移至&#x200B;**[!UICONTROL Database]**&#x200B;區域。

   ![](assets/simple-scoring-17.png)

1. 搜尋您在填寫表單時使用的電子郵件地址。

   ![](assets/simple-scoring-18.png)

1. 連按兩下您的人員。

   ![](assets/simple-scoring-19.png)

您的人員詳細資料將在新標籤或視窗中開啟。 看看您的分數在填寫表單時如何增加5分？

![](assets/simple-scoring-20.png)

## 任務完成！ {#mission-complete}

<br> 

[◄任務2：含表單的登陸頁面](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

[任務4：電子郵件自動回應►](/help/marketo/getting-started/quick-wins/email-auto-response.md)
