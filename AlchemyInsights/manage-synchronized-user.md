---
title: Upravljanje sinkronizirane korisnika
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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541975"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="06e24-102">Nije moguće postaviti adresu e-pošte primarnog ili promijeniti korisničke atribute</span><span class="sxs-lookup"><span data-stu-id="06e24-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="06e24-103">Ako sinkroniziranje direktorija je omogućen za vaše okruženje, neki atributi korisnik ili objekt nije moguće promijeniti pomoću centra za administraciju Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="06e24-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="06e24-104">Da biste upravljali potpuno sinkronizirane korisnika i njihove atribute, koristiti vaš aktivni imenik lokalne korisnike i grupe konzole za upravljanje (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="06e24-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="06e24-105">Umjesto toga, možete promijeniti pojedinačni korisnici ili atribute za sinkronizirane korisnici pomoću powershell kao što je prikazano u ove uobičajeni primjeri:</span><span class="sxs-lookup"><span data-stu-id="06e24-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="06e24-106">Skup MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="06e24-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="06e24-107">Skup MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Test User" - Prezime "Korisnički"-Naslov "Upravitelja"-odjel "HR"</span><span class="sxs-lookup"><span data-stu-id="06e24-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="06e24-108">Ukloni MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="06e24-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>