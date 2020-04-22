---
title: Rješavanje problema - Korisnik nije pronađen u direktoriju
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702730"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="f27f9-102">Rješavanje problema - Korisnik nije pronađen u direktoriju</span><span class="sxs-lookup"><span data-stu-id="f27f9-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="f27f9-103">Ako korisnik jesu primanje poruka o pogreški " korisnik ne moći' biti postaviti" in imenik, ugoditi probati opet gdje svi Ispostavljati je Korisnik ne in imenik.</span><span class="sxs-lookup"><span data-stu-id="f27f9-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="f27f9-104">Da biste otklonili problem, možete izvršiti sljedeće korake.</span><span class="sxs-lookup"><span data-stu-id="f27f9-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="f27f9-105">Provjerite je li račun koji je prihvatio pozivnicu za e-poštu isti račun koji se kasnije koristi za prijavu.</span><span class="sxs-lookup"><span data-stu-id="f27f9-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="f27f9-106">Provjerite koristi li korisnik isti račun za prihvaćanje pozivnice i prijavu na web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="f27f9-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="f27f9-107">Dodatne informacije [potražite u odjeljku Upravljanje pseudonimima</a> za Microsoftov račun radi upravljanja prijavom na Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="f27f9-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="f27f9-108">Pronađite svako web-mjesto(e) na kojem korisnik prima pogrešku.</span><span class="sxs-lookup"><span data-stu-id="f27f9-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="f27f9-109">Dodajte "/_layouts/15/people.aspx/membershipgroupid=0" (unutar dvostrukih navodnika) do kraja URL-a web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="f27f9-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="f27f9-110">Primjer: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="f27f9-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="f27f9-111">Odaberite korisnika s popisa.</span><span class="sxs-lookup"><span data-stu-id="f27f9-111">Select the user from the list.</span></span>

- <span data-ttu-id="f27f9-112">Na vrpci kliknite **Ukloni korisničke dozvole.**</span><span class="sxs-lookup"><span data-stu-id="f27f9-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="f27f9-113">Dodajte natrag korisnika i ponovno pošaljite pozivnicu korisniku.</span><span class="sxs-lookup"><span data-stu-id="f27f9-113">Add back the User and Resend the invite to the user.</span></span>

