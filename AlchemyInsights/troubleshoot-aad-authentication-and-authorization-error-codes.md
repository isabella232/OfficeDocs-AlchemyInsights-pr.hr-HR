---
title: Otklanjanje poteškoća s kodom pogreške Azure AD i autorizacija (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035197"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>Otklanjanje poteškoća s kodom pogreške Azure AD i autorizacija (AADSTS)

Da biste riješili provjeru autentičnosti AAD i šifre pogrešaka autorizacije (AADSTS), izvedite sljedeće preporučene korake:

1. **Rješavanje kodova pogrešaka u aplikaciji**

- **Spec. OAuth 2.0**, https://tools.ietf.org/html/rfc6749#section-5.2 nudi smjernice o tome kako obraditi pogreške tijekom provjere autentičnosti pomoću dijela pogreške u odgovoru na pogrešku.

    - **pogreška**: niz kod pogreške koji se može koristiti za klasificiranje vrsta pogrešaka koje se javljaju i moraju se koristiti za reakcije na pogreške.
    - Polje **pogreške** sadrži nekoliko mogućih vrijednosti – pregledajte veze s dokumentacijom protokola i specifikacije OAuth 2,0 da biste saznali više o određenim pogreškama i kako reagirati na njih.

- Ovdje je ogledni odgovor o pogrešci:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **Podaci o postojećem kodu pogreške**

- Kodovi pogrešaka i poruke podložni su promjeni. Najnovije informacije potražite u članku https://login.microsoftonline.com/error Pronalaženje AADSTS opisa pogrešaka, popravaka i nekih predloženih zaobilaznih rješenja.
- Možete potražiti i otkloniti [šifre pogrešaka Aadsts](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) navedenih u odjeljku članak [Provjera autentičnosti oglasa i pogreške autorizacije](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).

3. **Pomoć**

- [Mogućnosti podrške i pomoći za razvojne inženjere](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) – ako vam je potreban odgovor na pitanje ili pomoć u rješavanju problema koji nije pokriven našom dokumentacijom, možda je vrijeme da se obratite stručnjacima za pomoć. U ovom se članku nudi nekoliko prijedloga za dobivanje odgovora na pitanja prilikom razvoja aplikacija koje se integriraju u Microsoftovu platformu identiteta.








