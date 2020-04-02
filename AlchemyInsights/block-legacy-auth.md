---
title: BlokLegacyAuth
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: e7bff5f9fcf6f2f2c77e93c2f27f585f2cc18bea
ms.sourcegitcommit: 98231a228ecb2bf14ec3b96d4dd4ccf2507617a3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/01/2020
ms.locfileid: "43079252"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="62d24-102">Blokiranje naslijeđene provjere autentičnosti</span><span class="sxs-lookup"><span data-stu-id="62d24-102">Blocking legacy authentication</span></span>

<span data-ttu-id="62d24-103">Naslijeđena provjera autentičnosti izraz je koji se odnosi na zahtjev za provjeru autentičnosti koji je iznio:</span><span class="sxs-lookup"><span data-stu-id="62d24-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="62d24-104">Stariji klijenti sustava Office koji ne koriste modernu provjeru autentičnosti (na primjer, klijent sustava Office 2010).</span><span class="sxs-lookup"><span data-stu-id="62d24-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="62d24-105">Bilo koji klijent koji koristi naslijeđene protokole pošte kao što je IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="62d24-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="62d24-106">Dodatne informacije o blokiranju naslijeđene provjere autentičnosti i omogućavanju moderne provjere autentičnosti potražite u odjeljku [Blokiranje naslijeđene provjere autentičnosti](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="62d24-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="62d24-107">Zadane sigurnosne postavke u servisu Azure Active Directory (Azure AD) olakšavaju zaštitu i štite vašu tvrtku ili ustanovu.</span><span class="sxs-lookup"><span data-stu-id="62d24-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="62d24-108">Sigurnosne zadane postavke sadrže unaprijed konfigurirane sigurnosne postavke za uobičajene napade.</span><span class="sxs-lookup"><span data-stu-id="62d24-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="62d24-109">Dodatne informacije o zadanim postavkama sigurnosti potražite u odjeljku [Što su sigurnosne zadane postavke?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="62d24-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="62d24-110">**Napomena:** ako je vaš klijent stvoren 22.</span><span class="sxs-lookup"><span data-stu-id="62d24-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="62d24-111">U nastojanju da zaštiti sve naše korisnike, sigurnosne zadane se uvodi na sve nove stvorene klijente.</span><span class="sxs-lookup"><span data-stu-id="62d24-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
