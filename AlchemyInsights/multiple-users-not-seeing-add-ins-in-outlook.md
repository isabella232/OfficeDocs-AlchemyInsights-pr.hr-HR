---
title: Više korisnika koji ne vide dodatke u programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197771"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="7a1cb-102">Više korisnika koji ne vide dodatke u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="7a1cb-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="7a1cb-103">Ako testirate dodatke programa Outlook i ništa se ne prikazuje, kao prvi korak za otklanjanje poteškoća, upotrijebite cmdlet **Get-OrganizationConfig** PowerShell da biste upitali parametar _AppsForOfficeEnabled._</span><span class="sxs-lookup"><span data-stu-id="7a1cb-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="7a1cb-104">Ako upit vraća vrijednost **False**, postavite ovaj parametar na **True** pomoću cmdleta **Set-OrganizationConfig,** tako da se dodaci pojavljuju prema očekivanjima.</span><span class="sxs-lookup"><span data-stu-id="7a1cb-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="7a1cb-105">Ne preporučujemo da parametar _AppsForOfficeEnabled_ postavljen na **False**.</span><span class="sxs-lookup"><span data-stu-id="7a1cb-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="7a1cb-106">Vrijednost **False** nadjačava sve gore navedene postavke uloge administrativne i korisničke uloge i sprječava bilo koje nove aplikacije da budu aktivirane od strane bilo kojeg korisnika u tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="7a1cb-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="7a1cb-107">Dodatne informacije [potražite u odjeljku Određivanje administratora i korisnika koji mogu instalirati dodatke za Outlook i upravljati njima](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="7a1cb-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>