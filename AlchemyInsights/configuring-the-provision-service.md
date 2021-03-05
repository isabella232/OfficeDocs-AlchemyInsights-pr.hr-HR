---
title: Konfiguriranje servisa za pružanje resursa
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
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481344"
---
# <a name="configuring-the-provision-service"></a>Konfiguriranje servisa za pružanje resursa

Da bi automatizirani korisnici mogli funkcionirati, za Azure AD potrebna su valjana vjerodajnica koja omogućuje povezivanje s API-jem WORKDAY tkanje Services. Nadalje, gumb Testiraj vezu na radni dan u aplikaciji za dodjelu korisničkih resursa oglašava se i potvrđuje ako se može povezati s agentom za dodjelu resursa za Azure AD Connect u domenu oglasa.

Ako se na portalu Azure vraća pogreška prilikom spremanja vjerodajnica, slijedite preporučene upute u nastavku:

1. Potvrdite da ste konfigurirali korisnički račun za sustav integracije WORKDAY kao što je navedeno u odjeljku udžbenik [konfigurirajte korisnika sustava integracija u radnom danu](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
2. Potvrdite da je servis Azure AD Connect agent za dodjelu resursa instaliran i pokrenut na lokalnom sustavu Windows Server pomoću konzole za upravljanje servisima. Možete i provjeriti status agenta na portalu Azure tako da kliknete gumb Prikaz lokalnih agenata.
3. Uvjerite se da unosite vrijednost u polje "WORKDAY username" pomoću oblika username@workday-naziv korisnika. Ako nedostaje radni dan-naziv korisnika, provjera autentičnosti radnog dana neće uspjeti.
4. Ako konfigurirate integraciju s klijentom za provedbu radnog dana, primjetite zakazane sate zastoja u svom radnom danu. WORKDAY je zakazano vrijeme za provedbu stanara tijekom vikenda (obično od petka navečer do subote ujutro) i pogreške pri povezivosti tijekom ove pauze prozor je poznat problem koji automatski rješava čim se ponovno implementiraju stanari u mreži.
5. U rijetkim slučajevima možete vidjeti i ovu pogrešku ako je lozinka korisnika sustava integracije promijenjen zbog osvježavanja gosta ili ako je račun zaključan ili isteklog stanja. Provjerite status korisnika sustava integracija sa svojim administratorom radne dane.

Dodatne informacije o konfiguriranju radnog dana za automatiziranu dodjelu resursa potražite u članku [Udžbenik: Konfiguriranje radnog dana za automatsku dodjelu korisnika](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
