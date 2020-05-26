---
title: 618 Pravila zajedničkog korištenja kalendara
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/26/2020
ms.locfileid: "44372991"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Pogreška pravila prilikom zajedničkog korištenja kalendara

1. Učinite nešto od sljedećeg, ovisno o situaciji:
    - Povežite se sa sustavom Exchange Online pomoću udaljene ljuske PowerShell. Dodatne informacije [potražite u odjeljku Povezivanje sa sustavom Exchange Online pomoću udaljene ljuske PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Na lokalnom poslužitelju otvorite ljusku za upravljanje sustavom Exchange.
2. Odredite pravila zajedničkog korištenja koja su dodijeljena korisniku. Da biste to učinili, pokrenite sljedeću naredbu i zabilježite vraćeno pravilo:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Ažurirajte pravila zajedničkog korištenja za korisnika. Da biste to učinili, slijedite ove korake:
    - Otvorite centar za administratore sustava Exchange.
    - Kliknite **Organizacija**, a zatim dvokliknite pravilo koje je dodijeljeno korisniku u odjeljku **Pojedinačno zajedničko korištenje**. Ovo je pravilo koje je vraćeno u koraku 2.
    - Na stranici Pravilo zajedničkog korištenja odaberite razinu zajedničkog korištenja kalendara koju želite dopustiti u **odjeljku Navedite koje informacije želite zajednički koristiti**; kliknite **Spremi**.

Dodatne informacije potražite [u odjeljku "Pravila ne dopuštaju dodjeljivanje dozvola na ovoj razini jednom ili više primatelja" kada korisnik pokuša zajednički koristiti kalendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
