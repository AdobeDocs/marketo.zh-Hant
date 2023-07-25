---
unique-page-id: 4720257
description: 將Facebook自訂對象新增為LaunchPoint服務 — Marketo檔案 — 產品檔案
title: 將Facebook自訂對象新增為LaunchPoint服務
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---

# 將Facebook自訂對象新增為LaunchPoint服務 {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**需要管理員許可權**

透過這項整合，您可以將受眾資料從Marketo靜態和智慧清單傳送至Facebook，在Facebook Ad Campaigns中作為自訂受眾。 以下說明設定方法。

1. 前往Marketo **管理員**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. 前往 **啟動點**，按一下 **新增** 並選取 **新服務**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. 輸入 **顯示名稱** ，並選取 **facebook自訂對象** 服務來自 **服務** 下拉式清單。

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. 在同一瀏覽器中開啟新標籤，然後前往 [facebook.com](https://www.facebook.com/). 使用您要用於整合的帳戶登入Facebook。

   >[!CAUTION]
   >
   >為了讓Marketo可跨多個廣告經理帳戶傳送對象，您於以下步驟中授權的Facebook使用者需要擁有以下存取許可權 *全部* 這些帳戶中的。

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. 登入Facebook後，請返回Marketo。 按一下 **授權**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >您 _必須_ 使用Facebook Business Manager帳戶，讓您的自訂對象整合發揮作用。 若要瞭解如何設定Business Manager帳戶，請參閱 [facebook說明](https://www.facebook.com/business/help/1710077379203657).

1. 如果出現提示，請按一下 **確定** 接受Marketo應用程式安裝至Facebook。

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. 您現在已獲得授權！ 選取相符模式並按一下 **建立**.

   >[!NOTE]
   >
   >**基本比對** 僅使用電子郵件地址。 **進階比對** 會額外使用七個欄位，以提高匹配率，以獲得更多轉換。 但是，如果貴公司的隱私權政策不允許共用其他欄位，或您的資料不包含這些欄位，請選取「基本比對」。

   ![](assets/fb-custom-adv-matching-hands.png)

   做得好！ 您現在可以前往Marketo中的任何靜態或智慧清單，並將受眾資料傳送至Facebook。

   >[!CAUTION]
   >
   >哦，開始之前，請務必 [接受Facebook的自訂對象條款](https://www.facebook.com/ads/manage/customaudiences/tos.php) 在您的Facebook帳戶內！ 若未這麼做，對象更新將會失敗。

>[!MORELIKETHIS]
>
>* [在Facebook中建立自訂對象](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
>
>* [設定Facebook銷售機會廣告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
