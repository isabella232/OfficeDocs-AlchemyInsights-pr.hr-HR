---
title: 618 pravilnik za zajedničko korištenje kalendara
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684222"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Pogreška pravilnika prilikom zajedničkog korištenja kalendara

1. Učinite nešto od sljedećeg, ovisno o vašoj situaciji:
    - Povežite se sa sustavom Exchange Online pomoću udaljene komponente PowerShell. Dodatne informacije potražite u članku [Povezivanje sa sustavom Exchange Online pomoću udaljene komponente PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Na lokalnom poslužitelju otvorite ljusku za upravljanje sustavom Exchange.
2. Odredite pravilnik o podjeli koji je dodijeljen korisniku. Da biste to učinili, pokrenite sljedeću naredbu i obratite pozornost na povratak pravilnika:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Ažuriranje pravilnika za zajedničko korištenje korisnika. Da biste to učinili, slijedite ove korake:
    - Otvorite centar za administratore sustava Exchange.
    - Kliknite **tvrtka ili ustanova**, a zatim dvokliknite pravilo dodijeljeno korisniku u odjeljku **individualno zajedničko korištenje**. Ovo je pravilo koje je vraćeno u drugom koraku.
    - Na stranici pravilo zajedničkog korištenja odaberite razinu zajedničkog korištenja kalendara koju želite dopustiti u odjeljku **Navedite informacije koje želite zajednički koristiti**; kliknite **Spremi**.

Dodatne informacije potražite u članku: ["pravilo ne dopušta dodjeljivanje dozvola na ovoj razini jednom ili više primatelja (s)" kada korisnik pokuša zajednički koristiti kalendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
