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
ms.openlocfilehash: 262cca0feee17d1f929a5a94a4dd6c1ec317f6ec
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/21/2020
ms.locfileid: "43650560"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Umirovljenje naslijeđenih alata za predočavanje elektroničkih dokumenata

Kao rezultat nove i poboljšane funkcije predočavanja elektroničkih dokumenata u centru za usklađenost sustava Microsoft 365, sljedeći naslijeđeni alati i naredbe za predočavanje elektroničkih dokumenata bit će umirovljeni u narednim mjesecima:

- [Lokalno predočavanje elektroničkih dokumenata](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) i lokalno čekanje u centru za [administratore](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) sustava Exchange.

- Cmdleti komponente Exchange Online PowerShell koji podržavaju lokalno predočavanje elektroničkih dokumenata i lokalno čekanje. (Ti su cmdleti zajednički identificirani kao cmdleti *-MailboxSearch.) To uključuje sljedeće cmdlete:

    - [Novo pretraživanje poštanskih sandučića](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Početno pretraživanje poštanskog sandučića](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Postavljanje pretraživanja poštanskog sandučića](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) u komponenti Exchange Online PowerShell.
- Sljedeće operacije u API-ju exchange web-usluga:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Napredno predočavanje elektroničkih dokumenata v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Rokovi za umirovljenje:**
- 1. travanj 2020: nećete moći stvoriti nova pretraživanja i drži, ali još uvijek možete pokrenuti, urediti i izbrisati postojeća pretraživanja na vlastitu odgovornost. Microsoftova podrška više neće podržavati lokalno predočavanje elektroničkih dokumenata & u EAC-u.

- 1. srpanj 2020.: Funkcija otkrivanja elektroničkih dokumenata na mjestu & u EAC-u bit će smještena u načinu rada samo za čitanje. To znači da ćete moći ukloniti samo postojeća pretraživanja i čekanja.

**Dodatne informacije potražite u odjeljku**:

 - [Migriranje naslijeđenih pretraživanja i čekanja na microsoft 365 centar za usklađenost](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Umirovljenje naslijeđenih alata za predočavanje elektroničkih dokumenata](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Najčešća pitanja o otkrivanju elektroničkih dokumenata na mjestu i zasima zamjenom](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



