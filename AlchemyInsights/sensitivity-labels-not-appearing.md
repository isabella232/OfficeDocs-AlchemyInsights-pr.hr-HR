---
title: Oznake osjetljivosti ne prikazuju se
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
- "1778"
- "9000181"
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061424"
---
# <a name="sensitivity-labels-not-appearing"></a>Oznake osjetljivosti ne prikazuju se

Oznake osjetljivosti omogućuju vam klasificiranje i zaštitu osjetljivog sadržaja. Mogu se stvoriti u centru za Centar za usklađenost okruženja Microsoft 365, Microsoft 365 sigurnosti ili centru za Microsoft 365 za & u odjeljku Oznake > osjetljivosti. Dodatne informacije o ovoj značajki potražite u članku [Pregled oznaka osjetljivosti](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Ako ste konfigurirali oznake osjetljivosti, ali se ne prikazuju u aplikacijama Microsoft 365, provjerite sljedeće:

- Provjerite je li oznaka osjetljivosti [objavljena](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) korisnicima i grupama koje želite.

- Provjerite koristi li korisnik aplikaciju koja podržava oznake osjetljivosti – pogledajte oznake [osjetljivosti u dokumentu](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Ako migrirate [oznake azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), imajte na umu ovdje navedene [napomene](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Podrška za sprječavanje gubitka podataka (DLP): trenutno se samo oznake zadržavanja mogu koristiti kao uvjet u pravilnikima DLP-a.  Podrška za oznake osjetljivosti u pravilniku o DLP-u još nije dostupna, ali radimo na tome.

- Kada je šifriranje omogućeno na oznaci osjetljivosti, možete odabrati sljedeće:
    - Dodjela dozvola odmah
    - Korisnicima dodijelite dozvole


Dodatne informacije o mogućim problemima potražite u članku [Poznati problemi s oznakama osjetljivosti](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).