---
title: Omogući Sef privitke za SharePoint online, OneDrive i Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7357f53ef7827aea9cbb0d222c338a5edf429ffd201bfbb6d7307b3d446fdae2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894455"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogući Sef privitke za SharePoint online, OneDrive i Microsoft Teams

1. Pomoću vjerodajnica globalnog administratora ili sigurnosnih administratora otvorite portal Microsoft 365 Defender na servisu , a zatim otvorite Pravilnik & pravila Prijetnje <https://security.microsoft.com>  \>  \> **Sef Privici** u **odjeljku Pravila**

   Da biste izravno na stranicu **Sef privitke,** koristite <https://security.microsoft.com/safeattachmentv2> .

2. Na **stranici Sef privici** kliknite **Globalne postavke**.
3. Na letak koji će se prikazati odaberite Uključi **Microsoft Defender za Office 365 za SharePoint, OneDrive i Microsoft Teams**, a zatim **Odaberite Spremi**.

    > [!TIP]
    >
    > Učinite sljedeće da biste poboljšali zaštitu Sef za SharePoint, OneDrive i Microsoft Teams:
    >
    > - Da biste korisnicima onemogućili preuzimanje zlonamjernih datoteka, koristite vrijednost parametra `$true` *DisallowInfectedFileDownload* na **[cmdletu Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** u web-aplikaciji SharePoint Online PowerShell. Dodatne informacije potražite u članku [Korištenje komponente SharePoint Online PowerShell da biste korisnicima onemogućili preuzimanje zlonamjernih datoteka](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files).
    > - [Stvaranje pravilnika upozorenja za otkrivene datoteke](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Dodatne informacije potražite u [članku Sef za Office 365 za SharePoint, OneDrive i Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
