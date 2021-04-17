---
title: Upravljanje sinkroniziranim korisnikom
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823959"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="e40b6-102">Nije moguće postaviti primarnu adresu e-pošte, promijeniti korisničke atribute ili ukloniti/izbrisati sinkroniziranog korisnika</span><span class="sxs-lookup"><span data-stu-id="e40b6-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="e40b6-103">Ako je sinkronizacija direktorija omogućena za vaše okruženje, neke atribute korisnika ili objekta nije moguće promijeniti pomoću centra za administratore sustava Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e40b6-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="e40b6-104">Da biste u potpunosti upravljali sinkroniziranim korisnicima i svim njihovim atributima, koristite lokalnu konzolu za upravljanje active directory i grupama (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="e40b6-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="e40b6-105">Možete i promijeniti pojedinačne korisnike ili atribute za sinkronizirane korisnike pomoću ljuske powershell, kao što je prikazano u ovim uobičajenim primjerima:</span><span class="sxs-lookup"><span data-stu-id="e40b6-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
