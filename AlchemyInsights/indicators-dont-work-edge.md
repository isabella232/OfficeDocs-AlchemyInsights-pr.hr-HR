---
title: Pokazatelji ne funkcioniraju pomoću preglednika Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: 2a48a49ec52a585e450edf448bc9203cd9c3f935
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326253"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Pokazatelji ne funkcioniraju pomoću preglednika Edge

Kada ste stvorili pokazatelj, edge ga ne poštuje (Smartscreen). Dodatne informacije potražite u članku Stvaranje pokazatelja za IP adrese i [URL-ove/domene.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>1. korak: provjerite sljedeće

- Provjerite je li pokazatelj točan (bez pogrešaka u IP/URL-u, ispravna radnja, ispravne RBAC grupe).
- Pričekajte najmanje 2 sata nakon stvaranja pokazatelja da biste u obzir uzmu eventualnu latenciju.
- Provjerite jesu li u programu Microsoft Defender za krajnju točku u sustavu Microsoft Defender.
- Provjerite mogu li ti sustavi komunicirati s oblakom.
- Provjerite je li Smartscreen omogućen i dostupan tako da ode na [probno web-mjesto](https://demo.smartscreen.msft.net).

## <a name="step-2-troubleshoot-the-potential-issue"></a>Drugi korak: otklanjanje poteškoća s potencijalnim problemom

- Provjerite zadovoljava li klijent preduvjete. Detalje potražite u članku [Stvaranje pokazatelja za IP adrese i URL-ove/domene.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Provjerite koristite li najnoviju verziju preglednika Edge. Da biste saznali najnoviju verziju, pogledajte [informacije o verziji programa Microsoft Edge koju imate](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).
- Ponovno pokrenite preglednik Edge.
- Pomaknite se do web-mjesta za koje imate pokazatelj postavljanja. Ako se web-mjesto ne prikazuje očekivano, prijeđite na treći korak. 

## <a name="step-3-collect-data"></a>Treći korak: prikupljanje podataka

- Prikupite **dijagnostičke podatke mdeclientAnalyzer.** Upute potražite u članku [Problemi s uređajem za unošenje u Microsoft Defender za krajnju točku](issues-with-onboarding-machines.md).
- Ako ste zadovoljni instalacijom i prikupljanjem praćenja u aplikaciji Fiddler, pogledajte [Telerik Fiddler](http://www.telerik.com/fiddler).
- Ako želite smjernice Microsoftove podrške, odaberite ikonu Podrške u nastavku da biste otvorili slučaj podrške.
