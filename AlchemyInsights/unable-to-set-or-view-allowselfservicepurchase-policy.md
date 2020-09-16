---
title: Nije moguće postaviti ili prikazati pravilo Allowselfservicekupnja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735191"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="a897c-102">Nije moguće postaviti ili prikazati pravilo Allowselfservicekupnja</span><span class="sxs-lookup"><span data-stu-id="a897c-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="a897c-103">Kada pokušate postaviti ili prikazati pravilo Allowselfservicekupnja, prikazat će vam se sljedeća poruka o pogrešci:</span><span class="sxs-lookup"><span data-stu-id="a897c-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="a897c-104">*Funkcija HandleError: nije uspjelo dohvaćanje pravilnika o proizvodu s PolicyId ' Allowselfservicekupnja ', ErrorMessage-osnovna veza je zatvorena: došlo je do neočekivane pogreške na slanju.*</span><span class="sxs-lookup"><span data-stu-id="a897c-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="a897c-105">To može biti zbog starije verzije sigurnosnog sloja za transport (TLS).</span><span class="sxs-lookup"><span data-stu-id="a897c-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="a897c-106">Da biste povezali servis MSCommerce, morate koristiti TLS 1,2 ili noviji.</span><span class="sxs-lookup"><span data-stu-id="a897c-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="a897c-107">Pokušajte poduzeti sljedeće korake da biste omogućili/postavili TLS protokol na 1,2, potvrdili i pokušali ponovno.</span><span class="sxs-lookup"><span data-stu-id="a897c-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="a897c-108">U naredbeni upit za PowerShell (PS C: \) Unesite sljedeću naredbu da biste postavili TLS protokol na verziju 1,2:</span><span class="sxs-lookup"><span data-stu-id="a897c-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="a897c-109">Potvrđivanje TLS protokola (s) u upotrebi, uz sljedeću naredbu:</span><span class="sxs-lookup"><span data-stu-id="a897c-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="a897c-110">Ponovno pokušajte izvršiti naredbe Dohvati ili Ažuriraj po potrebi.</span><span class="sxs-lookup"><span data-stu-id="a897c-110">Retry the Get or Update commands as needed.</span></span>

