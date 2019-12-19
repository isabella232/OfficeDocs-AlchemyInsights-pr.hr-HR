---
title: Došlo je do pogreške pri validaciji pogreške tokena pristupa tijekom analitike radne površine
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741136"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="25c4c-102">"Došlo je do pogreške pri validaciji pristupne tokena" tijekom analitike radne površine</span><span class="sxs-lookup"><span data-stu-id="25c4c-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="25c4c-103">Ova pogreška se obično promatra kada token za provjeru autentičnosti istekne.</span><span class="sxs-lookup"><span data-stu-id="25c4c-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="25c4c-104">Obično osvježavanje stranice osvježava token.</span><span class="sxs-lookup"><span data-stu-id="25c4c-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="25c4c-105">Međutim, taj se problem može nastaviti ako postoje pravila uvjetnog pristupa koja se primjenjuju na račun koji se koristi za analitiku radne površine na ploči.</span><span class="sxs-lookup"><span data-stu-id="25c4c-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="25c4c-106">Možete pregledati zapise za prijavu u Azure AD u web-portalu Azure da biste vidjeli postoje li neuspjesi za prijavu za račun koji se koristi za analitiku radne površine.</span><span class="sxs-lookup"><span data-stu-id="25c4c-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="25c4c-107">Dodatne informacije o uvjetnom pristupu potražite u [planu uvođenja uvjetnog pristupa](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="25c4c-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>