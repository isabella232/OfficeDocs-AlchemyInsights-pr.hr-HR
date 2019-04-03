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
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="24443-102">Omogući zaštitu Office 365 napredne prijetnja za SharePoint na Internetu, OneDrive i Microsoft timove</span><span class="sxs-lookup"><span data-stu-id="24443-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="24443-103">Idi na https://protection.office.com i prijavite se.</span><span class="sxs-lookup"><span data-stu-id="24443-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="24443-104">Odaberite **prijetnja management** > **pravila** > **Sigurnom privitke**.</span><span class="sxs-lookup"><span data-stu-id="24443-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="24443-105">Odabir **uključiti ATP za SharePoint, OneDrive, i Microsoft timovima**i kliknite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="24443-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="24443-106">(Preporučeno) Kao globalni administrator ili SharePoint mrežni administrator, pokrenite cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrom **DisallowInfectedFileDownload** postavite na *true*.</span><span class="sxs-lookup"><span data-stu-id="24443-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="24443-107">(Preporučeno) [Postavljanje upozorenja](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) za otkriveni datoteke.</span><span class="sxs-lookup"><span data-stu-id="24443-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="24443-108">ATP će nU skeniranje svakih jednu datoteku u SharePoint Online, OneDrive ili Teams Microsoft.</span><span class="sxs-lookup"><span data-stu-id="24443-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="24443-109">Datoteke su skenirane asinkrono, kroz proces koji koristi zajedničko korištenje i gosta aktivnost događaje, uz pametne heuristike i prijetnja signale za identifikaciju zlonamjernog datoteke.</span><span class="sxs-lookup"><span data-stu-id="24443-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="24443-110">Pogledajte [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="24443-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>