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
ms.openlocfilehash: 61ca448ef146f3f6fb930f0dc6f09f41bde72087f56ffba820f0a2d517cddb31
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53964625"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogućivanje programa Microsoft Defender za Office 365 za SharePoint Online, OneDrive i Microsoft Teams

1. Idite https://protection.office.com na i prijavite se.
2. Odaberite **Pravilnik upravljanja**  >    >  **prijetnjama Sef Privici**.
3. Odaberite **Uključi Defender za Office 365 za SharePoint, OneDrive i Microsoft Teams**, a zatim kliknite **Spremi**.
4. (Preporučeno) Kao globalni administrator ili administrator SharePoint online pokrenite [cmdlet Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrom **DisallowInfectedFileDownload** postavljenim na *true*.
5. (Preporučeno) [Postavite upozorenja za otkrivene](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) datoteke.

> [!NOTE]
> Microsoft Defender za Office 365 neće skenirati svaku pojedinačnu datoteku u web-aplikaciji SharePoint Online, OneDrive ili Microsoft Teams. Datoteke se asinkrono skeniraju putem postupka koji koristi događaje zajedničkog korištenja i aktivnosti gostiju, kao i pametne heurističare i signale prijetnji za prepoznavanje zlonamjernih datoteka. Pogledajte [Microsoft Defender za Office 365 za SharePoint, OneDrive i Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).