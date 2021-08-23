---
title: Želite li Microsoftu prijaviti neželjenu poštu koja je lažno pozitivna?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396607"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Imate li valjane poruke koje su označene kao neželjena e-pošta?

Frustrirajuće je kada legitimna poruka e-pošte završi u mapi Bezvrijedno ili u karanteni. Uzmite u obzir sljedeće najčešće razloge za lažno pozitivan rezultat:

**Nadjačavanja klijenta (najčešće)** To je u potpunosti unutar vaše kontrole radi otklanjanja poteškoća.

Pošaljite poruku na Microsoft 365 Defender za analizu utjecaja na pravilnike i pravila; pojedinosti o ponovnom oknu dostupne su u roku od nekoliko minuta.
Pregledajte ili izmijenite pravilnike ili pravila prema potrebi. 

**Nadjačavanja krajnjeg korisnika (često)** To je u potpunosti unutar vaše kontrole radi otklanjanja poteškoća. 

Pošaljite poruku na Microsoft 365 Defender za analizu utjecaja na pravilnike i pravila; pojedinosti o ponovnom oknu dostupne su u roku od nekoliko minuta. 

Ako je poruka blokirana jer je poslana s adrese na korisnikov popis blokiranih pošiljatelja, zaglavlja obuhvaćaju presudu filtriranja neželjene pošte "SFV:BLK".

**Provjera autentičnosti e-pošte pošiljatelja** To je djelomično unutar vaše kontrole radi otklanjanja poteškoća.

Pošaljite poruku da biste analizirali pogreške u provjeri autentičnosti e-pošte pošiljatelja u trenutku isporuke; rezultati su dostupni u roku od jednog dana. 

Ako ste vlasnik infrastrukture za slanje, pregledajte kako je uskladiti sa SPF-om, DKIM-om i DMARC-om da biste bili sigurni da odredišni sustavi e-pošte šalju poruke poslane s vaše domene. Umjesto toga, obratite se pošiljateljima da biste se obratili njihovim KONFIGURACIJAMA DNS-a.

**Microsoftovo filtriranje presudi** To je djelomično unutar vaše kontrole radi otklanjanja poteškoća.

Pošaljite poruku i prijavite poruku kao sigurnu; rezultati pretraživanja dostupni su u roku od jednog dana. Popis dopuštenih/blokiranih klijenta koristite kada se ne slažete s filtriranjem presudi u određenim situacijama. No ne biste trebali trajno zaobići Microsoftovo filtriranje presudi. 

Dodatne informacije potražite u sljedećim člancima:

- Omogućite krajnjim korisnicima slanje poruka Microsoftu. Microsoft koristi te podneske da bi poboljšao učinkovitost tehnologija zaštite e-pošte, a prikazuju se u izvješćima za slanje koje možete koristiti kao pokazatelj za ažuriranje pravilnika. 

- Da biste vidjeli kratki videozapis o slanjem poruka radi analize, pogledajte [slanje poruka radi analize](https://go.microsoft.com/fwlink/?linkid=2166435).

- [Slanje sumnjive neželjene pošte, phish, URL-ova i datoteka pomoću slanja administratora Microsoftu](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Upravljanje popisom dopuštenih/blokiranih klijenta](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Zaglavlja poruka o neželjenoj pošti u Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Zaštita od odlazne neželjene pošte u programu EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)