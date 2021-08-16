---
title: Omogućivanje programa Microsoft Defender za Office 365 za SharePoint Online, OneDrive i Microsoft Teams
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
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058858"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogućivanje programa Microsoft Defender za Office 365 za SharePoint Online, OneDrive i Microsoft Teams

1. Pomoću vjerodajnica globalnog administratora ili sigurnosnih administratora prijavite se u [centar za Office 365 sigurnost i usklađenost](https://protection.office.com/).
2. U **lijevom oknu** odaberite Upravljanje prijetnjama, a zatim **Pravilnik Sef**  >  [privitke](https://protection.office.com/safeattachment).
3. Odaberite **Uključi Microsoft Defender za Office 365 za SharePoint, OneDrive i Microsoft Teams** pa odaberite **Spremi**.
    > [!TIP]
    >
    > - Kao globalni administrator ili administrator SharePoint online pokrenite sljedeći cmdlet komponente PowerShell s parametrom **DisallowInfectedFileDownload** postavljenim na *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Postavljanje upozorenja za otkrivene datoteke](https://go.microsoft.com/fwlink/?linkid=2092110)

Dodatne informacije potražite u članku [Microsoft Defender Office 365 za SharePoint, OneDrive i Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
