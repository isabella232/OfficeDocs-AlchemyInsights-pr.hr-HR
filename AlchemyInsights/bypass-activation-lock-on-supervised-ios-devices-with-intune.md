---
title: Zaobići potaknuće zaključati na nadzirani iOS sprava sa Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423367"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Zaobići potaknuće zaključati na nadzirani iOS sprava sa Intune

Mogućnost zaobilaženja zaključavanja aktivacije na iOS uređajima olakšava oporavak od scenarija u kojem korisnik omogućuje zaključavanje aktivacije na korporativnom uređaju, a zatim napušta tvrtku.

Preduvjeti za zaobilaženje zaključavanja aktivacije uključuju:

- Uređaj je da je "pod nadzorom."
- Zaključavanje aktivacije uspješno je omogućeno pomoću pravila ograničenja iOS uređaja u sustavu Intune.

Osim toga, prilikom zaobilaženja zaključavanja aktivacije trebali biste:

- Fizički posjedujete uređaj koji se briše.
- Kopirajte kôd prije nego što izdate brisanje.

**Napomena:** Kôd za brisanje ne razlikuje velika i mala slova, pa znakovi "-" nisu potrebni.

Pojedinosti potražite [u odjeljku Zaobilaženje zaključavanja aktivacije na nadziranim iOS uređajima pomoću mogućnosti Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**Najčešća pitanja**

P: **Izdao sam udaljenu akciju za uklanjanje podataka tvrtke s uređaja, a sada je zapela u stanju na čekanju.**

O: Da bi se daljinsko dovršavanje uspješno dovršilo, ciljani uređaj mora biti na mreži i zdrav. U sljedećim situacijama udaljena akcija ostaje u stanju na čekanju 30 dana ili dok uređaj ne potvrdi naredbu kada uređaj:

- Nema veze.
- Gubi svoj status upravljanja s Intune.

Ako mislite da se uređaj više ne prijavljuje i da neće ukloniti podatke tvrtke, odaberite Izbriši. Brisanjem se uklanja zapis uređaja tako da se više ne pojavljuje na popisu Intune uređaja. Da bi uređaj ponovno postao aktivan, njegov korisnik mora ponovno prijaviti uređaj.

P: **Zašto određene udaljene radnje nisu dostupne za korištenje?**

O: Ne podržavaju sve platforme sve akcije udaljenog uređaja. Sljedeće udaljene radnje specifične su za platformu.

- Zaobilaženje zaključavanja aktivacije (samo iOS)
- Novi početak (samo windows)
- Način izgubljenog načina rada (samo iOS)
- Pronalaženje uređaja (samo iOS)
- Ponovno pokretanje (samo windows)

Dodatne pojedinosti o svakoj radnji [potražite u odjeljku Dostupne radnje uređaja](https://docs.microsoft.com/intune/device-management#available-device-actions).