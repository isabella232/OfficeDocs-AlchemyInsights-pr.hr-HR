---
title: Rješavanje problema s SMTP provjerom autentičnosti
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 814c49e8e65966a0c9f927b1f7bfb03d3dc3d637
ms.sourcegitcommit: 0e43e19448705f151846e9e9e1e0f47e12938fdf
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/15/2020
ms.locfileid: "44264335"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="1fd49-102">Rješavanje problema s SMTP provjerom autentičnosti</span><span class="sxs-lookup"><span data-stu-id="1fd49-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="1fd49-103">Ako ste uzimajući greška 5.7.57 ili 5.7.3 našto težak to poslati SMTP elektronička pošta i ovjeriti sa mušterija ili aplikacija, ima malo predmet te bi trebao ček:</span><span class="sxs-lookup"><span data-stu-id="1fd49-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="1fd49-104">Autentičnost SMTP slanja možda je onemogućena u klijentu ili u poštanskom sandučiću koji pokušavate koristiti (provjerite obje postavke).</span><span class="sxs-lookup"><span data-stu-id="1fd49-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="1fd49-105">Dodatne informacije [potražite u odjeljku Omogućivanje i onemogućivanje slanja SMTP-a klijenta koji je provjeren](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span><span class="sxs-lookup"><span data-stu-id="1fd49-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="1fd49-106">Provjerite jesu li [za klijenta omogućeni zadani sigurnosni zadani sadržaji](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) za Azure; ako je omogućeno, SMTP provjera autentičnosti pomoću osnovne provjere autentičnosti (poznata i kao naslijeđena; to će koristiti korisničko ime i lozinku) neće uspjeti.</span><span class="sxs-lookup"><span data-stu-id="1fd49-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
