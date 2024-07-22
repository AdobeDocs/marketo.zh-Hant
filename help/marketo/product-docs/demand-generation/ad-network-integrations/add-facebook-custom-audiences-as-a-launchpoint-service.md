---
unique-page-id: 4720257
description: 將Facebook自訂對象新增為LaunchPoint Service - Marketo檔案 — 產品檔案
title: 將Facebook自訂對象新增為LaunchPoint Service
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# 將Facebook自訂對象新增為LaunchPoint Service {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**需要管理員許可權**

透過這項整合，您可以從Marketo Engage靜態與智慧列示傳送對象資料至Facebook，用作Facebook廣告促銷活動中的自訂對象。 以下說明設定方法。

1. 移至Marketo **[!UICONTROL 管理員]**。

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. 移至&#x200B;**[!UICONTROL LaunchPoint]**，按一下&#x200B;**[!UICONTROL 新增]**&#x200B;並選取&#x200B;**[!UICONTROL 新增服務]**。

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. 輸入您服務的&#x200B;**[!UICONTROL 顯示名稱]**，並從&#x200B;**[!UICONTROL 服務]**&#x200B;下拉式清單中選取&#x200B;**[!UICONTROL Facebook自訂對象]**&#x200B;服務。

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. 在相同的瀏覽器中開啟新分頁，並移至[facebook.com](https://www.facebook.com/){target="_blank"}。 使用您要用於整合的帳戶登入Facebook。

   >[!CAUTION]
   >
   >為了讓Marketo可以跨多個Ad Manager帳戶傳送受眾，您在以下步驟中授權的Facebook使用者需要擁有這些帳戶中&#x200B;*所有*&#x200B;的存取權。

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. 登入Facebook後，請返回Marketo。 按一下&#x200B;**[!UICONTROL 授權]**。

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >您&#x200B;_必須_&#x200B;使用Facebook Business Manager帳戶，您的自訂對象整合才能運作。 若要瞭解如何設定Business Manager帳戶，請參閱[Facebook說明](https://www.facebook.com/business/help/1710077379203657){target="_blank"}。

1. 如果出現提示，請按一下&#x200B;**[!UICONTROL 確定]**，接受將Marketo應用程式安裝到Facebook。

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. 您現在已獲得授權！ 選取相符模式，然後按一下&#x200B;**[!UICONTROL 建立]**。

   >[!NOTE]
   >
   >**基本比對**&#x200B;僅使用電子郵件地址。 **進階比對**&#x200B;使用七個額外的欄位，這會增加比對率，以獲得更多轉換。 但是，如果貴公司的隱私權政策不允許共用其他欄位，或您的資料不包含這些欄位，請選取「基本比對」。

   ![](assets/fb-custom-adv-matching-hands.png)

   做得好！您現在可以前往Marketo中的任何靜態或智慧清單，並將受眾資料傳送至Facebook。

   >[!CAUTION]
   >
   >噢，開始之前，請務必在您的Facebook帳戶中[接受Facebook的自訂對象條款](https://www.facebook.com/ads/manage/customaudiences/tos.php){target="_blank"}！ 若未這麼做，對象更新將會失敗。

>[!MORELIKETHIS]
>
>* [在Facebook中建立自訂對象](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md){target="_blank"}
>
>* [設定Facebook銷售機會廣告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md){target="_blank"}
