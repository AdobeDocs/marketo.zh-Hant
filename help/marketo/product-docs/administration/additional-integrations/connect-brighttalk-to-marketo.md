---
unique-page-id: 15695874
description: 將BrightTALK連接到Marketo-Marketo文檔——產品文檔
title: 將BrightTALK連接到Marketo
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# 將BrightTALK連接到Marketo{#connect-brighttalk-to-marketo}

瞭解如何將您的BrightTALK頻道連接至您的Marketo實例。 若要這麼做，您必須同時為兩者的管理員。

>[!NOTE]
>
>**需要管理員權限**

## BrightTALK {#steps-in-brighttalk}中的步驟

1. 登入[business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login)，然後按一下&#x200B;**立即連線**。
1. 在「高級Marketo連接器」下，按一下「連接」。****
1. 您將進入認證畫面，要求：用戶端ID、用戶端密碼、身分服務URL和余留服務URL。 若要取得這項資訊，請登入Marketo。

## Marketo步驟{#steps-in-marketo}

>[!NOTE]
>
>此時，您必須設定「僅限API使用者角色」和「API使用者」，以限制BrightTALK在您的Marketo實例中擁有的權限。 因為我們已經有這些步驟的文章，所以我們會將您連結到這些步驟。

1. 建立[僅API用戶角色](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)。
1. [使用您在步驟](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)4中建立的BrightTALK API角色，建立API使用者。
1. 返回「管理員」區域。

   ![](assets/one.png)

1. 在「整合」下，按一下&#x200B;**LaunchPoint**。

   ![](assets/two.png)

1. 按一下&#x200B;**新建**&#x200B;下拉式清單並選擇&#x200B;**新建服務**。

   ![](assets/three.png)

1. 輸入您選擇的顯示名稱。 按一下「服務」下拉式清單並選擇「**自定義**」（_not_&#x200B;選擇「BrightTALK」）。

   ![](assets/four.png)

   >[!CAUTION]
   >
   >切記不要在下拉式清單中選取BrightTALK。 我們正在移除這個領域，而選擇它可能會對您的Marketo/BrightTALK整合造成重大問題。

1. 輸入您選擇的說明。 按一下「僅API使用者」下拉式清單，然後選取您在步驟5中建立的BrightTALK API使用者。 按一下&#x200B;**建立**。

   ![](assets/five.png)

1. 按一下&#x200B;**查看您剛建立的自定義服務的詳細資訊**。

   ![](assets/six.png)

1. 複製（並保存）**客戶端ID**&#x200B;和&#x200B;**客戶端密碼**。 按一下&#x200B;**關閉**。

   ![](assets/eight-1.png)

1. 在「整合」下，選擇&#x200B;**Web服務**。

   ![](assets/nine-1.png)

1. 在Rest API下，複製（並儲存）**Endpoint**&#x200B;和&#x200B;**Identity**。

   ![](assets/ten.png)

## BrightTALK {#additional-steps-in-brighttalk}中的其他步驟

1. 從步驟3返回BrightTALK連接器設定螢幕，並輸入從步驟12和14保存的憑據。

   認證完成後，您已正式將BrightTALK連接至Marketo。 下一步是確定要同步的[資料欄位。](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync)
