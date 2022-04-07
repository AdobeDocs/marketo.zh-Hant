---
unique-page-id: 11382815
description: MarketoIT Outlook插件安裝 — Marketo文檔 — 產品文檔
title: MarketoIT安裝Outlook插件
exl-id: c1ae1fb8-d1ad-4c1b-899b-29629fcb166b
source-git-commit: a24b0de6493d4849723099d6164fafb73ef7c926
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# MarketoIT安裝Outlook插件 {#marketo-outlook-plugin-installation-by-it}

有時，公司策略要求其IT團隊在員工的電腦上安裝所有軟體。 在這些情況下， IT經常使用自己的部署軟體遠程執行此操作。 本文檔提供了在部署過程中用作輸入的命令行，以遠程安裝outlook插件。

>[!PREREQUISITES]
>
>[設定](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-add-in-for-outlook-with-an-enterprise-key.md) 企業密鑰。

使用要安裝的/i開關以「系統」或「管理」用戶帳戶的形式運行以下命令行。

`<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**示例**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

要進行故障排除，您可以啟用日誌記錄以建立輸出日誌檔案。

`<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**示例**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

要指定日誌檔案的位置，可以在命令行中指定檔案路徑。

`<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**示例**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>日誌檔案的儲存位置必須存在，否則安裝將中止。

請參閱 [Microsoft交換機完整清單](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) 是否嘗試不同的日誌記錄級別或用戶介面級別。

>[!MORELIKETHIS]
>
>[MarketoIT卸載Outlook插件](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
