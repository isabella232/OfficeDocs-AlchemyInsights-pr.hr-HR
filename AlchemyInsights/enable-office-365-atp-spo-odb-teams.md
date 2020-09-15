---
title: Omogućivanje sustava Office 365 ATP za SharePoint, OneDrive i Microsoftove timove
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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709899"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogućivanje napredne zaštite prijetnje u sustavu Office 365 za SharePoint Online, OneDrive i Microsoftove timove

1. Idite na https://protection.office.com i prijavite se.
2. Odaberite **Threat management**  >  **Policy**  >  **sigurne privitke**pravilnika za upravljanje prijetnjama.
3. Odaberite **Uključi ATP za SharePoint, OneDrive i Microsoftove timove**, a zatim kliknite **Spremi**.
4. Preporučuje Kao globalni administrator ili administrator sustava SharePoint Online, pokrenite cmdlet [set-Spostanar](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) uz parametar **Disallowinfectedfiledownload** postavljen na *True*.
5. Preporučuje [Postavljanje upozorenja](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) za otkrivene datoteke.

> [!NOTE]
> ATP će nZa skenirati sve pojedinačne datoteke u sustavu SharePoint Online, OneDrive ili Microsoftovim timovima. Datoteke se skeniraju asinkrono, kroz postupak koji koristi zajedničko korištenje i događaje aktivnosti gosta, uz pametne heuristike i signale prijetnji za identifikaciju zlonamjernih datoteka. Pogledajte [ATP za SharePoint, OneDrive i Microsoftove timove](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).