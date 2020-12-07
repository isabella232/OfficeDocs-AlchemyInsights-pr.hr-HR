---
title: Podrška za Microsoft Edge radi zaštite aplikacija za Microsoft Defender
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583251"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Podrška za Microsoft Edge radi zaštite aplikacija za Microsoft Defender

Dizajniran za Windows 10 i Microsoft Edge, čuvar aplikacije koristi hardver-izolaciju pristup koji omogućuje korisniku navigaciju nepouzdano web-mjesto unutar izoliranog, Hyper-V – omogućenog spremnika, razdvojenog od glavnog operacijskog sustava.

Administrator tvrtke definira popis pouzdanih web-mjesta, resursa u oblaku i interne mreže. Kada korisnik posjeti web-mjesto koje se ne nalazi na popisu, Microsoft Edge otvorit će web-mjesto u spremniku. To znači da ako se prikaže zlonamjerno web-mjesto, glavno računalo ostat će zaštićeno, a napadač neće doći do podataka tvrtke.

Instalacija proširenja u spremniku podržana je kao Microsoft Edge verzija 81 i može se kontrolirati putem pravilnika. Adresa updateURL koja se koristi u pravilima ExtensionInstallForcelist trebala bi biti dodana kao neutralni resurs u pravilima izolacije mreže koju koristi čuvar aplikacije.

Dodatne informacije potražite u [članku Podrška za Microsoft Edge za čuvara aplikacija za Microsoft Defender](https://go.microsoft.com/fwlink/?linkid=2134229).
