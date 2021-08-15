---
title: Automatska klasifikacija ne ponaša se prema očekivanom s klijentom AIP-a
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
- "4373"
ms.openlocfilehash: 93d15b8b65fd52a567ecbb6e1f84363bf2b38946c105896b0b5ef41e49d16ea9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53979701"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatska klasifikacija ne ponaša se prema očekivanom s klijentom AIP-a

Automatska klasifikacija ne ponaša se prema očekivanom, koristite sljedeće preporučene smjernice:

1. Ako imate problema s automatskim označavanjem, pogledajte upute za konfiguriranje uvjeta za automatsku i preporučenu klasifikaciju za [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) i Što [osjetljive vrste podataka izgledaju](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Provjerite koristite li pravilnike s opsegom koji nisu pravilno konfigurirani: Konfiguriranje pravilnika o zaštiti podataka za Azure za određene korisnike [pomoću pravilnika s opsegom](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Ako automatsko označavanje ne funkcionira za Outlook pri prilaganju dokumenta s oznakom, provjerite nije li to definirano na sljedeći `DRMEncryptProperty` način: [postavke registra IRM-a za sigurnost](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Ako ste za pravilnik o [zaštiti podataka](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) na servisu Azure koristili ugrađene vrste podataka, provjerite podudara li se sadržaj s očekivanim oblikom.
5. Provjerite je li naljepnica pravilno konfigurirana za automatsko **ili** **preporučeno**. (**Automatsko** označavanje dostupno je za sve Microsoft 365  aplikacije, dok je preporučeno dostupno za sve aplikacije Microsoft 365 osim za Outlook.)
6. Ne možete koristiti automatsku klasifikaciju za dokumente i poruke e-pošte koje su prethodno bile ručno označene ili prethodno automatski označene višom klasifikacijom.  Dodatne informacije potražite u članku Kako se [primjenjuju automatske ili preporučene naljepnice.](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)
7. Ako i dalje nailazite na probleme, prikupite zapisnike klijenta za Azure Information Protection i priložite izvezene zapisnike na kartu za podršku. Da biste izvezli zapisnike za Azure Information Protection:
    - Otvorite dokument Office ili stvorite novu e-poštu u Outlook.
    - Kliknite **Zaštita/osjetljivost Pomoć i**  >  **povratne informacije**.
    - Kliknite **Izvezi zapisnike**.
    - Spremite zapisnike na odabir lokacije i priložite ih zahtjevu za uslugu.

Dodatne informacije potražite u sljedećem članku:

- [Konfiguriranje uvjeta za automatsku i preporučenu klasifikaciju za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Vodiči za uobičajene scenarije koji koriste Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Pregled dokumentacije za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Pregled pretplata i značajki za Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)
- [Preduvjeti za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Vodič za brzi početak za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Preuzimanje klijenta za Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
