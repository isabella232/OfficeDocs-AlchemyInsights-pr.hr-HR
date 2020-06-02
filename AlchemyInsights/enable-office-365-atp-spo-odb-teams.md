---
title: Omogućivanje ATP-a sustava Office 365 za SharePoint, OneDrive i Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506910"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogućivanje napredne zaštite od prijetnji za Office 365 za SharePoint Online, OneDrive i Microsoft Teams

1. Idi https://protection.office.com i prijavite se.
2. Odaberite **Threat management**  >  **Sigurnost privitaka pravila upravljanja**prijetnjama  >  **Safe Attachments**.
3. Odaberite **Uključi ATP za SharePoint, OneDrive i Microsoft Teams**, a zatim kliknite **Spremi**.
4. (Preporučeno) Kao globalni administrator ili administrator sustava SharePoint Online pokrenite cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrom **DisallowInfectedFileDownload** postavljenim na *true*.
5. (Preporučeno) [Postavite upozorenja](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) za otkrivene datoteke.

> [!NOTE]
> ATP neće skenirati svaku datoteku u sustavima SharePoint Online, OneDrive ili Microsoft Teams. Datoteke se skeniraju asinkrono, kroz proces koji koristi događaje zajedničkog korištenja i aktivnosti gostiju, zajedno s pametnom heuristikom i signalima prijetnje za identifikaciju zlonamjernih datoteka. Pogledajte [ATP za SharePoint, OneDrive i Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).