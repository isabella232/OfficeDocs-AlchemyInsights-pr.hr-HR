---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820170"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="4a329-102">Blokiranje naslijeđene provjere autentičnosti</span><span class="sxs-lookup"><span data-stu-id="4a329-102">Blocking legacy authentication</span></span>

<span data-ttu-id="4a329-103">Naslijeđena provjera autentičnosti pojam je koji se odnosi na zahtjev za provjeru autentičnosti koji je zatražio:</span><span class="sxs-lookup"><span data-stu-id="4a329-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="4a329-104">Stariji klijenti sustava Office koji ne koriste modernu provjeru autentičnosti (npr. klijent sustava Office 2010).</span><span class="sxs-lookup"><span data-stu-id="4a329-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="4a329-105">Svaki klijent koji koristi naslijeđene protokole e-pošte, kao što su IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="4a329-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="4a329-106">Dodatne informacije o blokiranju naslijeđene provjere autentičnosti i omogućivanju moderne provjere autentičnosti potražite u odjeljku [Blokiranje naslijeđene provjere autentičnosti](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span><span class="sxs-lookup"><span data-stu-id="4a329-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="4a329-107">Zadane sigurnosne postavke na servisu Azure Active Directory (Azure AD) olakšavaju zaštitu i zaštitu tvrtke ili ustanove.</span><span class="sxs-lookup"><span data-stu-id="4a329-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="4a329-108">Zadane sigurnosne postavke sadrže unaprijed konfigurirane sigurnosne postavke za uobičajene napade.</span><span class="sxs-lookup"><span data-stu-id="4a329-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="4a329-109">Dodatne informacije o sigurnosnim zadanim postavkama potražite u odjeljku [Što su sigurnosne zadane postavke?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="4a329-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="4a329-110">**Napomena:** ako je klijent stvoren 22. listopada 2019., moguće je da nailazite na novo sigurno po zadanom ponašanje i već imate omogućene sigurnosne zadane postavke u klijentu.</span><span class="sxs-lookup"><span data-stu-id="4a329-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="4a329-111">U nastojanju da zaštitimo sve naše korisnike, sigurnosne se zadane postavke u svim novim korisnicima stvaraju.</span><span class="sxs-lookup"><span data-stu-id="4a329-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
