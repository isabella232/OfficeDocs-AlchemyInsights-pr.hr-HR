---
title: Napredni koncepti provjere autentičnosti koji se odnose na Microsoft Edge
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573297"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Napredni koncepti provjere autentičnosti koji se odnose na Microsoft Edge

Slijede Napredni koncepti provjere autentičnosti koji su primjenjivi na Microsoft Edge:

**Proaktivna provjera autentičnosti**

Kada omogućite pravilo [Proactiveauthenabled](https://go.microsoft.com/fwlink/?linkid=2134621) , Microsoft Edge nastojat će proaktivno provjeriti autentičnost korisnika potpisanih putem Microsoftova servisa. U pravilnim intervalima koristit će internetski servis za provjeru ažuriranog manifesta koji sadrži konfiguraciju koja regulira proaktivnu provjeru autentičnosti.

Prednosti: proaktivna provjera autentičnosti omogućuje provjeru autentičnosti ključnim servisima, kao što je stranica nove kartice sustava Office. Osim toga, ako se Bing koristi kao tražilica, proaktivna provjera autentičnosti poboljšava performanse adresne trake i olakšava stvaranje personalizirane rezultate pretraživanja na potrebe poslovanja.

**Windows Hello CredUI za NTLM provjeru autentičnosti**

Ako jedinstvena prijava (SSO) nije dostupna kada se web-mjesto pokuša prijavljivati korisniku putem mehanizma NTLM ili pregovara, ta će značajka omogućiti korisniku zajedničko korištenje vjerodajnica za OS uz web-mjesto i zadovoljavanje izazova za provjeru autentičnosti pomoću korisničkog sučelja za Windows Hello Cred. Taj će se tijek prijave prikazivati samo u sustavu Windows 10 i to samo za korisnike koji ne dobiju SSO tijekom programa NTLM ili pregovarača.

**Automatsko prijavljivanje pomoću spremljenih lozinki**

Korisnici koji spremaju lozinke u pregledniku Microsoft Edge mogu omogućiti automatsko prijavljivanje na web-mjesta na kojima su spremljene vjerodajnice. Korisnici mogu uključiti ili isključiti ovu značajku na servisu edge://settings/passwords, a možete je konfigurirati u pravilima [upravitelja lozinki](https://go.microsoft.com/fwlink/?linkid=2134622) .
