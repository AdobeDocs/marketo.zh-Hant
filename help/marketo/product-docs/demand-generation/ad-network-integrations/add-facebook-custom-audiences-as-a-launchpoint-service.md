---
unique-page-id: 4720257
description: 將Facebook自訂對象新增為LaunchPoint服務 — Marketo檔案 — 產品檔案
title: 將Facebook自訂對象新增為LaunchPoint服務
exl-id: 5c5b5c80-fd0f-482a-8163-6eef3dbcb236
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 0%

---

# 將Facebook自訂對象新增為LaunchPoint服務 {#add-facebook-custom-audiences-as-a-launchpoint-service}

>[!NOTE]
>
>**需要管理權限**

透過此整合，您可以將受眾資料從Marketo靜態和智慧型清單傳送至Facebook，以在Facebook廣告行銷活動中作為自訂受眾。 下面是如何設定它。

1. 前往Marketo **管理**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. 前往 **LaunchPoint**，按一下 **新增** 選取 **新服務**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. 輸入 **顯示名稱** 為您的服務，並選取 **Facebook自訂對象** 服務 **服務** 下拉式清單。

   ![](assets/image2016-11-29-12-3a51-3a8.png)

1. 在相同的瀏覽器中開啟新標籤，然後前往 [facebook.com](https://www.facebook.com/). 使用您要用於整合的帳戶登入Facebook。

   >[!CAUTION]
   >
   >為了讓Marketo跨多個廣告管理員帳戶傳送對象，您在下列步驟中授權的Facebook使用者必須擁有 *all* 這些賬戶。

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. 登入Facebook後，返回Marketo。 按一下 **授權**.

   ![](assets/fb-custom-authorize-hand.png)

   >[!NOTE]
   >
   >您 _必須_ 使用Facebook Business Manager帳戶，讓自訂對象整合運作正常。 要了解如何設定Business Manager帳戶，請參閱 [Facebook說明](https://www.facebook.com/business/help/1710077379203657).

1. 如果出現提示，請按一下 **確定** 接受Marketo應用程式安裝至Facebook。

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. 你現在被授權了！ 選取相符模式，然後按一下 **建立**.

   >[!NOTE]
   >
   >**基本比對** 僅使用電子郵件地址。 **進階比對** 使用另外7個欄位（這會增加匹配率）以進行更多轉換。 不過，如果貴公司的隱私權政策不允許共用其他欄位，或您的資料未包含這些欄位，請選取「基本比對」。

   ![](assets/fb-custom-adv-matching-hands.png)

   幹得好！ 您現在可以移至Marketo中的任何靜態或智慧清單，並將對象資料傳送至Facebook。

   >[!CAUTION]
   >
   >你走之前，一定要 [接受Facebook的自訂對象條款](https://www.facebook.com/ads/manage/customaudiences/tos.php) 在你的Facebook賬戶里！ 若不這麼做，對象更新將會失敗。

>[!MORELIKETHIS]
>
>* [在Facebook中建立自訂對象](/help/marketo/product-docs/demand-generation/facebook/create-a-custom-audience-in-facebook.md)
>
>* [設定Facebook銷售機會廣告](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)

