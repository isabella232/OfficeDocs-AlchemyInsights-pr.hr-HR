---
title: Umirovljenje naslijeđenih alata za predočavanje elektroničkih dokumenata
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157532"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Umirovljenje naslijeđenih alata za predočavanje elektroničkih dokumenata

Kao rezultat nove i poboljšane funkcionalnosti predočavanja elektroničkih dokumenata u centru za usklađenost sustava Microsoft 365, sljedeći naslijeđeni alati i naredbe za predočavanje elektroničkih dokumenata bit će umirovljeni u narednim mjesecima:

- [Lokalno predočavanje elektroničkih dokumenata](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) i Lokalno držanje u centru za [administratore](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) sustava Exchange.

- Cmdleti komponente Exchange Online PowerShell koji podržavaju lokalno predočavanje elektroničkih dokumenata i držanja na mjestu. (Ovi cmdleti su kolektivno identificirani kao *-MailboxSearch cmdlets.) To uključuje sljedeće cmdlete:

    - [Novi poštanski sandučić](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Pretraživanje početnog poštanskog sandučića](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Pretraživanje poštanskog sandučića](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Postavljanje pretraživanja poštanskog sandučića](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) u komponenti Exchange Online PowerShell.
- Sljedeće operacije u API-ju za Exchange Web Services:
    - [GetSearchablePoštanski sandučići](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnPoštanski sandučići](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnPoštanski sandučići](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Napredno predočavanje elektroničkog dokumenata za Office 365 v1.0](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

**Vremenski slijed za umirovljenje:**
- 1. travanj 2020.: nećete moći stvoriti nova pretraživanja i čekanja, ali i dalje možete pokrenuti, uređivati i brisati postojeća pretraživanja na vlastitu odgovornost. Microsoftova podrška više neće podržavati lokalno predočavanje & drži u EAC-u.

- Srpanj 1, 2020: In-Place eDiscovery & Drži funkcionalnost u EAC će biti smještenu u načinu rada samo za čitanje. To znači da ćete moći ukloniti samo postojeća pretraživanja i držanja.

**Dodatne informacije potražite u odjeljku**:

 - [Migracija naslijeđenih pretraživanja predočavanje elektroničkih dokumenata](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Umirovljenje naslijeđenih alata za predočavanje elektroničkih dokumenata](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Najčešća pitanja o unaprijed i na mjestu čekanja](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



