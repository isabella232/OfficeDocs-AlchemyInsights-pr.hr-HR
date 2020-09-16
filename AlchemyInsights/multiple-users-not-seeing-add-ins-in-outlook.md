---
title: Više korisnika koji ne vide dodatke u programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729863"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="b1f6e-102">Više korisnika koji ne vide dodatke u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="b1f6e-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="b1f6e-103">Ako isprobate dodatke programa Outlook, a nijedna se ne prikaže, kao prvi korak otklanjanja poteškoća, pomoću cmdleta **Get-OrganizationConfig** PowerShell zatražite upit za parametar _Appsforofficeenabled_ .</span><span class="sxs-lookup"><span data-stu-id="b1f6e-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="b1f6e-104">Ako upit vraća vrijednost **False**, postavite ovaj parametar na **True** pomoću cmdleta **set-OrganizationConfig** , pa se dodaci prikazuju kao što je očekivano.</span><span class="sxs-lookup"><span data-stu-id="b1f6e-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="b1f6e-105">Ne preporučujemo da parametar _Appsforofficeenabled_ bude postavljen na **False**.</span><span class="sxs-lookup"><span data-stu-id="b1f6e-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="b1f6e-106">Vrijednost **lažnih** prekoračenja svih navedenih postavki administrativne i korisničke uloge i onemogućuje aktiviranje novih aplikacija od strane bilo kojeg korisnika u tvrtki ili ustanovi.</span><span class="sxs-lookup"><span data-stu-id="b1f6e-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="b1f6e-107">Dodatne informacije potražite u članku [određivanje administratora i korisnika koji mogu instalirati dodatke za Outlook i upravljati njima](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="b1f6e-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>