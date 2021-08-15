---
title: Problem s jednim korisnikom
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
- "9004687"
- "8469"
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960143"
---
# <a name="problem-with-single-user"></a>Problem s jednim korisnikom

- Korisniku možda nije dodijeljena dodjela resursa jer servis još nije imao priliku procijeniti korisnika. Pregledajte smjernice za vrijeme potrebnog dodjeljivanja resursa, kao i traku tijeka na stranici konfiguracije dodjele resursa. Ako je stanje dinamičke ravnoteže navedeno u odjeljku s dodatnim detaljima prije datuma kada je korisnik stvoren/ažuriran/izbrisan, to znači da još nismo procijenili korisnika. U ovom scenariju najbolje je pričekati da se servis za dodjeljivanje resursa dovrši.

  - Imajte na umu da je naš servis upoznat samo s promjenama korisnika u izvorišnom sustavu (CLOUD HR). U izvorišnom sustavu za Azure AD mora biti valjana promjena da bi se promjena otkrila i strujala u Active Directory.
- Servis za dodjeljivanje resursa procijenio je korisnika i odredio da mu nije dodijeljena dodjela resursa:
  - Ako ste postavili filtar za određivanje opsega utemeljen na atributima, provjerite zadovoljava li korisnik kriterije koje ste naveli.
  - Ako korisnici već postoje u ciljnom sustavu i stanju korisnika u izvorišnom i ciljnom podudaraju, nećemo više ništa poduzeti.
- Servis za dodjeljivanje resursa pokušao je dodijeliti korisniku i nije uspio. U tim scenarijima pregledajte karticu otklanjanje poteškoća i preporuka zapisnika dodjele resursa:
  - Na lokalnom servisu Active Directory ili Azure AD možda nema obaveznog atributa za korisnika. Primjerice, pravila generacije userPrincipalName ili sAMAccountName ne generiraju pravu vrijednost.
  - Odgovarajući atribut (obično employeeId) ne rješava se jedinstvenom korisniku u lokalnom servisu Active Directory ili Azure AD. Na primjer, postoje dva korisnika s istim ID-om zaposlenika u AD-u, a servis vraća kod pogreške koji označava duplicirane ciljne unose za istu izvornu stavku.

Da biste pregledali zapisnike za jednog korisnika i grupe, [pogledajte pregled zapisnika dodjele resursa za problem s određenim korisnikom](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).
