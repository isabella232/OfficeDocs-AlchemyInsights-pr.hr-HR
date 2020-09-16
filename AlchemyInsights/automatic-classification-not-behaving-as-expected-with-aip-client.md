---
title: Automatska klasifikacija ne ponaša se kao što je očekivano s klijentom za AIP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: d7a2246d78cbd6c4ab40c2a4e5a21807933b619a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715193"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automatska klasifikacija ne ponaša se kao što je očekivano s klijentom za AIP

Automatska klasifikacija ne ponaša se kao što je očekivano, upotrijebite sljedeće preporučene smjernice:

1. Ako imate problema s automatskim označavanju, pročitajte članak [kako konfigurirati uvjete za automatsku i preporučenu klasifikaciju za zaštitu informacija za Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) i [koje vrste osjetljivih podataka traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Provjerite koristite li pravila koja nisu ispravno konfigurirana: [kako konfigurirati pravilnik o zaštiti podataka za Azure za određene korisnike pomoću pravilnika u opsegu](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Ako automatsko označavanje ne funkcionira u programu Outlook prilikom prilaganja označenom dokumentu, provjerite `DRMEncryptProperty` nije li navedeno ovdje: [postavke registra IRM-a za sigurnost](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Ako ste koristili [ugrađene vrste podataka](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) za pravilnik o zaštiti informacija za Azure, provjerite odgovara li vaš sadržaj očekivanom obliku.
5. Provjerite je li naljepnica na odgovarajući način konfigurirana za **Automatsko** ili **preporučeno**. (**Automatsko** označavanje dostupno je za sve aplikacije sustava Microsoft 365, a **preporučeno** je dostupno za sve aplikacije sustava Microsoft 365, osim za Outlook.)
6. Ne možete koristiti automatsku klasifikaciju za dokumente i e-poštu koji su prethodno bili ručno označeni ili prethodno automatski označeni višim klasifikaciji.  Dodatne informacije potražite u članku: [kako se primjenjuju automatske ili preporučene naljepnice](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Ako i dalje nailazite na probleme, prikupite zapisnike o zaštiti podataka za Azure i priložite izvezene zapisnike na karticu za podršku. Da biste izvezli zapisnike o zaštiti informacija o Azuru:
    - Otvaranje dokumenta sustava Office ili stvaranje nove poruke e-pošte u programu Outlook.
    - Kliknite **zaštiti/osjetljivosti**  >  **pomoći i povratnih informacija**.
    - Kliknite **Izvezi zapisnike**.
    - Spremite zapisnike na odabir mjesta i priložite ih na zahtjev za uslugu.

Dodatne informacije potražite u članku:

- [Konfiguriranje uvjeta za automatsku i preporučenu klasifikaciju za zaštitu informacija za Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Vodiči za zajednički scenariji koji koriste zaštitu informacija za Azure](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Pregledajte dokumentaciju o zaštiti informacija za Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Pregled pretplate i značajki za Azure za zaštitu informacija](https://azure.microsoft.com/pricing/details/information-protection)
- [Preduvjeti za zaštitu informacija o Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Vodič za brzi početak za zaštitu informacija za Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Preuzimanje klijenta za zaštitu informacija za Azure](https://www.microsoft.com/download/details.aspx?id=53018)
