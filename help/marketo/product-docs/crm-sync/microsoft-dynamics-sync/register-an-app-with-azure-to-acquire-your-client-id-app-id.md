---
unique-page-id: 12983390
description: 向Azure註冊應用程式以取得您的用戶端ID/應用程式ID —— 行銷人員檔案——產品檔案
title: 向Azure註冊應用程式以取得您的用戶端ID/應用程式ID
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---


# 向Azure註冊應用程式以取得您的用戶端ID/應用程式ID {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory將您的內部目錄延伸至雲端，提供MS Dynamics 365 CRM的內部部署ADFS驗證支援。

## 註冊新應用程式{#registering-a-new-app}

1. [使用](https://manage.windowsazure.com/) 具有管理權限的帳戶登入Microsoft Azure管理入口網站。您也可以透過Office 365管理中心存取Microsoft Azure入口網站，方法是展開左側導覽窗格中的&#x200B;**Admin**&#x200B;項目，然後選取&#x200B;**Azure AD**。

   >[!CAUTION]
   >
   >您必須在同一份Office 365訂閱中使用您要向其註冊應用程式的帳戶。

   >[!NOTE]
   >
   >如果您沒有Azure帳戶，可以[註冊](https://azure.microsoft.com/en-us/free/)一個帳戶。 請參閱Microsoft的文檔或聯繫您的Microsoft代表以瞭解更多資訊。 在您建立Azure帳戶後，就可以使用下列程式註冊一或多個應用程式。
   >
   >
   >如果您有Azure帳戶，但Microsoft Dynamics 365的Office 365訂閱無法在Azure訂閱中使用，請依照[這些指示](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription)來關聯這兩個帳戶。

1. 在左側導覽窗格中，尋找並按一下「Azure Active Directory」(Azure Active Directory)。****

   ![](assets/two.png)

1. 在「管理」下，按一下「應用程式註冊&#x200B;**」。**

   ![](assets/three.png)

1. 按一下頁面頂部的&#x200B;**新建註冊**。

   ![](assets/four.png)

1. 輸入應用程式的名稱、選擇您適用的帳戶類型，然後輸入重新導向URL。 然後按一下頁面底部的&#x200B;**Register**。

   ![](assets/five.png)

1. 您現在應該會在&#x200B;**App registrations**&#x200B;標籤中看到您的應用程式。

   ![](assets/six.png)

## 設定應用程式權限{#configuring-app-permissions}

1. 在Active Directory的&#x200B;**App registations**&#x200B;標籤下，按一下您要設定權限的應用程式。

   ![](assets/seven.png)

1. 在「管理」下，按一下「**API權限**」。

   ![](assets/eight.png)

1. 按一下&#x200B;**添加權限**&#x200B;按鈕。

   ![](assets/nine.png)

1. 選擇&#x200B;**Dynamics CRM**。

   ![](assets/ten.png)

1. 選中「以組織用戶身份訪問公共資料服務」框****s **，然後按一下「添加權限」。******

   ![](assets/eleven.png)

1. 成功新增權限後，請至少等待10秒。

   ![](assets/twelve.png)

1. 按一下&#x200B;**授予管理員許可**&#x200B;按鈕。

   ![](assets/thirteen.png)

1. 按一下&#x200B;**是**&#x200B;確認。

   ![](assets/fourteen.png)

   你完了！

   ![](assets/fifteen.png)

