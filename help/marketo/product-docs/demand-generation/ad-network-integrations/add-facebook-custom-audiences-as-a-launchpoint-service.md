---
unique-page-id: 4720257
description: 新增 [!DNL Facebook] 自訂對象作為 [!DNL LaunchPoint] 服務 — Marketo檔案 — 產品檔案
title: 將 [!DNL Facebook] 自訂對象新增為 [!DNL LaunchPoint] 服務
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 1%

---

# 將[!DNL Facebook]個自訂對象新增為[!DNL LaunchPoint]服務 {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**需要管理員許可權**

透過這項整合，您可以從Marketo靜態與智慧列示傳送對象資料至[!DNL Facebook]，以在[!DNL Facebook]廣告行銷活動中作為自訂對象使用。 以下說明設定方法。

1. 前往Marketo **[!UICONTROL Admin]**。

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. 移至&#x200B;**[!UICONTROL LaunchPoint]**，按一下&#x200B;**[!UICONTROL New]**&#x200B;並選取&#x200B;**[!UICONTROL New Service]**。

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. 輸入您服務的&#x200B;**[!UICONTROL Display Name]**，然後從&#x200B;**[!UICONTROL Facebook Custom Audiences]**&#x200B;下拉式清單中選取&#x200B;**[!UICONTROL Service]**&#x200B;服務。

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. 在相同的瀏覽器中開啟新標籤，並移至[facebook.com](https://www.facebook.com/)。 使用您要用於整合的帳戶登入[!DNL Facebook]。

   >[!CAUTION]
   >
   >為了讓Marketo可跨多個廣告管理員帳戶傳送對象，您於下列步驟中授權的[!DNL Facebook]使用者必須擁有這些帳戶中&#x200B;*所有*&#x200B;的存取權。

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. 登入[!DNL Facebook]後，請返回Marketo。 按一下「**[!UICONTROL Authorize]**」。

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >您&#x200B;_必須_&#x200B;使用[!DNL Facebook] Business Manager帳戶，您的自訂對象整合才能運作。 若要瞭解如何設定Business Manager帳戶，請參閱[[!DNL Facebook] 說明](https://www.facebook.com/business/help/1710077379203657)。

1. 如果出現提示，請按一下&#x200B;**[!UICONTROL OK]**&#x200B;接受Marketo應用程式安裝到[!DNL Facebook]。

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. 您現在已獲得授權！ 選取相符模式並按一下&#x200B;**[!UICONTROL Create]**。

   >[!NOTE]
   >
   >**[!UICONTROL Basic Matching]**&#x200B;僅使用電子郵件地址。 **[!UICONTROL Advanced Matching]**&#x200B;使用七個額外的欄位，這會增加匹配率，以獲得更多轉換。 但是，如果貴公司的隱私權政策不允許共用其他欄位，或您的資料不包含這些欄位，請選取「[!UICONTROL Basic Matching]」。

   ![](assets/fb-custom-adv-matching-hands.png)

   做得好！您現在可以移至Marketo中的任何靜態或智慧清單，並將對象資料傳送至[!DNL Facebook]。

   >[!CAUTION]
   >
   >噢，開始之前，請務必在您的[帳戶中 [!DNL Facebook]接受](https://www.facebook.com/ads/manage/customaudiences/tos.php)的自訂對象條款[!DNL Facebook]！ 若未這麼做，對象更新將會失敗。

>[!MORELIKETHIS]
>
>* [在 [!DNL Facebook]](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)中建立自訂對象
>
>* [設定 [!DNL Facebook] 潛在客戶廣告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
