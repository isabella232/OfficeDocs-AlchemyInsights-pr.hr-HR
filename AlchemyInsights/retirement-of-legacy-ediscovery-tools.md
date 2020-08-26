---
title: Povlačenje naslijeđenih alata za otkriće
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
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902612"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Povlačenje naslijeđenih alata za otkriće

Kao rezultat nove i poboljšane funkcionalnosti otkrivanja sustava Microsoft 365, u sljedećim mjesecima bit će umirovljen sljedeći Alati za otkrivanje naslijeđenih i naredbina:

- U centru za administratore sustava Exchange [na mjestu e-otkrivanje](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) i [mjesto](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)

- Cmdleti za Exchange Online PowerShell koji podržavaju web-otkriće i web-mjesto koje sadrži. (Ovi su cmdleti kolektivno identificirani za cmdlete *-MailboxSearch.) To obuhvaća sljedeće cmdlete:

    - [Novo-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Početak – MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Zaustavljanje-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) u komponenti Exchange Online PowerShell.
- Sljedeće operacije u API-ju sustava Exchange Web Services:
    - [Getsearchablepoštanske sandučiće](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [Setholdonsandučići](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Getholdonsandučići](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Napredno Idiscovery v 1,0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Vremenska traka za mirovinu**:
- **Srpanj 1, 2020** Više ne možete stvarati nova pretraživanja i održavati, no možete pokrenuti, uređivati i brisati postojeća pretraživanja na vlastitu odgovornost. Microsoftova podrška više ne podržava e-otkrivanje na mjestu & drži u sustavu e-servisa.
    
- **1. listopada 2020** U načinu rada za idiscovery & sadrži funkcionalnost u programu IAC bit će postavljena samo za čitanje, pa možete ukloniti samo postojeća pretraživanja i sadrži.

Dodatne **informacije potražite u članku**:

 - [Migraciju naslijeđenih pretraživanja u programu Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Povlačenje naslijeđenih alata za otkriće](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Najčešća pitanja o Neotkrivanjem na servisu i servisu na mjestu](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



