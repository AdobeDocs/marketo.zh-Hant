---
title: 瞭解my-token
description: 瞭解我的預付碼
exl-id: d56748e2-d742-45dd-96a8-dd80e30d9d8b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# 瞭解我的預付碼

<br> 

我的Token是自訂變數，您可以在程式或促銷活動資料夾中建立和使用。 它們看起來像這樣：`{{_my.Name of Token_}}`

## 範例

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

若要存取並建立我的Token，請選取您的程式或促銷活動資料夾，然後前往[!UICONTROL My Tokens]標籤。 將任何Token拖放至您的[!UICONTROL Local Tokens]畫布。

![影像一](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-1.png)

>[!CAUTION]
>
>儲存代號後無法變更其名稱，請謹慎選擇。

>[!NOTE]
>
>在Microsoft Dynamics或Salesforce上，從Sales Insight傳送電子郵件時，My Token無法解析；只會填入標準Token（銷售機會、公司等）。 不過，預付碼的預設值會運作。

>[!NOTE]
>
>連結Token無法在純文字電子郵件中運作。

## 巢狀代號

當您建立新的Token時，樹狀結構中的其他物件可參照它。 您可以在樹狀結構的較低層級覆寫全域變數。 Token的建立位置有命名結構，以方便管理。

* **本機Token:** Token是直接在程式或資料夾中建立。
* **[已覆寫的Token:](/help/sky/override-an-inherited-my-token.md)** 此Token已繼承，但在此程式或資料夾中發生異常。
* **繼承的Token:** Token是在較高層級程式或資料夾的樹狀結構中建立。

您可以在方案或促銷活動資料夾的&#x200B;**[!UICONTROL My Tokens]**&#x200B;標籤下找到這三種類型。

![影像2](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-2.png)

移動程式和資料夾也會影響Token。 請務必檢查，以確定在移動期間參照未損壞。

>[!NOTE]
>
>如果從參與方案傳送的電子郵件是預設方案的子電子郵件（即，非您的參與方案的本機），則電子郵件中使用的任何My Token都會從子電子郵件所在的預設程式中解析。

## 代號使用

選取任何Token，然後按一下右上角的使用圖示，即可查看包含該Token的資產清單。

![影像三](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-3.png)

![影像4](/help/sky/assets/my-tokens/understanding-my-tokens/understanding-my-tokens-4.png)

**深入探討**

進一步瞭解每個My Token:

* [CRM促銷活動](/help/sky/my-token-crm-campaign.md)
* [日期](/help/sky/my-token-date.md)
* [日曆檔案](/help/sky/my-token-calendar-file.md)
* [影像](/help/sky/my-token-image.md)
* [連結](/help/sky/my-token-link.md)
* [數字](/help/sky/my-token-number.md)
* [Rich Text](/help/sky/my-token-rich-text.md)
* [分數](/help/sky/my-token-score.md)
* [電子郵件指令碼](/help/sky/my-token-email-script.md)
* [文字](/help/sky/my-token-text.md)
