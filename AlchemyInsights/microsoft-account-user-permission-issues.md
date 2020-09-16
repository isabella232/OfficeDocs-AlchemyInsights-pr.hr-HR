---
title: Otklanjanje poteškoća s problemom – korisnik nije pronađen u direktoriju
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725399"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="df113-102">Otklanjanje poteškoća s problemom – korisnik nije pronađen u direktoriju</span><span class="sxs-lookup"><span data-stu-id="df113-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="df113-103">Ako korisnici prime poruku o pogrešci "korisnik se ne može pronaći" u direktoriju, pokušajte ponovno gdje je vrsta problema korisnik koji nije u direktoriju.</span><span class="sxs-lookup"><span data-stu-id="df113-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="df113-104">Rješavanje problema može se dovršiti u sljedećim koracima.</span><span class="sxs-lookup"><span data-stu-id="df113-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="df113-105">Provjerite je li račun koji je prihvatio pozivnicu za e-poštu isti račun koji se koristi za prijavu kasnije.</span><span class="sxs-lookup"><span data-stu-id="df113-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="df113-106">Provjerite koristi li korisnik isti račun za prihvaćanje poziva i prijava na web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="df113-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="df113-107">Dodatne informacije potražite u članku [upravljanje pseudonimima za Microsoftov račun </a> za upravljanje prijavom u Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="df113-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="df113-108">Dođite do svih web-mjesta u kojima korisnik prima pogrešku.</span><span class="sxs-lookup"><span data-stu-id="df113-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="df113-109">Na kraj URL-a web-mjesta dodajte "/_layouts/15/People.aspx/membershipgroupid = 0" (unutar dvostrukih navodnika).</span><span class="sxs-lookup"><span data-stu-id="df113-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="df113-110">Primjer: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="df113-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="df113-111">Odaberite korisnika s popisa.</span><span class="sxs-lookup"><span data-stu-id="df113-111">Select the user from the list.</span></span>

- <span data-ttu-id="df113-112">Na vrpci kliknite **Ukloni korisničke dozvole** .</span><span class="sxs-lookup"><span data-stu-id="df113-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="df113-113">Dodajte natrag korisnika i ponovno pošaljite pozivnicu korisniku.</span><span class="sxs-lookup"><span data-stu-id="df113-113">Add back the User and Resend the invite to the user.</span></span>

