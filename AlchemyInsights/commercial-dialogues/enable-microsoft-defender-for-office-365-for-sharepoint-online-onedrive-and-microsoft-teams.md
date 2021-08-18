---
title: Omogućivanje Sef privitaka za SharePoint online, OneDrive i Microsoft Teams
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
ms.openlocfilehash: 61372075ac8ccf04606a8003b4ec29f89fc048e5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332371"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogućivanje Sef privitaka za SharePoint online, OneDrive i Microsoft Teams

1. Pomoću vjerodajnica globalnog administratora ili sigurnosnog administratora otvorite portal Microsoft 365 Defender na servisu , a zatim idite na Pravila & Pravila <https://security.microsoft.com>  \>  \> **prijetnji Sef Privici** u **odjeljku Pravila**

   Da biste izravno na stranicu **Sef privitke,** koristite <https://security.microsoft.com/safeattachmentv2> .

2. Na **stranici Sef privici** kliknite **Globalne postavke**.
3. Na letak koji će se prikazati **odaberite Uključi Microsoft Defender za Office 365 za SharePoint, OneDrive i Microsoft Teams**, a zatim **Odaberite Spremi**.

    **Savjet**: Učinite sljedeće da biste poboljšali zaštitu Sef privitaka za SharePoint, OneDrive i Microsoft Teams:
    - Da biste korisnicima onemogućili preuzimanje zlonamjernih datoteka, koristite vrijednost parametra `$true` *DisallowInfectedFileDownload* na **[cmdletu Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** u web-aplikaciji SharePoint Online PowerShell. Dodatne informacije potražite u članku Korištenje [komponente SharePoint Online PowerShell da biste korisnicima onemogućili preuzimanje zlonamjernih datoteka](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files).
    - [Stvaranje pravilnika upozorenja za otkrivene datoteke](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Dodatne informacije potražite u [članku Sef za Office 365 za SharePoint, OneDrive i Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
