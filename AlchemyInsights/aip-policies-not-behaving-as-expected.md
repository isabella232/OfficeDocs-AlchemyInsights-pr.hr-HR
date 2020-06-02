---
title: 'AIP: Pravila se ne ponašaju prema očekivanjima'
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
- "4780"
ms.openlocfilehash: 7926ff9ebbd54969fb5b3ae5d909baffe96a4292
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/26/2020
ms.locfileid: "44492954"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Pravila se ne ponašaju prema očekivanjima

Azure Information Protection: Pravila se ne ponašaju prema očekivanjima, pogledajte sljedeće za preporučene smjernice za različite probleme s pravilima:

1. Ako imate problema s vizualnim oznakama, pregledajte [Kada se primjenjuju vizualne oznake](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Ako imate problema s automatskim označavanjem, pregledajte [Kako konfigurirati uvjete za automatsku i preporučenu klasifikaciju za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) i Što traže vrste [osjetljivih informacija](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).
3. Ako imate problema s zaštitom nativnog/pfile, pregledajte [konfiguraciju API-ja datoteka](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Provjerite koristite li pravila s opsegom koja nisu ispravno konfigurirana: [Konfiguriranje pravila zaštite podataka za Azure za određene korisnike pomoću pravila s opsegom](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Ako automatsko označavanje ne funkcionira za Outlook prilikom prilaganja označenog dokumenta, provjerite nije li DRMEncryptProperty definiran kao što je ovdje opisano: [Postavke registra IRM-a za sigurnost](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Ako i dalje imate problema, prikupite zapisnike klijenata za zaštitu podataka usluge Azure i priložite izvezene zapisnike ovoj karti.

1. Otvorite dokument sustava Office ili stvorite novu e-poštu u programu Outlook.
2. Kliknite **Zaštiti/osjetljivost**  >  **Pomoć i povratne informacije**.
3. Kliknite **Izvoz zapisnika**.
4. Spremite zapisnike na svoj izbor lokacije i priložite ih ovom zahtjevu za uslugom.

Dodatni resursi:

- [Konfiguriranje oznake za vizualne oznake za zaštitu informacija za Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Pregled dokumentacije o zaštiti podataka za Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Korištenje oznaka osjetljivosti u aplikacijama sustava Office](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

