---
title: Primjer Microsoft Defender za Office 365 anti-phishing pravilnik
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743896"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Primjer Microsoft Defender za Office 365 anti-phishing pravilnik

Ove postavke omogućuju politiku zvanu *domena i izvršni direktor*. Ovo pravilo omogućuje oponašanje korisnika i domene, a zatim pravilnik primjenjuje na sve e-poštu primljene od korisnika unutar domene. Najprije dodajte sljedeće podatke da biste stvorili pravilo:

- **Naziv**: domena i ceo **Opis**: osigurava da se izvršni direktor i vaša domena ne oponašate.
  **Primijenjena na**: odaberite **domenu primatelja**. U odjeljku **bilo koji od ovih** mogućnosti odaberite **Odaberi**, a zatim odaberite domenu. Odaberite **+ Dodaj**. Potvrdite okvir pokraj naziva domene na popisu (na primjer, *contoso.com*), a zatim odaberite **Dodaj**. Odaberite **gotovo**.
- Nakon stvaranja pravilnika možete precizno podesiti pravilo pomoću sljedećih mogućnosti:
  - **Dodavanje korisnika u zaštitu:** U ovom primjeru na minimum dodajte adresu e-pošte glavnog direktora.
  - **Dodajte domene koje treba štititi**: Dodajte organizacijsku domenu koja obuhvaća ured izvršnog direktora.
  - **Odaberite akcije**: **Ako je e-pošta poslao imitirani korisnik**, odaberite **Preusmjeri poruku na drugu adresu e-pošte**, a zatim unesite adresu e-pošte sigurnosnog administratora (na primjer, *securityadmin@contoso.com*). **Ako je e-pošta poslala imitirana domena**, odaberite **karantensku poruku**.
  - **Inteligencija poštanskog sandučića**: po zadanom je odabrana ta mogućnost prilikom stvaranja novog pravilnika o krađi identiteta. Ovu **postavku ostavite radi najboljih** rezultata.
  - **Dodavanje pouzdanih pošiljatelja i domena:** U ovom primjeru nemojte definirati prekoračenja.
- Kada pregledate postavke, odaberite **Stvori ovo pravilo** ili **Spremi**, po potrebi.

Dodatne informacije potražite u članku [politika suzbijanja krađe identiteta u programu Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
