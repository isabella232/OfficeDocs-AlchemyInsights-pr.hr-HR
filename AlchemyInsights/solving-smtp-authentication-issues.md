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
# <a name="solving-smtp-authentication-issues"></a>Rješavanje problema s provjerom autentičnosti SMTP

Ako dobivate pogreške 5.7.57 ili 5.7.3 prilikom pokušaja slanja SMTP e-pošte i autentičnosti pomoću klijenta ili aplikacije, morate provjeriti nekoliko stavki:

- Provjereni SMTP slanje može biti onemogućeno u vašem zakupcu ili na poštanskom sandučiću koji pokušavate koristiti (provjerite obje postavke). Da biste pročitali više, pročitajte članak [Omogućivanje i onemogućivanje slanja SMTP autentičnosti klijenta](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).

- Provjerite jesu li za vašeg stanara omogućene [sigurnosne zadane postavke Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) . Ako je omogućeno, provjera autentičnosti SMTP-a pomoću osnovne provjere autentičnosti (poznata i kao ostavština; to će koristiti korisničko ime i lozinku) neće uspjeti.
