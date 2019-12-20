---
title: Rješavanje problema s zvukom u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 46b23f97c2e682258224dc95e7a76b1201991828
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796011"
---
# <a name="troubleshooting-audio-problems-in-windows-10"></a>Rješavanje problema s zvukom u sustavu Windows 10

**Pokretanje alata za otklanjanje poteškoća s zvukom**

Alat za otklanjanje poteškoća s zvukom možda može automatski ispraviti probleme s zvukom: 

1. Odaberite **Start**, upišite **Otklanjanje poteškoća**, a zatim odaberite **Otklanjanje poteškoća** s popisa rezultata. 
2. Odaberite **Reprodukcija audiozapisa** > **Pokreni alat za otklanjanje poteškoća**.

**Provjerite kabele, glasnoću, zvučnike i slušalice**

- Provjerite ima li zvučnik i slušalice veze za labave kabele i provjerite jesu li spojeni na ispravan priključak.
- Provjerite razinu napajanja i glasnoće i pokušajte pretvoriti sve kontrole glasnoće.
- Neki zvučnici i aplikacije imaju svoje kontrole glasnoće, i možda ćete morati provjeriti sve kako bi bili sigurni da su na pravom nivou.
- Pokušajte povezati pomoću drugog USB priključka.
- **Napomena:** Sjetite se da zvučnici možda neće raditi kada su priključene slušalice.

**Provjeri upravitelja uređaja**

Da biste bili sigurni da su upravljački programi ažurirani:

- Odaberite **Start**, upišite **Upravitelj uređaja**, a zatim odaberite **Upravitelj uređaja** s popisa rezultata.

2. U odjeljku **Kontroleri zvuka, videozapisa i igre**Odaberite zvučnu karticu, otvorite je, odaberite karticu **upravljački program** i odaberite **Ažuriraj upravljački program**. 

**Napomena:** Ako Windows ne pronađe novi upravljački program, potražite ga na web-mjestu proizvođača uređaja i slijedite njihove upute.

**Ponovna instalacija upravljačkog programa**

Ako ne možete ažurirati putem upravitelja uređaja ili pronaći novi upravljački program na web-mjestu proizvođača, pokušajte ove korake: 

1. U upravitelju uređaja desnom tipkom miša kliknite (ili pritisnite i držite) upravljački program za audio i odaberite **Deinstaliraj**. Ponovno pokrenite uređaj i Windows će pokušati ponovno instalirati upravljački program.

2. Ako ponovna instalacija upravljačkog programa ne radi, pokušajte koristiti generički upravljački program za audiozapise koji dolazi sa sustavom Windows. U upravitelju uređaja desnom tipkom miša kliknite (ili pritisnite i držite) vaš upravljački program za audio > **Update Driver softver** > **Pregledajte moje računalo za upravljački** > program**Dopustite mi da izaberem s popisa upravljačkih programa uređaja na računalu**, odaberite **audiouređaj visoke razlučivosti**, odaberite **dalje**i slijedite upute da biste ga instalirali.

**Postavljanje zadanog uređaja**

Ako se priključujete na audio uređaj pomoću USB ili HDMI, možda ćete morati postaviti taj uređaj kao zadani: 

1. Odaberite **Start**, upišite **zvuk**, a zatim odaberite **zvuk** ili **Promjena zvukova sustava** s popisa rezultata.

2. Na kartici **Reprodukcija** odaberite uređaj, odaberite **Postavi zadano**, a zatim odaberite **u redu**.

