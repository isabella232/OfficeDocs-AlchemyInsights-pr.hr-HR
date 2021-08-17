---
title: Pronalaženje izgubljenih uređaja sa sustavom iOS pomoću aplikacije Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: af747a63caf76e7b4a4a180eaef25dfdf2cb5e3391079c713fe0e413198efb15
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54042298"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Pronalaženje izgubljenih uređaja sa sustavom iOS pomoću aplikacije Intune

Omogućivanje načina rada za izgubljeno na uređaju sa sustavom iOS administratoru omogućuje prikaz poruke i telefonskog broja kontakta na zaključanom zaslonu.

Kada je omogućen način rada za izgubljeno, administrator može koristiti akciju Pronađi uređaj da bi identificirao fizičko mjesto uređaja.

Akcija Pronađi uređaj u aplikaciji Intune funkcionira s uređajima sa sustavom iOS da bi se na karti prikazilo mjesto određenog uređaja.

Pomoću te akcije uređaj sa sustavom iOS mora biti u sljedećem:

- Nadzirani način rada
- Način rada za izgubljeno

Dodatne informacije potražite u članku Omogućivanje izgubljenog načina rada na uređajima sa sustavom [iOS/iPadOS pomoću aplikacije Intune](https://docs.microsoft.com/intune/device-lost-mode) i Pronalaženje izgubljenih ili ukradenih uređaja sa sustavom [iOS/iPadOS pomoću aplikacije Intune](https://docs.microsoft.com/intune/device-locate).

**Najčešća pitanja**

P: izdala sam udaljenu akciju za uklanjanje podataka tvrtke s uređaja, a sada je zapela u stanju čekanja.

O: Da bi se daljinska akcija uspješno dovršila, ciljani uređaj mora biti na mreži i zdrav. U sljedećim situacijama daljinska akcija ostaje u stanju čekanja 30 dana ili dok uređaj ne potvrdi naredbu:

- Kada uređaj nema povezivost
- Kada uređaj izgubi status upravljanja pomoću uređaja Intune

Ako mislite da se uređaj više ne prijavljuje i da neće moći ukloniti podatke tvrtke, odaberite Izbriši. Brisanjem se uklanja zapis uređaja tako da se više ne prikazuje na popisu uređaja Intune. Ako uređaj ponovno postane aktivan, korisnik će ga morati ponovno registrirati.

P: Zašto određene udaljene akcije nisu dostupne za korištenje?

O: Nisu sve platforme podržane za sve radnje na udaljenim uređajima. Sljedeće udaljene akcije specifične su za platformu, pa su dostupne samo za platforme koje su na njima naučene.

- Zaobilaženje zaključavanja aktivacije (samo za iOS)
- Fresh Start (samo Windows)
- Način rada za izgubljeno (samo za iOS)
- Pronalaženje uređaja (samo za iOS)
- Ponovno pokreni (Windows samo)

Dodatne informacije o svakoj radnji potražite u članku [Dostupne akcije uređaja](https://docs.microsoft.com/intune/device-management#available-device-actions).