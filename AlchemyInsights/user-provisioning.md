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
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971331"
---
# <a name="user-provisioning"></a>Dodjela resursa korisniku

- Upotrijebite [mogućnost dodjele resursa na zahtjev](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) da biste korisniku dodijeliti resursa i dobili detaljnu dijagnostiku o poduzetim koracima.
- Da biste otklonili poteškoće na koje nailazite prilikom dodjele resursa korisnicima i grupama, pogledajte vodič za otklanjanje poteškoća [Bez dodjele resursa korisnicima](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- Ako primijetite da korisnicima nije dodijeljena dodjela resursa, pogledajte zapisnike dodjele [resursa (pretpregled)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) u programu Azure Active Directory (AD). Potražite unose zapisnika koji se odnose na određenog korisnika.
- Povremeno ponovno pokrenite dodjeljivanje resursa da biste uhvatili sve korisnike koji su propustili u prethodnom ciklusu dodjele resursa.
- Korisnik/grupa možda nije dodijeljena dodjela resursa jer naš servis još nije imao priliku procijeniti korisnika. Pregledajte smjernice za vrijeme potrebnog dodjeljivanja resursa, kao i traku tijeka na stranici konfiguracije dodjele resursa. Ako je stanje dinamičke ravnoteže navedeno u odjeljku s dodatnim detaljima prije datuma kada je korisnik stvoren/ažuriran/izbrisan, to znači da još nismo procijenili korisnika. U ovom scenariju najbolje je pričekati da se servis za dodjeljivanje resursa dovrši. Ako se stanje dinamičke ravnoteže postići, preporučujemo da ponovno pokrenete UI na portalu Azure.
  - Imajte na umu da je naš servis upoznat samo s promjenama korisnika/grupe u izvorišnom sustavu (Azure Active Directory). Ako se korisnik/grupa ukloni izravno u aplikaciji (na primjer, ServiceNow), nismo svjesni tih promjena i ne vraćamo ih na temelju stanja korisnika u izvorišnom sustavu. U ovom je scenariju najbolje vratiti promjenu izravno u ciljnoj aplikaciji.
- Naš servis procijenio je korisnika/grupu i odredio da se ne smije dodjeljivati:
  - Ako ste opseg postavili na dodijeljene korisnike i grupe, provjerite je li korisnik/grupa dodijeljen aplikaciji.
  - Ako je korisniku/grupi dodijeljena aplikacija, provjerite nisu li dodijeljeni zadanoj ulozi pristupa. Tu ulogu nije moguće koristiti za dodjeljivanje resursa.
  - Ako ste postavili filtar za određivanje opsega utemeljen na atributima, provjerite zadovoljava li korisnik kriterije koje ste naveli.
  - Ako korisnici već postoje u ciljnom sustavu i stanju korisnika u izvorišnom i ciljnom podudaraju, nećemo više ništa poduzeti.
- Naš servis pokušao je dodijeliti korisniku i nije uspio. U tim scenarijima pregledajte karticu otklanjanje poteškoća i preporuka zapisnika dodjele resursa:
  - Obavezni atribut na korisniku možda nema u Azure Active Directory ili ne odgovara obliku koji zahtijeva aplikacija drugih proizvođača. Atribut Država korisnika, primjerice, može biti postavljen na Sjedinjene Američke Države kada bi trebao biti u SAD-u.
  - Atribut je referencijalni atribut koji još ne postoji u ciljnoj aplikaciji. Referencijalni atribut atribut je koji upućuje na drugi objekt, primjerice korisnika koji je član grupe. KORISNIKOV ID nalazio bi se u atributu člana grupe, ali se može obraditi samo ako korisnički objekt na koji upućuje već postoji.
