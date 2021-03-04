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
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429469"
---
# <a name="problem-with-single-user"></a>Problem s jednim korisnikom

- Korisniku možda nije dodijeljena dodjela resursa jer servis još nije imao priliku procijeniti korisnika. Pregledajte upute o tome koliko traje dodjela resursa, kao i traka tijeka na stranici Konfiguracija dodjele resursa. Ako je stanje stanja koje je navedeno u odjeljku Dodatne pojedinosti prije datuma kada je korisnik stvoren/ažuriran/izbrisan, to znači da još nismo procijenili korisnika. U ovom scenariju najbolje je čekati da servis za dodjelu resursa završi.

  - Imajte na umu da je naš servis svjestan samo promjena korisnika u izvornom sustavu (Cloud HR). Mora postojati valjana promjena u izvornom sustavu za Azure AD za prepoznavanje promjene i njihovo strujanje u Active Directory.
- Servis za dodjelu resursa procijenio je korisnika i utvrdio da mu se ne treba dodijeliti:
  - Ako ste postavili filtar zasnovan na atributu, Provjerite zadovoljava li korisnik kriterij koji ste naveli.
  - Ako korisnici već postoje u ciljnom sustavu i stanju korisnika u izvoru i ciljnom podudaranju, nećemo poduzeti nikakve daljnje akcije.
- Servis za dodjelu resursa pokušao je dodijeliti korisniku i nije uspio. U tim scenarijima Pregledajte karticu Otklanjanje poteškoća i preporuke u zapisnicima za dodjelu resursa:
  - Potreban atribut na korisniku možda nema u lokalnom servisu Active Directory ili Azure AD. Primjerice, pravila stvaranja userPrincipalName ili sAMAccountName ne stvaraju pravu vrijednost.
  - Podudarni atribut (obično IDZaposlenika) ne rješava jedinstven korisnik u lokalnom servisu Active Directory ili Azure AD. Na primjer, postoje dva korisnika s istim Zaposlajnim osobama u aplikaciji AD, a servis vraća šifru pogreške koja označava duplicirane ciljne unose za isti izvorni unos.

Da biste pregledali zapisnike za pojedinačne korisnike i grupe, pročitajte članak [Pregled zapisnika dodjele resursa za problem s određenim korisnikom](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).
