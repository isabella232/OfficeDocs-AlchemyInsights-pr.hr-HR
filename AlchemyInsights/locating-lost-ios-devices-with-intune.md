---
title: Pronalaženje izgubljenih iOS uređaja s intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438906"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Pronalaženje izgubljenih iOS uređaja s intune

Omogućivanje izgubljenog načina rada na iOS uređaju administratoru omogućuje prikaz poruke i telefonskog broja za kontakt na zaključanom zaslonu.

Nakon što je omogućen izgubljeni način rada, administrator može koristiti akciju Pronađi uređaj za identifikaciju fizičke lokacije uređaja.

Akcija Pronađi uređaj u aplikaciji Intune radi s uređajima sa sustavom iOS kako bi se prikazala lokacija određenog uređaja na karti.

Za korištenje ove akcije potreban je iOS uređaj:

- Nadzirani način rada
- Način izgubljenog

Dodatne informacije [potražite u odjeljku Omogućivanje izgubljenog načina rada na iOS/iPadOS uređajima s intune](https://docs.microsoft.com/intune/device-lost-mode) i [pronalaženje izgubljenih ili ukradenih iOS/iPadOS uređaja s intune](https://docs.microsoft.com/intune/device-locate).

**Najčešća pitanja**

P: Izdao sam udaljenu akciju za uklanjanje podataka tvrtke s uređaja, a sada je zapela u stanju na čekanju.

O: Da bi se daljinsko dovršavanje uspješno dovršilo, ciljani uređaj mora biti na mreži i zdrav. U sljedećim situacijama udaljena akcija ostaje u stanju na čekanju 30 dana ili dok uređaj ne potvrdi naredbu:

- Kada uređaj nema
- Kada uređaj izgubi status upravljanja intune

Ako mislite da se uređaj više ne prijavljuje i da neće moći ukloniti podatke tvrtke, odaberite Izbriši. Brisanjem se uklanja zapis uređaja tako da se više ne pojavljuje na popisu Intune uređaja. Ako uređaj ponovno postane aktivan, korisnik će ga morati ponovno prijaviti.

P: Zašto određene udaljene radnje nisu dostupne za korištenje?

O: Ne podržavaju sve platforme sve akcije udaljenog uređaja. Sljedeće udaljene radnje specifične su za platformu, tako da su dostupne samo za navedene platforme.

- Zaobilaženje zaključavanja aktivacije (samo iOS)
- Novi početak (samo windows)
- Način izgubljenog načina rada (samo iOS)
- Pronalaženje uređaja (samo iOS)
- Ponovno pokretanje (samo windows)

Dodatne pojedinosti o svakoj radnji [potražite u odjeljku Dostupne radnje uređaja](https://docs.microsoft.com/intune/device-management#available-device-actions).