---
title: Rješavanje problema s provjerom autentičnosti SMTP-a
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826407"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="77a85-102">Rješavanje problema s provjerom autentičnosti SMTP-a</span><span class="sxs-lookup"><span data-stu-id="77a85-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="77a85-103">Ako prilikom slanja SMTP e-pošte i provjere autentičnosti s klijentom ili aplikacijom primate pogreške 5.7.57 ili 5.7.3, provjerite nekoliko stvari:</span><span class="sxs-lookup"><span data-stu-id="77a85-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="77a85-104">Provjereno slanje SMTP-a možda je onemogućeno u klijentu ili u poštanskom sandučiću koji pokušavate koristiti (provjerite obje postavke).</span><span class="sxs-lookup"><span data-stu-id="77a85-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="77a85-105">Dodatne informacije potražite u članku Omogućivanje i onemogućivanje provjere [autentičnosti smtp slanja](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)klijenta .</span><span class="sxs-lookup"><span data-stu-id="77a85-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="77a85-106">Provjerite jesu [li za vaš klijent omogućene](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) zadane postavke sigurnosti za Azure; ako je omogućena, SMTP provjera autentičnosti pomoću osnovne provjere autentičnosti (poznata i kao naslijeđena; to će koristiti korisničko ime i lozinku) neće uspjeti.</span><span class="sxs-lookup"><span data-stu-id="77a85-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
