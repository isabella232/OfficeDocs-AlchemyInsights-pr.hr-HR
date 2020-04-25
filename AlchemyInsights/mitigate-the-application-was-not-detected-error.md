---
title: Ublažavanje pogreške "Aplikacija nije otkrivena"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810476"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Ublažavanje pogreške "Aplikacija nije otkrivena"

Pogreška prilikom instalacije aplikacije koja glasi "Aplikacija nije otkrivena nakon uspješnog dovršetka instalacije", koju prijavljuje Intune, može se pojaviti u svim većim OS-ovima (Windows, iOS i Android).

Najčešći su scenariji koji generiraju tu pogrešku sljedeći:

- Aplikacija je nakon početne implementacije ažurirana izvan servisa Intune (iz trgovine aplikacija drugog proizvođača). Primjerice, neke aplikacije kao što je Google Chrome mogu provoditi automatska ažuriranja.
- Korisnik je deinstalirao aplikaciju nakon inicijalne instalacije.

Da biste ublažili taj problem, najprije izvršite pregled uređaja na kojima se on pojavljuje i utvrdite scenarij u kojem dolazi do pogreške.

- Ako se aplikacija ažurirala izvan servisa Intune, implementacija aplikacije može se postaviti tako da ignorira verziju aplikacije. Da biste to učinili, u odjeljku **Konfiguracija aplikacije > Informacije o aplikaciji** postavite **Zanemari verziju aplikacije** na **Da**.
- Prilikom ciljanja klijenata može biti primjereno implementirati aplikaciju kao "obaveznu" i osigurati implementaciju najnovije verzije.
- Umjesto toga na platformi iOS može se koristiti funkcija **automatskog ažuriranja** povezana s programom Apple Volume Purchase, koja se može konfigurirati za automatsko ažuriranje na nove verzije aplikacija čim one postanu dostupne.

Dodatne informacije o otklanjanju poteškoća s instalacijom aplikacija potražite u članku [Otklanjanje poteškoća s instalacijom aplikacija](https://docs.microsoft.com/intune/troubleshoot-app-install).
