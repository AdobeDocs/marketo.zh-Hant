---
solution: Marketo Engage
product: marketo
title: Spam刺客
description: 文字移至此處
level: Beginner, Intermediate
feature: Email Editor
hide: true
hidefromtoc: true
source-git-commit: 0157bc64444151a43bf464158d508e84d75b3427
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 3%

---

# Spam刺客 {#spam-assassin}

在Marketo Engage中使用SpamAssassin，您可以測試您的電子郵件內容，並檢視ISP/信箱提供者將其標示為垃圾郵件的可能性。

SpamAssassin會分析您的內容，並根據各種條件指派分數。 分數越低越好。請務必維持低分，因為傳送高分的電子郵件可能會對您的整體傳遞能力造成負面影響。

## 存取垃圾郵件報告 {#access-the-spam-report}

1. 在[模擬]畫面中，按一下&#x200B;**垃圾郵件報告**&#x200B;按鈕。

熒幕擷圖

1. 產生垃圾郵件報告。

熒幕擷圖

1. 檢查每個專案的分數和說明。

>[!IMPORTANT]
>
>如果整體分數高於5，您的電子郵件可能會在傳送時遭到封鎖或標示為垃圾郵件。

1. 如果您認為分數太高，請在電子郵件Designer中編輯您的內容，然後重新執行垃圾郵件報告，直到分數為您想要的位置。

熒幕擷圖

>[!NOTE]
>
>垃圾郵件分數透過SpamAssassin衍生，而規則不屬於Adobe。 有關這些規則的更多詳細資訊，請參閱[SpamAssassin檔案](https://spamassassin.apache.org/#_blank)。 您可在此看到[錯誤的完整清單](https://spamassassin.apache.org/old/tests_3_0_x.html?utm_source=chatgpt.com)。
