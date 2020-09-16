---
title: 'AIP: pravila se ne ponašaju kao što je očekivano'
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
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663181"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: pravila se ne ponašaju kao što je očekivano

Zaštita informacija o Azure: pravila se ne ponašaju kao što je očekivano, pročitajte sljedeće za preporučene smjernice za razne probleme s politikom:

1. Ako nailazite na probleme s vizualnim oznakama, pregledajte [kada se primjenjuju vizualne oznake](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Ako imate problema s automatskim označavanju, pregledajte [način konfiguriranja uvjeta za automatsku i preporučenu klasifikaciju za zaštitu informacija za Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) te [koje vrste osjetljivih podataka traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Ako imate problema s zaštitom izvornih/Pdatoteka, pročitajte [konfiguraciju datoteka API](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)-ja.
4. Provjerite koristite li pravila koja nisu ispravno konfigurirana: [kako konfigurirati pravilnik o zaštiti podataka za Azure za određene korisnike pomoću pravilnika u opsegu](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Ako automatsko označavanje ne funkcionira u programu Outlook prilikom prilaganja označenom dokumentu, provjerite ne definira li se funkcija DRMEncryptProperty kao što je opisano ovdje: [postavke registra IRM-a za sigurnost](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Ako i dalje nailazite na probleme, prikupite zapisnike o zaštiti podataka za Azure i priložite izvezene zapisnike na ovu ulaznicu.

1. Otvaranje dokumenta sustava Office ili stvaranje nove poruke e-pošte u programu Outlook.
2. Kliknite **zaštiti/osjetljivosti**  >  **pomoći i povratnih informacija**.
3. Kliknite **Izvezi zapisnike**.
4. Spremite zapisnike na odabir mjesta i priložite ih na ovaj zahtjev za servis.

Dodatni resursi:

- [Konfiguriranje natpisa za vizualne oznake za zaštitu informacija za Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Pregledajte dokumentaciju o zaštiti informacija za Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Korištenje naljepnica s osjetljivosti u aplikacijama Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

