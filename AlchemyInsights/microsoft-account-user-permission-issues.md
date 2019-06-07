---
title: Stvarati i koristiti zajednički poštanski sandučić
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81bf8082198de1c44037291f23c434d06a77f02a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762393"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="fbcc3-102">Poteškoća - korisnik nije pronađen u imeniku</span><span class="sxs-lookup"><span data-stu-id="fbcc3-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="fbcc3-103">Ako korisnici primaju pogreška poruka "nije moguće pronaći korisnika" u imeniku.</span><span class="sxs-lookup"><span data-stu-id="fbcc3-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="fbcc3-104">Molimo pokušajte ponovo gdje vrste problema nije korisnik u imenik.</span><span class="sxs-lookup"><span data-stu-id="fbcc3-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="fbcc3-105">Sljedeće korake možete dovršiti za otklanjanje poteškoća.</span><span class="sxs-lookup"><span data-stu-id="fbcc3-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="fbcc3-106">Provjerite račun koji je prihvatio poziv e-poštom je isti račun koji koristi se prijaviti kasnije.</span><span class="sxs-lookup"><span data-stu-id="fbcc3-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="fbcc3-107">Provjerite je li korisnik koristi isti račun za prihvaćanje na Pozovi i prijaviti na web-mjestu.</span><span class="sxs-lookup"><span data-stu-id="fbcc3-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="fbcc3-108">Za dodatne informacije pogledajte [kako upravljati pseudonime za Microsoftov račun</a> za upravljanje Office 365 prijava](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="fbcc3-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="fbcc3-109">Pregledaj svakog web-mjesta u kojima korisnik prima pogrešku.</span><span class="sxs-lookup"><span data-stu-id="fbcc3-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="fbcc3-110">Dodaj "/ _layouts/15/people.aspx/membershipgroupid=0" (unutar u dvostruke navodnike) na kraj URL web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="fbcc3-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="fbcc3-111">Primjer: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="fbcc3-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="fbcc3-112">Odaberite korisnika s popisa.</span><span class="sxs-lookup"><span data-stu-id="fbcc3-112">Select the user from the list.</span></span>

- <span data-ttu-id="fbcc3-113">Kliknite **Ukloni korisničke dozvole** na vrpci.</span><span class="sxs-lookup"><span data-stu-id="fbcc3-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="fbcc3-114">Dodavanje korisnika i ponovo pošaljite na poziv korisniku.</span><span class="sxs-lookup"><span data-stu-id="fbcc3-114">Add back the User and Resend the invite to the user.</span></span>

