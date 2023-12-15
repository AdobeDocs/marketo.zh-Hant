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

1. 前往Marketo **[!UICONTROL 管理員]**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. 前往 **[!UICONTROL 啟動點]**，按一下 **[!UICONTROL 新增]** 並選取 **[!UICONTROL 新服務]**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. 輸入 **[!UICONTROL 顯示名稱]** ，並選取 **[!UICONTROL facebook自訂對象]** 來自的服務 **[!UICONTROL 服務]** 下拉式清單。

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. 在相同的瀏覽器中開啟新標籤，並前往 [facebook.com](https://www.facebook.com/){target="_blank"}. 使用您要用於整合的帳戶登入Facebook。

   >[!CAUTION]
   >
   >為了讓Marketo可跨多個Ad Manager帳戶傳送受眾，您在以下步驟中授權的Facebook使用者需要擁有存取權 *全部* 這些帳戶中的一個。

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. 登入Facebook後，請返回Marketo。 按一下 **[!UICONTROL 授權]**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >您 _必須_ 使用Facebook Business Manager帳戶，讓您的自訂對象整合發揮作用。 若要瞭解如何設定Business Manager帳戶，請參閱 [facebook說明](https://www.facebook.com/business/help/1710077379203657){target="_blank"}.

1. 如果出現提示，請按一下 **[!UICONTROL 確定]** 接受Marketo應用程式安裝至Facebook的方式。

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. 您現在已獲得授權！ 選取相符模式並按一下 **[!UICONTROL 建立]**.

   >[!NOTE]
   >
   >**基本比對** 僅使用電子郵件地址。 **進階比對** 會使用七個其他欄位，這會增加匹配率，以獲得更多轉換。 但是，如果貴公司的隱私權政策不允許共用其他欄位，或您的資料不包含這些欄位，請選取「基本比對」。

   ![](assets/fb-custom-adv-matching-hands.png)

   做得好！您現在可以前往Marketo中的任何靜態或智慧清單，並將受眾資料傳送至Facebook。

   >[!CAUTION]
   >
   >噢，開始之前，請務必 [接受Facebook的自訂對象條款](https://www.facebook.com/ads/manage/customaudiences/tos.php){target="_blank"} 在您的Facebook帳戶內！ 若未這麼做，對象更新將會失敗。

>[!MORELIKETHIS]
>
>* [在Facebook中建立自訂對象](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md){target="_blank"}
>
>* [設定Facebook銷售機會廣告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md){target="_blank"}
