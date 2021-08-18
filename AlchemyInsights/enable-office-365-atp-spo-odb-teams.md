---
title: Omogućivanje Office 365 ATP za SharePoint, OneDrive i Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4a29fdf1b61dd51b85793a1346bea193c67f70d32344470cb5449cf767da4a24
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896595"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogućivanje programa Microsoft Defender Office 365 za SharePoint Online, OneDrive i Microsoft Teams

1. Idite https://protection.office.com na i prijavite se.
2. Odaberite **Pravilnik upravljanja**  >    >  **prijetnjama Sef Privici**.
3. Odaberite **Uključi Defender za Office 365 za SharePoint, OneDrive i Microsoft Teams**, a zatim kliknite **Spremi**.
4. (Preporučeno) Kao globalni administrator ili administrator SharePoint Online pokrenite [cmdlet Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrom **DisallowInfectedFileDownload** postavljenim na *true*.
5. (Preporučeno) [Postavite upozorenja za otkrivene](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) datoteke.

> [!NOTE]
> Microsoft Defender za Office 365 neće skenirati svaku pojedinačnu datoteku u web-aplikaciji SharePoint Online, OneDrive ili Microsoft Teams. Datoteke se asinkrono skeniraju putem postupka koji koristi događaje zajedničkog korištenja i aktivnosti gostiju, kao i pametne heurističare i signale prijetnji za prepoznavanje zlonamjernih datoteka. Pogledajte [Microsoft Defender za Office 365 za SharePoint, OneDrive i Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).