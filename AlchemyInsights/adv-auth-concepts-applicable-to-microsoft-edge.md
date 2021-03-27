---
title: Napredni koncepti provjere autentičnosti koji se primjenjuju na Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398546"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Napredni koncepti provjere autentičnosti koji se primjenjuju na Microsoft Edge

Slijede napredni koncepti provjere autentičnosti koji se primjenjuju na Microsoft Edge:

**Proaktivna provjera autentičnosti**

Kada omogućite [pravilnik ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge će pokušati proaktivno provjeriti autentičnost prijavljenih korisnika putem Microsoftovih servisa. U pravilnim vremenskim razmacima koristit će internetski servis za provjeru ažuriranog manifesta koji sadrži konfiguraciju koja uređuje proaktivnu provjeru autentičnosti.

Prednosti: proaktivna provjera autentičnosti omogućuje provjeru autentičnosti ključnim servisima, kao što je stranica nove kartice sustava Office. Osim toga, ako se Bing koristi kao tražilica, proaktivna provjera autentičnosti poboljšava performanse adresne trake i pridonosi generiranju rezultata pretraživanja personaliziranih potrebama vaše tvrtke.

**Windows Hello CredUI za provjeru autentičnosti NTLM-om**

Ako jedinstvena prijava (SSO) nije dostupna kada se web-mjesto pokuša prijaviti na korisnika putem mehanizma NTLM ili Negotiate, ta će značajka korisniku omogućiti zajedničko korištenje vjerodajnica operacijskog sustava s web-mjestom i zadovoljavanje izazova provjere autentičnosti pomoću korisničkog sučelja za Windows Hello Cred. Taj će se tijek prijave prikazivati samo u sustavu Windows 10 i samo za korisnike koji ne primaju SSO tijekom NTLM-a ili izazova za pregovore.

**Automatska prijava pomoću spremljenih lozinki**

Korisnici koji spremaju lozinke u pregledniku Microsoft Edge mogu omogućiti automatsku prijavu na web-mjesta na kojima su spremili vjerodajnice. Korisnici tu značajku mogu uključiti ili isključiti u edge://settings/passwords, a možete je konfigurirati u pravilima [upravitelja lozinkom.](https://go.microsoft.com/fwlink/?linkid=2134622)
