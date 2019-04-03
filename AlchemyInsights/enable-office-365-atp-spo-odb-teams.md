---
title: Omogući ATP Office 365 za SharePoint, OneDrive i Microsoft timove
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/02/2019
ms.locfileid: "31030910"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Omogući zaštitu Office 365 napredne prijetnja za SharePoint na Internetu, OneDrive i Microsoft timove

1. Idi na https://protection.office.com i prijavite se.
2. Odaberite **prijetnja management** > **pravila** > **Sigurnom privitke**.
3. Odabir **uključiti ATP za SharePoint, OneDrive, i Microsoft timovima**i kliknite **Spremi**.
4. (Preporučeno) Kao globalni administrator ili SharePoint mrežni administrator, pokrenite cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrom **DisallowInfectedFileDownload** postavite na *true*.
5. (Preporučeno) [Postavljanje upozorenja](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) za otkriveni datoteke.

> [!NOTE]
> ATP će nU skeniranje svakih jednu datoteku u SharePoint Online, OneDrive ili Teams Microsoft. Datoteke su skenirane asinkrono, kroz proces koji koristi zajedničko korištenje i gosta aktivnost događaje, uz pametne heuristike i prijetnja signale za identifikaciju zlonamjernog datoteke. Pogledajte [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).