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
ms.openlocfilehash: 70f12328813a312631c67cd72cc75559ed2eca1b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675148"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Pronalaženje izgubljenih uređaja sa sustavom iOS pomoću aplikacije Intune

Omogućivanje Izgubljenog načina rada na uređaju sa sustavom iOS administrator ima poruku i telefonski broj kontakta koji se prikazuje na zaključanom zaslonu.

Nakon omogućivanja izgubljenog načina rada administrator može identificirati fizičku lokaciju uređaja pomoću akcije pronađite uređaj.

Akcija pronađite uređaj u programu Intune radi s uređajima sa sustavom iOS da bi se prikazalo mjesto određenog uređaja na karti.

Pomoću ove akcije potreban je uređaj sa sustavom iOS:

- Nadzirani način rada
- Izgubljeni način rada

Dodatne informacije potražite u članku [omogućivanje Izgubljenog načina rada na uređajima sa sustavom iOS/ipados pomoću aplikacije Intune](https://docs.microsoft.com/intune/device-lost-mode) i [pronalaženje izgubljenih ili ukradenih uređaja sa sustavom iOS/Ipados pomoću aplikacije Intune](https://docs.microsoft.com/intune/device-locate).

**Najčešća pitanja**

P: izdala sam daljinsku akciju za uklanjanje podataka tvrtke s uređaja, a sada je zaglavljena u stanju neriješenog.

O: da bi se daljinska akcija uspješno dovršena, ciljani uređaj mora biti online i zdrav. U sljedećim situacijama daljinska akcija ostaje u stanju neriješenog tijekom 30 dana ili dok uređaj ne potvrdi naredbu:

- Kada uređaj nema povezivost
- Kada uređaj izgubi status upravljanja pomoću aplikacije Intune

Ako mislite da se uređaj više ne prijavljuje i da neće moći ukloniti podatke tvrtke, odaberite Izbriši. Brisanjem se uklanja zapis uređaja tako da se više ne prikazuje na popisu Intune na uređajima. Ako uređaj ponovno postane aktivan, njezin će ga korisnik morati ponovno prijaviti.

P: zašto određene udaljene akcije nisu dostupne za korištenje?

O: nisu sve platforme podržavaju sve akcije udaljenog uređaja. Sljedeće udaljene akcije specifične su za platformu, pa su dostupne samo za navedene platforme.

- Zaobilaženje aktivacije za aktivaciju (samo sa sustavom iOS)
- Novi Start (samo u sustavu Windows)
- Izgubljeni način rada (samo sa sustavom iOS)
- Pronađite uređaj (samo za iOS)
- Ponovno pokretanje (samo u sustavu Windows)

Dodatne informacije o svakoj akciji potražite u članku [dostupne akcije uređaja](https://docs.microsoft.com/intune/device-management#available-device-actions).