---
title: ATP za SharePoint, OneDrive i Microsoftove timove
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715553"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="670e4-102">ATP za SharePoint, OneDrive i Microsoftove timove</span><span class="sxs-lookup"><span data-stu-id="670e4-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="670e4-103">Slijedite ove korake da biste omogućili naprednu zaštitu od prijetnji:</span><span class="sxs-lookup"><span data-stu-id="670e4-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="670e4-104">Idite na [https://protection.office.com](https://protection.office.com) i prijavite se pomoću računa globalnog administratora ili sigurnosnog administratora.</span><span class="sxs-lookup"><span data-stu-id="670e4-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="670e4-105">U lijevoj navigacijskom oknu u odjeljku **Upravljanje prijetnjama**odaberite **Policy** \> **sigurni prilozi**pravilnika.</span><span class="sxs-lookup"><span data-stu-id="670e4-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="670e4-106">Odaberite **Uključi ATP za SharePoint, OneDrive i Microsoftove timove**.</span><span class="sxs-lookup"><span data-stu-id="670e4-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="670e4-107">[Stvaranje pravilnika upozorenja o aktivnostima](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) za primanje obavijesti prilikom otkrivanja zlonamjernih datoteka.</span><span class="sxs-lookup"><span data-stu-id="670e4-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="670e4-108">Detaljne upute potražite u ovoj [temi](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="670e4-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="670e4-109">**Pažnja**: prema dizajnu, ATP ne skenira svaku pojedinačnu datoteku u sustavu SharePoint Online, OneDrive za tvrtke ili Microsoftove timove.</span><span class="sxs-lookup"><span data-stu-id="670e4-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="670e4-110">Datoteke se asinkrono skenira pomoću postupka koji koristi zajedničko korištenje aktivnosti, aktivnosti gosta i signale prijetnji radi prepoznavanja zlonamjernih datoteka.</span><span class="sxs-lookup"><span data-stu-id="670e4-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="670e4-111">Dodatne informacije potražite u ovoj [temi](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="670e4-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
