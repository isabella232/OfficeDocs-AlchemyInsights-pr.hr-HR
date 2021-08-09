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
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934357"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Napredni koncepti provjere autentičnosti koji se primjenjuju na Microsoft Edge

Slijede napredni koncepti provjere autentičnosti koji se primjenjuju na Microsoft Edge:

**Proaktivna provjera autentičnosti**

Kada omogućite [pravilnik ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge će pokušati proaktivno provjeriti autentičnost prijavljenih korisnika putem Microsoft services. U pravilnim vremenskim razmacima koristit će internetski servis za provjeru ažuriranog manifesta koji sadrži konfiguraciju koja uređuje proaktivnu provjeru autentičnosti.

Prednosti: proaktivna provjera autentičnosti omogućuje provjeru autentičnosti ključnim servisima, kao što je Office nova stranica kartice. Ako se Bing kao tražilica, proaktivna provjera autentičnosti poboljšava performanse adresne trake i pridonosi generiranju rezultata pretraživanja personaliziranih potrebama vaše tvrtke.

**Windows Hello CredUI za NTLM provjeru autentičnosti**

Ako jedinstvena prijava (SSO) nije dostupna kada se web-mjesto pokuša prijaviti na korisnika putem mehanizma NTLM ili Negotiate, ta će značajka korisniku omogućiti zajedničko korištenje vjerodajnica operacijskog sustava s web-mjestom i zadovoljavanje izazova provjere autentičnosti pomoću korisničkog sučelja Windows Hello Cred. Taj će se tijek prijave prikazivati samo u Windows 10 i samo za korisnike koji ne primaju SSO tijekom NTLM-a ili izazova za pregovore.

**Automatska prijava pomoću spremljenih lozinki**

Korisnici koji spremaju lozinke u Microsoft Edge mogu omogućiti automatsku prijavu na web-mjesta na kojima su spremili vjerodajnice. Korisnici tu značajku mogu uključiti ili isključiti u edge://settings/passwords, a možete je konfigurirati u pravilima [upravitelja lozinkom.](https://go.microsoft.com/fwlink/?linkid=2134622)
