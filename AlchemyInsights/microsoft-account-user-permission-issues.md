---
title: Rješavanje problema-korisnik nije pronađen u direktoriju
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0f1e427801107109e31486a4d300f53084880caf
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054802"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="fa874-102">Rješavanje problema-korisnik nije pronađen u direktoriju</span><span class="sxs-lookup"><span data-stu-id="fa874-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="fa874-103">Ako korisnici primaju poruku o pogrešci "korisnik ne može naći" u direktoriju, pokušajte ponovno gdje vrsta problema je korisnik nije u direktoriju.</span><span class="sxs-lookup"><span data-stu-id="fa874-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="fa874-104">Za otklanjanje problema možete dovršiti sljedeće korake.</span><span class="sxs-lookup"><span data-stu-id="fa874-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="fa874-105">Provjerite je li račun koji je prihvatio pozivnicu e-poštom isti račun koji se koristi za prijavu kasnije.</span><span class="sxs-lookup"><span data-stu-id="fa874-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="fa874-106">Provjerite koristi li korisnik isti račun za prihvaćanje pozivnice i prijavu na web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="fa874-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="fa874-107">Dodatne informacije potražite u članku [kako upravljati pseudonime za Microsoftov račun</a> za upravljanje uredom 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="fa874-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="fa874-108">Pregledajte Svaka web-mjesta u kojima korisnik prima pogrešku.</span><span class="sxs-lookup"><span data-stu-id="fa874-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="fa874-109">Dodajte "/_layouts/15/. aspx/membershipgroupid = 0" (unutar dvostrukih navodnika) do kraja URL-a web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="fa874-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="fa874-110">Primjer: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="fa874-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="fa874-111">Odaberite korisnika s popisa.</span><span class="sxs-lookup"><span data-stu-id="fa874-111">Select the user from the list.</span></span>

- <span data-ttu-id="fa874-112">Kliknite **Ukloni korisničke dozvole** s vrpce.</span><span class="sxs-lookup"><span data-stu-id="fa874-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="fa874-113">Dodajte korisnika natrag i ponovno pošaljite pozivnicu korisniku.</span><span class="sxs-lookup"><span data-stu-id="fa874-113">Add back the User and Resend the invite to the user.</span></span>

