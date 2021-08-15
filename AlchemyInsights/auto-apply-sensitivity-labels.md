---
title: Automatska primjena oznaka osjetljivosti
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1737"
- "9000181"
ms.openlocfilehash: 7a32ad52f115b9ada40f7cd47c90ceb3dcd3f9cd99a8f9eae3514b2e45e73bb8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53969274"
---
# <a name="auto-apply-sensitivity-labels"></a>Automatska primjena oznaka osjetljivosti

Oznake osjetljivosti korisnici mogu ručno primijeniti na sadržaj ili ih možete konfigurirati tako da se automatski primjenjuju na sadržaj.

Automatskom primjenom oznaka osjetljivosti uklanja se potreba za obučavanje korisnika o klasificiranju sadržaja i potrebi da ih obavijestite o konfiguracijama pravilnika.

Da biste automatski primijenili naljepnice, potrebno je sljedeće:

- Pretplata na Azure Information Protection P2
- [Preuzimanje i instalacija klijenta za sjedinjeno označavanje servisa Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/install-unifiedlabelingclient-app)

Radimo na nativnoj podršci koja u budućnosti neće zahtijevati klijent za sjedinjeno označavanje azure Information Protection.

Trenutno samo Windows podržava klijent za sjedinjeno označavanje.  Značajka još nije podržana na Macu, iOS-u i Androidu.

Dodatne informacije o oznakama osjetljivosti i automatskoj primjeni na sadržaj potražite u članku:

- [Pregled oznaka osjetljivosti](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)
- [Automatska primjena oznake osjetljivosti na sadržaj](https://docs.microsoft.com/microsoft-365/compliance/apply-sensitivity-label-automatically)