---
unique-page-id: 2359644
description: Show Custom HTML Form for Known People - Marketo Docs - Product Documentation
title: 顯示已知人員的自訂HTML表單
exl-id: 668216ea-7c2b-4204-81a5-56547c3baf1d
feature: Forms
source-git-commit: 55964499f5d49258539492f952513833af5692b5
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 1%

---

# 顯示已知人員的自訂HTML表單 {#show-custom-html-form-for-known-people}

If a visitor has provided their full name and email address in the past, and you don&#39;t want them to get the whole form, learn how to show them some custom HTML (e.g., just a download button).

1. Go to **Marketing Activities**.

   ![](assets/login-marketing-activities-5.png)

1. Under **Marketing Activities**, select your form and click **Edit Form**.

   ![](assets/image2014-9-15-12-3a24-3a6.png)

1. Under **Form Settings**, click on **Settings**.

   ![](assets/image2014-9-15-12-3a24-3a36.png)

1. Set If **Known Visitor, Show**: to **Custom HTML**.

   ![](assets/image2014-9-15-12-3a24-3a59.png)

1. Click the ![--](assets/image2014-9-25-14-3a1-3a26.png) to edit the **Custom HTML** that will be shown to known people.

   ![](assets/image2014-9-15-12-3a25-3a38.png)

1. There&#39;s some default content, but feel free to change it up.

   ![](assets/image2014-9-15-12-3a25-3a49.png)

   Available tokens:

   | Token | 說明 |
   |---|---|
   | `{{lead.FirstName}}` | This will display the person&#39;s first name. |
   | `{{lead.LastName}}` | This will display the person&#39;s last name. |
   | `{{form.Button:default=Download}}` | 這會顯示表單按鈕。 Replace the area after the `=` to change the button text. |
   | `{{form.NotYou:default=Not you?}}` | This will display a link in case the person is someone else. Replace the area after the `=` to change the link text. |

   >[!CAUTION]
   >
   >Only the four tokens above can be used. Any other token will not work here.

1. 按一下&#x200B;**完成**。

   ![](assets/image2014-9-15-12-3a27-3a25.png)

1. Click **Approve and Close**.

   >[!NOTE]
   >
   >The form must be approved to be used on landing pages.

   ![](assets/image2014-9-15-12-3a27-3a53.png)

   >[!NOTE]
   >
   >Remember to [approve the landing page draft](/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md) created by the form changes.

   Piece of cake! Check out what a person would see if they came back to the same form:

   ![](assets/image2014-9-15-12-3a28-3a12.png)

   >[!TIP]
   >
   >You can direct the click of the button to the asset by setting the form follow-up page to the file&#39;s URL.
