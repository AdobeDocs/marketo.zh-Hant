---
unique-page-id: 15695874
description: 將BrightTALK連接至Marketo - Marketo Docs —— 產品檔案
title: 將BrightTALK連接至Marketo
translation-type: tm+mt
source-git-commit: 23428a6e0ba9b2108a8f2f7dd6a69929dd069834
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---


# 將BrightTALK連接至Marketo {#connect-brighttalk-to-marketo}

瞭解如何將您的BrightTALK頻道連接至您的Marketo實例。 若要這麼做，您必須同時為兩者的管理員。

>[!NOTE]
>
>**需要管理員權限**

## BrightTALK中的步驟 {#steps-in-brighttalk}

1. 登入business.brighttalk.com/demandcentral，然 [後按](http://business.brighttalk.com/demandcentral/login) 「立即 **連線」**。
1. 在「進階行銷連接器」下方，按一下「 **連線**」。
1. 您將進入認證畫面，要求：用戶端ID、用戶端密碼、身分服務URL和余留服務URL。 若要取得此資訊，請登入Marketo。

## Marketo中的步驟 {#steps-in-marketo}

>[!NOTE]
>
>此時，您必須設定「僅限API使用者角色」和「API使用者」，以限制BrightTALK在您的Marketo例項中擁有的權限。 因為我們已經有這些步驟的文章，所以我們會將您連結到這些步驟。

1. 建立僅 [限API的使用者角色](http://docs.marketo.com/x/iwMk)。
1. [使用您在步驟](http://docs.marketo.com/x/jwMk)4中建立的BrightTALK API角色，建立API使用者。
1. 返回「管理員」區域。

   ![](assets/one.png)

1. 在「整合」下方，按一 **下LaunchPoint**。

   ![](assets/two.png)

1. 按一下「 **新** 」下拉式清單，然後選 **取「新服務」**。

   ![](assets/three.png)

1. 輸入您選擇的顯示名稱。 按一下「服務」下拉式清單並選 **擇「自定義** 」( **不選擇** 「BrightTALK」)。

   ![](assets/four.png)

   >[!CAUTION]
   >
   >切記不要在下拉式清單中選取BrightTALK。 我們正在移除此欄位，而選取此欄位可能會對您的Marketo/BrightTALK整合造成重大問題。

1. 輸入您選擇的說明。 按一下「僅API使用者」下拉式清單，然後選取您在步驟5中建立的BrightTALK API使用者。 按一下 **建立**。

   ![](assets/five.png)

1. 按一 **下您剛建立之自訂服務的「檢視詳細資訊** 」。

   ![](assets/six.png)

1. 複製（並儲存） **用戶端ID****和用戶端密碼**。 按一下 **關閉**。

   ![](assets/eight-1.png)

1. 在「整合」下，選 **取「網站服務」**。

   ![](assets/nine-1.png)

1. 在「Rest API」下，複製（並儲存） **端點****和Identity**。

   ![](assets/ten.png)

## BrightTALK中的步驟 {#steps-in-brighttalk-1}

1. 從步驟3返回BrightTALK連接器設定螢幕，並輸入從步驟12和14保存的憑據。

   認證完成後，您已正式將BrightTALK連線至Marketo。 下一步是決定 [您要同步的資料欄位](http://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync)。

