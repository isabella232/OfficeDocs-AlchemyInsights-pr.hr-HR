---
title: Konfiguriranje servisa za dodjelu resursa
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
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033270"
---
# <a name="configuring-the-provision-service"></a>Konfiguriranje servisa za dodjelu resursa

Da bi automatizirano dodjeljivanje resursa funkcioniralo, za Azure AD potrebne su valjane vjerodajnice koje mu omogućuju povezivanje s API-jem za radne web-servise. Nadalje, gumb Testiraj vezu u aplikaciji Workday to AD User Provisioning provjerava i može li se povezati s agentom za dodjeljivanje resursa servisa Azure AD Povezivanje pridruženom ad domeni.

Ako portal Azure vraća pogrešku prilikom spremanja vjerodajnica, slijedite preporučene korake u nastavku:

1. Provjerite jeste li konfigurirali korisnički račun za integraciju radnog dana kao što je navedeno u odjeljku vodiča [Konfiguriranje korisnika sustava integracije u radni dan](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
2. Provjerite je li servis Azure AD Povezivanje za dodjeljivanje resursa pokrenut na lokalnom poslužitelju Windows putem konzole za upravljanje servisima. Status agenta na portalu Azure možete provjeriti i klikom na gumb Prikaži lokalne agente.
3. Provjerite unosite li vrijednost za polje "Korisničko ime radnog dana" pomoću oblika username@workday-naziv klijenta. Ako nema naziva radnog dana-klijenta, provjera autentičnosti radnog dana ne uspijeva.
4. Ako konfigurirate integraciju s klijentom za implementaciju radnog dana, imajte na umu zakazane sate zastoja klijenta radnog dana. Radni dan zakazao je vrijeme za implementaciju korisnika tijekom vikenda (obično od petka uveče do subote ujutro), a neuspjesi povezivanja tijekom tog razdoblja zastoja poznati su problem koji automatski rješava čim se implementacijski zakupnici ponovno vrate na internet.
5. U rijetkim slučajevima ta vam se pogreška može pojaviti i ako se lozinka korisnika sustava integracije promijenila zbog osvježavanja klijenta ili ako je račun u zaključanom ili isteklom stanju. Provjerite status korisnika sustava integracije s administratorom radnog dana.

Dodatne informacije o konfiguriranju radnog dana za automatizirano dodjeljivanje resursa potražite u članku [Vodič: Konfiguriranje radnog dana za automatsko dodjeljivanje resursa korisnicima.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
