---
title: BlockLegacyAuth
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
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685590"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="6989d-102">Blokiranje naslijeđene provjere autentičnosti</span><span class="sxs-lookup"><span data-stu-id="6989d-102">Blocking legacy authentication</span></span>

<span data-ttu-id="6989d-103">Ostavština provjere autentičnosti pojam je koji se odnosi na zahtjev za provjeru autentičnosti od strane:</span><span class="sxs-lookup"><span data-stu-id="6989d-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="6989d-104">Stariji klijenti sustava Office koji ne koriste modernu provjeru autentičnosti (primjerice, klijent sustava Office 2010).</span><span class="sxs-lookup"><span data-stu-id="6989d-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="6989d-105">Bilo koji klijent koji koristi postojeće protokole e-pošte, kao što je IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="6989d-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="6989d-106">Dodatne informacije o blokiranju naslijeđene provjere autentičnosti i omogućivanju moderne provjere autentičnosti potražite u odjeljku [blokiranje naslijeđene provjere autentičnosti](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="6989d-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="6989d-107">Postavke sigurnosti u servisu Azure Active Directory (Azure AD) olakšavaju sigurnost i pomažu u zaštiti tvrtke ili ustanove.</span><span class="sxs-lookup"><span data-stu-id="6989d-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="6989d-108">Sigurnosne zadane postavke sadrže unaprijed konfigurirane sigurnosnu postavku za česte napade.</span><span class="sxs-lookup"><span data-stu-id="6989d-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="6989d-109">Dodatne informacije o sigurnosnim zadanim postavkama potražite u odjeljku [što su zadane postavke sigurnosti?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="6989d-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="6989d-110">**Pažnja**: ako je vaš stanar stvoren na ili nakon 22. listopada, 2019, moguće je da nailazite na novo ponašanje sigurnog prema zadanom, a već imate omogućen sigurnosni propust u zakupcu.</span><span class="sxs-lookup"><span data-stu-id="6989d-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="6989d-111">U nastojanju da se zaštiti svi naši korisnici, sigurnosne zadane postavke iskotrljali su se na sve nove stanare stvorene.</span><span class="sxs-lookup"><span data-stu-id="6989d-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
