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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801039"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogućivanje programa Microsoft Defender za Office 365 za SharePoint Online, OneDrive i Microsoftove timove

1. Idite na https://protection.office.com i prijavite se.
2. Odaberite **Threat management**  >  **Policy**  >  **sigurne privitke** pravilnika za upravljanje prijetnjama.
3. Odaberite **Uključi ATP za SharePoint, OneDrive i Microsoftove timove** , a zatim kliknite **Spremi** .
4. Preporučuje Kao globalni administrator ili administrator sustava SharePoint Online, pokrenite cmdlet [set-Spostanar](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) uz parametar **Disallowinfectedfiledownload** postavljen na *True* .
5. Preporučuje [Postavljanje upozorenja](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) za otkrivene datoteke.

> [!NOTE]
> ATP će nZa skenirati sve pojedinačne datoteke u sustavu SharePoint Online, OneDrive ili Microsoftovim timovima. Datoteke se skeniraju asinkrono, kroz postupak koji koristi zajedničko korištenje i događaje aktivnosti gosta, uz pametne heuristike i signale prijetnji za identifikaciju zlonamjernih datoteka. Pogledajte [ATP za SharePoint, OneDrive i Microsoftove timove](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).