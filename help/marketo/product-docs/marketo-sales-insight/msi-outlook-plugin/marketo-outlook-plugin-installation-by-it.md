---
unique-page-id: 11382815
description: Marketo [!DNL Outlook] IT安裝外掛程式 — Marketo檔案 — 產品檔案
title: 由IT安裝Marketo [!DNL Outlook] 外掛程式
exl-id: c1ae1fb8-d1ad-4c1b-899b-29629fcb166b
feature: Marketo Sales Insights
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 1%

---

# 由IT安裝Marketo [!DNL Outlook]外掛程式 {#marketo-outlook-plugin-installation-by-it}

有時公司政策會要求其IT團隊在員工的電腦上安裝所有軟體。 在這些情況下，IT通常會使用自己的部署軟體從遠端執行這項作業。 此檔案提供您在部署程式期間用來作為輸入以遠端安裝Outlook外掛程式的命令列。

>[!PREREQUISITES]
>
>[設定](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-add-in-for-outlook-with-an-enterprise-key.md)企業金鑰。

以&#39;System&#39;的身分或具有/i引數的「管理」使用者帳戶執行下列命令列，以進行安裝。

`<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**範例**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

若要進行疑難排解，您可以啟用記錄以建立輸出記錄檔。

`<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**範例**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

若要指定日誌檔的位置，您可以在命令列中指定檔案路徑。

`<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**範例**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>記錄檔的儲存位置必須存在，否則安裝將會中止。

如果您想要嘗試不同的記錄層級或使用者介面層級，請參閱[Microsoft的完整交換器清單](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6)。

>[!MORELIKETHIS]
>
>[Marketo [!DNL Outlook] IT解除安裝外掛程式](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
