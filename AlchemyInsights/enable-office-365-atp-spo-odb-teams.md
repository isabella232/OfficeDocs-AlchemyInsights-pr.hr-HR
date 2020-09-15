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
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="2bed8-102">Omogućivanje napredne zaštite prijetnje u sustavu Office 365 za SharePoint Online, OneDrive i Microsoftove timove</span><span class="sxs-lookup"><span data-stu-id="2bed8-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="2bed8-103">Idite na https://protection.office.com i prijavite se.</span><span class="sxs-lookup"><span data-stu-id="2bed8-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="2bed8-104">Odaberite **Threat management**  >  **Policy**  >  **sigurne privitke**pravilnika za upravljanje prijetnjama.</span><span class="sxs-lookup"><span data-stu-id="2bed8-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="2bed8-105">Odaberite **Uključi ATP za SharePoint, OneDrive i Microsoftove timove**, a zatim kliknite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="2bed8-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="2bed8-106">Preporučuje Kao globalni administrator ili administrator sustava SharePoint Online, pokrenite cmdlet [set-Spostanar](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) uz parametar **Disallowinfectedfiledownload** postavljen na *True*.</span><span class="sxs-lookup"><span data-stu-id="2bed8-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="2bed8-107">Preporučuje [Postavljanje upozorenja](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) za otkrivene datoteke.</span><span class="sxs-lookup"><span data-stu-id="2bed8-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="2bed8-108">ATP će nZa skenirati sve pojedinačne datoteke u sustavu SharePoint Online, OneDrive ili Microsoftovim timovima.</span><span class="sxs-lookup"><span data-stu-id="2bed8-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="2bed8-109">Datoteke se skeniraju asinkrono, kroz postupak koji koristi zajedničko korištenje i događaje aktivnosti gosta, uz pametne heuristike i signale prijetnji za identifikaciju zlonamjernih datoteka.</span><span class="sxs-lookup"><span data-stu-id="2bed8-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="2bed8-110">Pogledajte [ATP za SharePoint, OneDrive i Microsoftove timove](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="2bed8-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>