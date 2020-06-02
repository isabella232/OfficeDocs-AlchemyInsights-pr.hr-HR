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
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="945be-102">Omogućivanje napredne zaštite od prijetnji za Office 365 za SharePoint Online, OneDrive i Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="945be-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="945be-103">Idi https://protection.office.com i prijavite se.</span><span class="sxs-lookup"><span data-stu-id="945be-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="945be-104">Odaberite **Threat management**  >  **Sigurnost privitaka pravila upravljanja**prijetnjama  >  **Safe Attachments**.</span><span class="sxs-lookup"><span data-stu-id="945be-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="945be-105">Odaberite **Uključi ATP za SharePoint, OneDrive i Microsoft Teams**, a zatim kliknite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="945be-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="945be-106">(Preporučeno) Kao globalni administrator ili administrator sustava SharePoint Online pokrenite cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrom **DisallowInfectedFileDownload** postavljenim na *true*.</span><span class="sxs-lookup"><span data-stu-id="945be-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="945be-107">(Preporučeno) [Postavite upozorenja](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) za otkrivene datoteke.</span><span class="sxs-lookup"><span data-stu-id="945be-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="945be-108">ATP neće skenirati svaku datoteku u sustavima SharePoint Online, OneDrive ili Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="945be-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="945be-109">Datoteke se skeniraju asinkrono, kroz proces koji koristi događaje zajedničkog korištenja i aktivnosti gostiju, zajedno s pametnom heuristikom i signalima prijetnje za identifikaciju zlonamjernih datoteka.</span><span class="sxs-lookup"><span data-stu-id="945be-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="945be-110">Pogledajte [ATP za SharePoint, OneDrive i Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="945be-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>