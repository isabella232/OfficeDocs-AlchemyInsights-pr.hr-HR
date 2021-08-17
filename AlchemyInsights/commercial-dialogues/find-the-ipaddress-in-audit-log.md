---
title: Pronalaženje IP adrese u zapisniku nadzora
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 258e92368b8a33e8ea807f0cb9af90132c86ed5b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58303569"
---
# <a name="find-the-ip-address-in-audit-log"></a>Pronalaženje IP adrese u zapisniku nadzora

IP adresa koja odgovara aktivnosti koju je izveo korisnik ili administrator prikazuje se u zapisnicima nadzora. Zapisuje se i podaci o klijentu. Evo kako prepoznati IP adresu:

1. Učinite jednu od sljedećih akcija:
   - U Centar za usklađenost okruženja Microsoft 365 na <https://compliance.microsoft.com> idite na **Nadzor** \> **rješenja**. Možete i izravno pristupiti stranici **Nadzor** pomoću sustava <https://compliance.microsoft.com/auditlogsearch> .
   - Na portalu Microsoft 365 Defender idite <https://security.microsoft.com> na **Nadzor**. Možete i izravno pristupiti stranici **Nadzor** pomoću sustava <https://security.microsoft.com/auditlogsearch> .

    **Napomena:** ako vidite obavijest da morate uključiti nadzor, odmah je uključite. Ako ta značajka nije omogućena, rezultati pretraživanja neće moći povući podatke iz prethodnih datuma.

2. Na **stranici** Nadzor provjerite je li **odabrana** kartica Pretraživanje, a zatim konfigurirajte sljedeće postavke:
   - **Raspon datuma i vremena:** odaberite raspon datuma/vremena u **okvirima Početak** **i** Kraj.
   - **Aktivnosti**: ako vas zanima određena aktivnost, odaberite je s popisa; U suprotnom će zadana vrijednost **Pokaži rezultate za sve aktivnosti** vratiti sve aktivnosti. Imajte na umu da određene aktivnosti možda nisu dostupne za odabir; No te će stavke nadzora biti vraćene ako **je odabrana** stavka Prikaži rezultate za sve aktivnosti.
   - **Korisnici:** prihvatite praznu zadanu vrijednost da biste vratili rezultate za sve korisnike ili unesite jednog ili više korisnika.

3. Kada završite, kliknite **Pretraživanje**. Aktivnosti se prikazuju na novoj stranici **pretraživanja nadzora.**

4. U rezultatima kliknite Filtriraj rezultate **i** u okvir filtar aktivnosti **upišite Set-Mailbox.**

5. Odaberite zapis nadzora u rezultatima da biste otvorili **letak** Detalji.

Dodatne informacije potražite u članku Pretraživanje [zapisnika nadzora da biste istražili uobičajene probleme s podrškom](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios).
