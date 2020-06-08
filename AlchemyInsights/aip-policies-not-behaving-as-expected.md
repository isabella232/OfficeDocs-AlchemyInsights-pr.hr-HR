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
ms.openlocfilehash: 91308850c06485bdd11e81bd130770aefb247118
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580757"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Pravila se ne ponašaju prema očekivanjima

Azure Information Protection: Pravila se ne ponašaju prema očekivanjima, pogledajte sljedeće za preporučene smjernice za različite probleme s pravilima:

1. Ako imate problema s vizualnim oznakama, pregledajte [Kada se primjenjuju vizualne oznake](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Ako imate problema s automatskim označavanjem, pregledajte [Kako konfigurirati uvjete za automatsku i preporučenu klasifikaciju za Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) i Što traže vrste [osjetljivih informacija](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
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
- [Korištenje oznaka osjetljivosti u aplikacijama microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

