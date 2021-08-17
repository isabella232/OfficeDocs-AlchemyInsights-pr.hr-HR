---
title: Umirovljenje naslijeđenih alata za predočavanje elektroničkih elektroničkih podataka
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074641"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Umirovljenje naslijeđenih alata za predočavanje elektroničkih elektroničkih podataka

Zbog nove i poboljšane funkcije predočavanja elektroničkih elektroničkih obveza u centru za usklađenost sustava Microsoft 365 sljedeći naslijeđeni alati i naredbe za predočavanje elektroničkih obveza bit će povučeni u sljedećim mjesecima:

- [In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [and In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.

- Cmdleti Exchange Online komponente PowerShell koji podržavaju In-Place predočavanje elektroničkih In-Place čuvanja. (Ti se cmdleti zajednički identificiraju kao cmdleti za *-MailboxSearch.) To obuhvaća sljedeće cmdlete:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [Cmdlet Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) u Exchange Online PowerShell.
- Sljedeće operacije u API-ju Exchange web-servisa:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Vremenska crta za umirovljenje:**
- **1. srpnja 2020.** Više ne možete stvarati nova pretraživanja i zadržavanja, ali postojeće pretraživanja možete pokrenuti, uređivati i brisati na vlastitu odgovornost. Microsoftova podrška više ne podržava In-Place eDiscovery & čuvanja u EAC-u.
    
- **1. listopada 2020** In-Place eDiscovery & Holds funkcionalnost u EAC-u bit će smještena u načinu samo za čitanje, pa možete ukloniti samo postojeća pretraživanja i čuvanja.

**Dodatne informacije potražite u članku**:

 - [Migracija naslijeđenih pretraživanja elektroničkih predočavanja elektroničkih elektroničkih podataka i čuvanja na Centar za usklađenost okruženja Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Umirovljenje naslijeđenih alata za predočavanje elektroničkih elektroničkih podataka](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Najčešća pitanja o In-Place predočavanja elektroničkih In-Place čuvanja](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



