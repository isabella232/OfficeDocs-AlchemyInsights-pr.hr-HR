---
title: Moderna web-mjesta kao korijensko web-mjesto
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057683"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="02916-102">Moderna web-mjesta kao korijensko web-mjesto</span><span class="sxs-lookup"><span data-stu-id="02916-102">Modern site as root site</span></span>

<span data-ttu-id="02916-103">[Ciljni izdanje](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) kupci sada možete omogućiti web-mjesta doživljaj Moderna komunikacije na klasični korijensko web-mjesto klijentske svoje SharePoint.</span><span class="sxs-lookup"><span data-stu-id="02916-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="02916-104">Ovu značajku možete aktivirati pokretanjem jednostavne cmdlet PowerShell.</span><span class="sxs-lookup"><span data-stu-id="02916-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="02916-105">Na uspješno izvršavanje PowerShell command(s) korijenskog web-mjesta imaju nove početne stranice web-mjesta komunikacije.</span><span class="sxs-lookup"><span data-stu-id="02916-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="02916-106">Pojedinosti o preduvjetima cmdlet i značajka PowerShell su dostupne u članku [Omogući SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="02916-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="02916-107">Možemo ćete biti postupno pomični to, isključiti po zadanom ciljane izdanje kupcima u ranim 2019 možda i bacanje out bit će dostupna širom svijeta kraja lipanj 2019.</span><span class="sxs-lookup"><span data-stu-id="02916-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="02916-108">Nastavak za upućivanje na [Poruku centar](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) za ostale nove značajke s Moderni.</span><span class="sxs-lookup"><span data-stu-id="02916-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="02916-109">**Važno**: brisanje klasični korijensko web-mjesto za stvaranje Moderna komunikacije web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="02916-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="02916-110">Ovo je Microsoft ne podržava.</span><span class="sxs-lookup"><span data-stu-id="02916-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="02916-111">Brisanje korijenskog web-mjesta će napraviti sve SharePoint web-mjestima u vašoj organizaciji nedostupni na sve korisnike dok ne obnovite web-mjesto ili stvorite novo web-mjesto na URL-u istoj.</span><span class="sxs-lookup"><span data-stu-id="02916-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 