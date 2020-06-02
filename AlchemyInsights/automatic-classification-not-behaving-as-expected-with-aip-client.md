---
title: Automatsko razvrstavanje ne ponaša prema očekivanjima s AIP klijentom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: 95a994d6a49ee8737a6ebcb196314f92776d8482
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/26/2020
ms.locfileid: "44492960"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatsko razvrstavanje ne ponaša prema očekivanjima s AIP klijentom

Automatsko razvrstavanje koje se ne ponaša prema očekivanjima, koristite sljedeće preporučene smjernice:

1. Ako imate problema s automatskim označavanjem, [pročitajte članak Konfiguriranje uvjeta za automatsku i preporučenu klasifikaciju za zaštitu informacija za Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) i [Što traže vrste osjetljivih informacija](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).
2. Provjerite koristite li pravila s opsegom koja nisu ispravno konfigurirana: [Konfiguriranje pravila zaštite podataka za Azure za određene korisnike pomoću pravila s opsegom](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Ako automatsko označavanje ne funkcionira za Outlook prilikom prilaganja označenog dokumenta, provjerite nije li `DRMEncryptProperty` definirano kao što je ovdje opisano: [Postavke registra IRM-a za sigurnost](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Ako ste [koristili ugrađene vrste informacija](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) za pravila zaštite podataka za Azure, provjerite odgovara li sadržaj očekivanom obliku.
5. Provjerite je li oznaka prikladno konfigurirana za **automatsko** ili **preporučeno**. **(Automatsko** označavanje dostupno je za sve aplikacije sustava Office, dok je **preporučeno** dostupno za sve aplikacije sustava Office osim za Outlook.)
6. Ne možete koristiti automatsku klasifikaciju za dokumente i poruke e-pošte koje su prethodno ručno označene ili prethodno automatski označene višom klasifikacijom.  Dodatne informacije [potražite u odjeljku Kako se primjenjuju automatske ili preporučene oznake](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Ako i dalje imate problema, prikupite zapisnike klijenata za zaštitu podataka usluge Azure i priložite izvezene zapisnike na kartu za podršku. Da biste izvezli zapisnike zaštite podataka usluge Azure:
    - Otvorite dokument sustava Office ili stvorite novu e-poštu u programu Outlook.
    - Kliknite **Zaštiti/osjetljivost**  >  **Pomoć i povratne informacije**.
    - Kliknite **Izvoz zapisnika**.
    - Spremite zapisnike na svoj izbor lokacije i priložite ih zahtjevu za uslugom.

Dodatne informacije potražite u odjeljku:

- [Konfiguriranje uvjeta za automatsku i preporučenu klasifikaciju za zaštitu informacija azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Upute za uobičajene scenarije koji koriste Azure information protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Pregled dokumentacije o zaštiti podataka za Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Pregled pretplata i značajki azure information protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Zahtjevi za zaštitu informacija azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Vodič za brzi početak zaštite informacija za Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Preuzimanje klijenta za zaštitu podataka za Azure](https://www.microsoft.com/download/details.aspx?id=53018)
