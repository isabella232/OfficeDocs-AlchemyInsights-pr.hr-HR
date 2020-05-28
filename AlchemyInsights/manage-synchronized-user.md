---
title: Upravljanje sinkroniziranim korisnikom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407342"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="3ca69-102">Nije moguće postaviti primarnu adresu e-pošte, promijeniti korisničke atribute ili ukloniti/izbrisati sinkroniziranog korisnika</span><span class="sxs-lookup"><span data-stu-id="3ca69-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="3ca69-103">Ako je sinkronizacija direktorija omogućena za vaše okruženje, neki atributi korisnika ili objekta ne mogu se mijenjati pomoću centra za administratore sustava Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3ca69-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="3ca69-104">Da biste u potpunosti upravljali sinkroniziranim korisnicima i svim njihovim atributima, upotrijebite lokalne korisnike i konzolu za upravljanje aktivnim direktorijem (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="3ca69-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="3ca69-105">Umjesto toga, možete promijeniti pojedinačne korisnike ili atribute za sinkronizirane korisnike pomoću ljuske powershell kao što je prikazano u ovim uobičajenim primjerima:</span><span class="sxs-lookup"><span data-stu-id="3ca69-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
