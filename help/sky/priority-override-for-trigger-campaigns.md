---
title: priority-override-for-trigger-campaigns
description: 觸發促銷活動的優先順序覆寫
exl-id: 4468868c-33d7-4b5e-b524-bfcc2785c8ce
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---

# 觸發促銷活動的優先順序覆寫

<br> 

管理員可以覆寫Marketo決定的優先順序，以觸發促銷活動，以設定更符合業務目標的優先順序。

>[!NOTE]
>
>此功能僅適用於觸發促銷活動，以及已授與「編輯觸發促銷活動優先順序」權限的使用者。

>[!CAUTION]
>
>強烈建議您在有限的關鍵業務促銷活動集上使用此功能（建議最大值為25）。 在大型群組上鬆散使用功能可能會對整體促銷活動執行造成負面影響。

## 覆寫優先順序

1. 在觸發器促銷活動中，按一下&#x200B;**[!UICONTROL Schedule]**&#x200B;標籤，然後按一下&#x200B;**[!UICONTROL Override Priority]**。

   ![影像一](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-1.png)

1. 從下拉式清單中選擇新的優先順序層級。 按一下&#x200B;**[!UICONTROL Confirm]**。

   ![影像2](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-2.png)

   ![影像三](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-3.png)

>[!NOTE]
>
>* 您可以在[!UICONTROL Marketing Activities]下方的[!UICONTROL Campaign Queue]中檢視促銷活動的預設優先順序。 若要提高執行率，建議您將促銷活動的優先順序設定為高於其預設值的層級。
>* 使用者設定的優先順序僅適用於符合促銷活動資格的新訪客；已在佇列中的人員將不會受到影響。


## 重設優先順序

1. 若要將促銷活動優先順序重設回系統預設值，請前往觸發促銷活動中的&#x200B;**[!UICONTROL Schedule]**&#x200B;標籤，然後按一下&#x200B;**[!UICONTROL Reset Priority]**。

   ![影像4](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-4.png)

1. 按一下&#x200B;**[!UICONTROL Reset]**&#x200B;進行確認。

   ![影像5](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-5.png)

>[!NOTE]
>
>優先順序覆寫和重設會在稽核記錄中擷取。 您可以透過Classic體驗的[!UICONTROL Admin]區域，檢視[稽核記錄](https://docs.marketo.com/x/GZ2t)。

## 授予優先順序覆蓋訪問權限

>[!CAUTION]
>
>只有具有管理責任的管理員或使用者才應擁有促銷活動優先順序覆寫存取權。

1. 在[!UICONTROL Admin]區域中，按一下&#x200B;**[!UICONTROL Users & Roles]**。

   ![影像6](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-6.png)

1. 按一下&#x200B;**[!UICONTROL Roles]**&#x200B;頁籤，選擇要授予訪問權限的用戶，然後按一下&#x200B;**[!UICONTROL Edit Role]**。

   ![影像7](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-7.png)

1. 在[!UICONTROL Access Marketing Activities]下，選中&#x200B;**[!UICONTROL Edit Trigger Campaign Priority]**。 按一下&#x200B;**[!UICONTROL Save]**。

   ![影像8](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-8.png)

## 在Marketo Classic檢視促銷活動優先順序

按一下觸發促銷活動中的&#x200B;**[!UICONTROL Schedule]**&#x200B;標籤，即可在[!DNL Classic]體驗中檢視促銷活動優先順序。

![影像9](/help/sky/assets/smart-campaigns/priority-override-for-trigger-campaigns/priority-override-for-trigger-campaigns-9.png)

>[!NOTE]
>
>[!DNL Classic]體驗的優先順序為僅檢視。 變更或重設促銷活動優先順序只能透過Marketo Sky。
