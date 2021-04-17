---
title: 'AIP: pravila se ne ponašaju prema očekivanom'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821619"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: pravila se ne ponašaju prema očekivanom

Azure Information Protection: pravila koja se ne ponašaju prema očekivanom, potražite u nastavku preporučene smjernice za razne probleme s pravilnikom:

1. Ako imate problema s vizualnim oznakama, pregledajte Kada se primjenjuju [vizualne oznake](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Ako imate problema s automatskim označavanjem, pročitajte upute za konfiguriranje uvjeta za automatsku i preporučenu klasifikaciju za [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) i Što [osjetljive vrste podataka izgledaju](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Ako imate problema sa zaštitom Native/Pfile, pregledajte [konfiguraciju API-ja za datoteke.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Provjerite koristite li pravilnike s opsegom koji nisu pravilno konfigurirani: Konfiguriranje pravilnika o zaštiti podataka za Azure za određene korisnike [pomoću pravilnika s opsegom](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Ako automatsko označavanje ne funkcionira za Outlook prilikom prilaganja označenog dokumenta, provjerite nije li DRMEncryptProperty definiran ovdje: [postavke registra IRM za sigurnost](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Ako i dalje nailazite na probleme, prikupite zapisnike klijenta za Azure Information Protection i priložite izvezene zapisnike na ovu kartu.

1. Otvorite dokument sustava Office ili stvorite novu e-poštu u programu Outlook.
2. Kliknite **Zaštita/osjetljivost Pomoć i**  >  **povratne informacije**.
3. Kliknite **Izvezi zapisnike**.
4. Spremite zapisnike na odabir mjesta i priložite ih tom zahtjevu za uslugu.

Dodatni resursi:

- [Konfiguriranje oznake za vizualne oznake za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Pregled dokumentacije za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Korištenje oznaka osjetljivosti u aplikacijama microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

