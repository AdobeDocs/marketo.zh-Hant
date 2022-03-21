---
description: 動態欄位 — Marketo文檔 — 產品文檔
title: 動態欄位
hide: true
hidefromtoc: true
source-git-commit: a0b10255513c13b7100b667513e3e61fc3788a15
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# 動態欄位 {#dynamic-fields}

我們允許您使用預定義的屬性(如 `{{first_name}}` 或 `{{company}}`。 通過這些欄位，您可以向多個聯繫人發送電子郵件並自動完成這些欄位，而無需為每個聯繫人單獨鍵入這些欄位。

>[!TIP]
>
>「first_name」和「company」欄位是Sales Insight Actions和Salesforce的唯一欄位。 這表示，如果 [Web應用](https://toutapp.com/login)，我們在Salesforce中查看我們是否可以找到具有匹配電子郵件地址的聯繫人/潛在顧客記錄。 然後，我們使用該記錄中的資訊填充該欄位。

## 將動態欄位插入模板 {#insert-a-dynamic-field-into-a-template}

1. 在 **模板和市場活動**，查找要編輯的模板，然後按一下 **編輯模板**。

1. 按一下 **插入動態欄位**。

   >[!NOTE]
   >
   >在通過電子郵件發送Sales Insight Actions中存在的聯繫人時，您可以使用基本的動態欄位。 這些將直接從聯繫人處拉出。

如果您正在向Salesforce中存在的聯繫人發送電子郵件，則可以利用Salesforce動態欄位。 這些都以&quot;sfdc&quot;開頭。 只要您與Salesforce有連接，這些欄位將直接呼叫Salesforce中的潛在客戶/聯繫人，以填充模板中的資訊。

## 在主題行中插入動態欄位 {#insert-dynamic-fields-in-a-subject-line}

只需手動將它們複製並貼上到電子郵件的主題欄位中，並要小心確保您具有正確的格式。

## 動態欄位辭彙表 {#dynamic-fields-glossary}

在Sales Insight Actions中建立模板時，我們始終建議使用 **插入動態欄位** 按鈕

此工具用於 `auto-personalize your email` 並節省大量時間 `pulling information from the People page`。

| 動態欄位 | 電子郵件中顯示的示例 |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | 基思 |
| `{{friendly_unsubscribe}}` | 如果你不想再聽我的，請告訴我 |
| `{{my_name}}` | 艾倫·布拉德利 |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | 高級技術撰稿人 |
| `{{work_website}}` | https://www.marketo.com |

**要注意的事項**:

* 如果聯繫人的資訊輸入不正確或在「人員」頁中丟失，則無法正確將其拉入模板。
* 兩者之差 `{{company}}` 和 `{{company_friendly}}` 是 `{{company_friendly}}` 將從您聯繫人的公司名稱中刪除任何正式標題，如Inc., LLC等。
* 使用時 `{{company_friendly}}`，確保在聯繫人詳細資訊中用逗號分隔Inc.或Co。。 這就是Sales Insight Actions在提取值時知道要刪除什麼的方法。
* 我們允許您使用預定義的屬性(如 `{{my_name}}` 或 `{{my_title}}`。 這些欄位允許您在電子郵件模板中快速引用自己。

>[!TIP]
>
>如果未填充動態欄位，請簽出 [這篇文章](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md)。
