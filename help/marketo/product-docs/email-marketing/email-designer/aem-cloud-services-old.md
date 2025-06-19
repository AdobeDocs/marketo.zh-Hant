---
title: 連線Experience Manager檔案
description: 瞭解如何將Adobe Experience Manager雲端服務連結至Adobe Marketo Engage，讓您能夠運用AEM資產。
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: bfa1bc900c2adc263e634a81440b77bef2976d3b
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# 連線Adobe Experience Manager雲端服務 {#connect-adobe-experience-manager-cloud-services}

瞭解如何將您的AEM Assets Cloud Services帳戶連結至Adobe Marketo Engage執行個體，以便在Marketo Engage電子郵件Designer中善用AEM資產存放庫。

>[!NOTE]
>
>**需要管理員許可權**

1. 在Marketo Engage中，移至&#x200B;**管理員**&#x200B;區域，然後在左側導覽樹狀結構中選取&#x200B;**Adobe Experience Manager**。

熒幕擷圖

1. 按一下&#x200B;_Adobe Experience Manager雲端服務_&#x200B;旁的&#x200B;**編輯**。

熒幕擷圖

1. 選取一或多個存放庫。

熒幕擷圖

>[!NOTE]
>
>系統只會列出與您的Marketo Engage訂閱在同一IMS組織中關聯的存放庫。

1. 您必須新增[服務認證憑證](https://experienceleague.adobe.com/zh-hant/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials)才能設定存放庫。 按一下&#x200B;**+新增憑證**&#x200B;按鈕。

熒幕擷圖

1. 拖放憑證（僅限JSON檔案），或從電腦中選取憑證。 完成時，按一下&#x200B;**新增**。

熒幕擷圖

1. 已設定的存放庫及其狀態和到期日會顯示於下方。 按一下省略符號按鈕(**...**)以檢視憑證。 否則，您就完成了。

熒幕擷圖

現在，您可以從Marketo Engage Email Designer存取該存放庫中數位資產管理資料庫的所有影像。

>[!MORELIKETHIS]
>
>[使用Experience Manager資產](/help/marketo/product-docs/email-marketing/email-designer/aem-assets.md)
