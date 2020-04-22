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
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703418"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogućivanje napredne zaštite od prijetnji sustava Office 365 za SharePoint Online, OneDrive i Microsoft Teams

1. Idi https://protection.office.com i prijavi se.
2. Odaberite**Sigurni privici****pravila** >  **upravljanja** > prijetnjama .
3. Odaberite **Uključi ATP za SharePoint, OneDrive i Microsoft Teams**, a zatim kliknite **Spremi**.
4. (Preporučeno) Kao globalni administrator ili administrator sustava SharePoint Online pokrenite cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrom **DisallowInfectedFileDownload** postavljenim na *true*.
5. (Preporučeno) [Postavite upozorenja](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) za otkrivene datoteke.

> [!NOTE]
> ATP neće skenirati svaku datoteku u sustavima SharePoint Online, OneDrive ili Microsoft Teams. Datoteke se skeniraju asinkrono, kroz proces koji koristi događaje zajedničkog korištenja i aktivnosti gostiju, zajedno s pametnom heuristikom i signalima prijetnji za identifikaciju zlonamjernih datoteka. Vidiљ. [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)