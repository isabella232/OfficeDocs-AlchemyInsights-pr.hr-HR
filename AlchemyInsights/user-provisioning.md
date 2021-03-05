---
title: Dodjela resursa korisniku
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004348"
- "8428"
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480968"
---
# <a name="user-provisioning"></a>Dodjela resursa korisniku

- Upotrijebite mogućnost [dodjele resursa na zahtjev](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) da biste dodijelili korisniku i dobili detaljnu dijagnostiku o poduznekim koracima.
- Da biste otklonili poteškoće s kojima nailazite prilikom dodjele resursa korisnicima i grupama, pročitajte članak vodič za otklanjanje poteškoća koji [nije dodijeljen korisnicima](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- Ako promatrate da se korisnicima ne dodjeljuju resursi, pročitajte članak [Dodjela resursa zapisnicima (pretpregled) u servisu](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) Azure Active Directory (AD). Potražite stavke zapisnika koje se odnose na određenog korisnika.
- Periodički započinjanje dodjele resursa radi hvatanja svih korisnika koji su propušteni u prethodnom ciklusu dodjele resursa.
- Korisniku/grupi možda nisu dodijeljeni resursi jer naš servis još nije imao priliku procijeniti korisnika. Pregledajte upute o tome koliko traje dodjela resursa, kao i traka tijeka na stranici Konfiguracija dodjele resursa. Ako je stanje stanja koje je navedeno u odjeljku Dodatne pojedinosti prije datuma kada je korisnik stvoren/ažuriran/izbrisan, to znači da još nismo procijenili korisnika. U ovom scenariju najbolje je čekati da servis za dodjelu resursa završi. Ako je stanje stanja dinamičke ravnoteže postignuto, preporučujemo da ponovno pokrenete iz korisničkog sučelja na portalu Azure.
  - Imajte na umu da je naš servis svjestan samo promjena korisnika/grupe u izvornom sustavu (Azure Active Directory). Ako se korisnik/grupa uklanja izravno u aplikaciji (na primjer, ServiceNow), nismo svjesni tih promjena i ne vraćamo ga na temelju stanja korisnika u izvornom sustavu. U ovom scenariju najbolje je vratiti promjenu izravno u ciljnu aplikaciju.
- Naš servis procjenjuje korisnika/grupu i određuje da ga nije potrebno dodijeliti:
  - Ako ste postavili doseg na dodijeljene korisnike i grupe, provjerite je li aplikacija dodijeljena korisniku/grupi.
  - Ako je korisnik/grupa dodijeljen aplikaciji, provjerite nisu li dodijeljeni zadanom ulozi programa Access. Ovu ulogu nije moguće koristiti za dodjelu resursa.
  - Ako ste postavili filtar zasnovan na atributu, Provjerite zadovoljava li korisnik kriterij koji ste naveli.
  - Ako korisnici već postoje u ciljnom sustavu i stanju korisnika u izvoru i ciljnom podudaranju, nećemo poduzeti nikakve daljnje akcije.
- Naš je servis pokušao dodijeliti korisniku i nije uspio. U tim scenarijima Pregledajte karticu Otklanjanje poteškoća i preporuke u zapisnicima za dodjelu resursa:
  - Obavezan atribut korisnika možda nema u servisu Azure Active Directory ili ne odgovara obliku koji je potreban u aplikaciji treće strane. Atribut country na korisniku, primjerice, može biti postavljen u Sjedinjene Države kada bi to trebali biti mi.
  - Atribut je referentni atribut koji još ne postoji u ciljnoj aplikaciji. Referentni atribut predstavlja atribut koji upućuje na neki drugi objekt, na primjer, korisnik koji je član grupe. Korisnički ID bit će u atributu člana grupe, ali se može obraditi samo ako korisnički objekt koji upućuje na već postoji.
