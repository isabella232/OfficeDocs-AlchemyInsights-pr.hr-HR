---
title: Rješavanje problema s provjerom autentičnosti SMTP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 3eaab2c601f78e20f2ee67bc21a9598cb45a24f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737981"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="e1d19-102">Rješavanje problema s provjerom autentičnosti SMTP</span><span class="sxs-lookup"><span data-stu-id="e1d19-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="e1d19-103">Ako dobivate pogreške 5.7.57 ili 5.7.3 prilikom pokušaja slanja SMTP e-pošte i autentičnosti pomoću klijenta ili aplikacije, morate provjeriti nekoliko stavki:</span><span class="sxs-lookup"><span data-stu-id="e1d19-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="e1d19-104">Provjereni SMTP slanje može biti onemogućeno u vašem zakupcu ili na poštanskom sandučiću koji pokušavate koristiti (provjerite obje postavke).</span><span class="sxs-lookup"><span data-stu-id="e1d19-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="e1d19-105">Da biste pročitali više, pročitajte članak [Omogućivanje i onemogućivanje slanja SMTP autentičnosti klijenta](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span><span class="sxs-lookup"><span data-stu-id="e1d19-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="e1d19-106">Provjerite jesu li za vašeg stanara omogućene [sigurnosne zadane postavke Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) . Ako je omogućeno, provjera autentičnosti SMTP-a pomoću osnovne provjere autentičnosti (poznata i kao ostavština; to će koristiti korisničko ime i lozinku) neće uspjeti.</span><span class="sxs-lookup"><span data-stu-id="e1d19-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
