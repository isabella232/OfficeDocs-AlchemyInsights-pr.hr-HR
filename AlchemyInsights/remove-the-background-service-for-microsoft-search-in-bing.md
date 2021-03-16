---
title: Uklanjanje pozadinskog servisa za Microsoft Search u programu Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816090"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="c4115-102">Uklanjanje pozadinskog servisa za Microsoft Search u programu Bing</span><span class="sxs-lookup"><span data-stu-id="c4115-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="c4115-103">Da biste uklonili pozadinski servis za Microsoft Search u programu Bing, isprobajte sljedeće lijekove:</span><span class="sxs-lookup"><span data-stu-id="c4115-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="c4115-104">Da biste se vratili na izvorne postavke tražilice, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="c4115-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="c4115-105">je.</span><span class="sxs-lookup"><span data-stu-id="c4115-105">a.</span></span> <span data-ttu-id="c4115-106">Promijenite gumb **koristi Bing kao zadanu postavku isključivanja tražilice [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**.</span><span class="sxs-lookup"><span data-stu-id="c4115-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="c4115-107">b.</span><span class="sxs-lookup"><span data-stu-id="c4115-107">b.</span></span> <span data-ttu-id="c4115-108">[Otvorite centar za administratore sustava Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) i poništite postavku koja utječe na sve korisnike u tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="c4115-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="c4115-109">Da biste uklonili pozadinski servis s pojedinog uređaja, učinite sljedeće:</span><span class="sxs-lookup"><span data-stu-id="c4115-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="c4115-110">je.</span><span class="sxs-lookup"><span data-stu-id="c4115-110">a.</span></span> <span data-ttu-id="c4115-111">Odaberite **Upravljačka ploča > programe > programe i značajke**.</span><span class="sxs-lookup"><span data-stu-id="c4115-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="c4115-112">b.</span><span class="sxs-lookup"><span data-stu-id="c4115-112">b.</span></span> <span data-ttu-id="c4115-113">Desnom tipkom miša kliknite **Microsoft Search u programu Bing na** popisu instaliranih programa, a zatim kliknite **Deinstaliraj**.</span><span class="sxs-lookup"><span data-stu-id="c4115-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="c4115-114">Da biste uklonili poslužitelj pozadine s više uređaja u tvrtki ili ustanovi, prijavite se kao administrator i pokrenite sljedeću naredbu u skripti:</span><span class="sxs-lookup"><span data-stu-id="c4115-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
