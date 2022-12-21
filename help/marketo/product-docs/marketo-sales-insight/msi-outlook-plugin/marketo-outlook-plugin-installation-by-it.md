---
unique-page-id: 11382815
description: Marketo Outlook外掛程式由IT安裝 — Marketo檔案 — 產品檔案
title: Marketo Outlook插件由IT安裝
exl-id: c1ae1fb8-d1ad-4c1b-899b-29629fcb166b
source-git-commit: a24b0de6493d4849723099d6164fafb73ef7c926
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# Marketo Outlook插件由IT安裝 {#marketo-outlook-plugin-installation-by-it}

有時，公司策略要求其IT團隊在員工的電腦上安裝所有軟體。 在這些情況下，IT通常使用自己的部署軟體遠程執行此操作。 本文檔提供在部署過程中用作輸入的命令行，以遠程安裝Outlook插件。

>[!PREREQUISITES]
>
>[設定](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/install-the-marketo-add-in-for-outlook-with-an-enterprise-key.md) 企業密鑰。

以「System」或具有要安裝的/i開關的管理用戶帳戶的形式運行以下命令行。

`<pre>msiexec.exe /i [File Name] /qn REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**範例**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn REG=ABC9-123y-WXYZ-4321</pre>`

若要進行疑難排解，您可以啟用記錄來建立輸出記錄檔。

`<pre>msiexec.exe /i [File Name] /qn /L*v MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**範例**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

要指定日誌檔案的位置，可以在命令行中指定檔案路徑。

`<pre>msiexec.exe /i [File Name] /qn /L*v [File Path]MarketoAddin.log REG=[Enterprise Key]</pre>`

>[!NOTE]
>
>**範例**
>
>`<pre>msiexec.exe /i MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddin.log REG=ABC9-123y-WXYZ-4321</pre>`

>[!CAUTION]
>
>日誌檔案的儲存位置必須存在，否則安裝將被中止。

請參閱 [Microsoft交換機的完整清單](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) 如果您想要嘗試不同的記錄層級或使用者介面層級。

>[!MORELIKETHIS]
>
>[Marketo Outlook外掛程式由IT卸載](/help/marketo/product-docs/marketo-sales-insight/msi-outlook-plugin/marketo-outlook-plugin-uninstall-by-it.md)
