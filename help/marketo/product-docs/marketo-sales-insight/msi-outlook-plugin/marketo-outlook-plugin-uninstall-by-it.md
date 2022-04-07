---
unique-page-id: 11382829
description: MarketoOutlook插件由IT卸載 — Marketo文檔 — 產品文檔
title: MarketoIT卸載Outlook插件
exl-id: 678684da-3e99-462f-9950-504df1c1bb1e
source-git-commit: a24b0de6493d4849723099d6164fafb73ef7c926
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# MarketoIT卸載Outlook插件 {#marketo-outlook-plugin-uninstall-by-it}

下面是IT如何遠程卸載MarketoOutlook插件。

以「System」或「Administrative user account（管理用戶帳戶）」的形式運行以下命令行，並使用/x開關卸載。

`<pre>msiexec.exe /x [File Name] /qn </pre>`

>[!NOTE]
>
>**示例**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn </pre>`

要排除故障，您可以啟用日誌記錄以建立輸出日誌檔案。

`<pre>msiexec.exe /x [File Name] /qn /L*v MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**示例**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v MarketoAddinUninstall.log</pre>`

要指定日誌檔案的位置，可以在命令行中指定檔案路徑。

`<pre>msiexec.exe /x [File Name] /qn /L*v [File Path]MarketoAddinUninstall.log</pre>`

>[!NOTE]
>
>**示例**
>
>`<pre>msiexec.exe /x MarketoAddInSetup64.msi /qn /L*v C:\temp\MarketoAddinUninstall.log</pre>`

>[!CAUTION]
>
>遠程卸載插件將強制關閉用戶電腦上的Outlook。

請參考 [Microsoft交換機完整清單](https://support.microsoft.com/en-us/office/command-line-switches-for-microsoft-office-products-079164cd-4ef5-4178-b235-441737deb3a6) 是否嘗試不同的日誌記錄級別或用戶介面級別。
