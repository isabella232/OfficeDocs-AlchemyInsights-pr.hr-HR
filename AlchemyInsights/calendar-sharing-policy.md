---
title: Pravilnik o zajedničkom korištenju kalendara 618
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
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091588"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Pogreška pravilnika prilikom zajedničkog korištenja kalendara

1. Učinite nešto od sljedećeg, prema potrebi za svoju situaciju:
    - Povezivanje se Exchange Online pomoću komponente Remote PowerShell. Dodatne informacije potražite u [članku Povezivanje Exchange Online udaljene ljuske PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Na lokalnom poslužitelju otvorite ljusku Exchange Management Shell.
2. Odredite pravilnik za zajedničko korištenje koji je dodijeljen korisniku. Da biste to učiniti, pokrenite sljedeću naredbu i zabilježite vraćeni pravilnik:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Ažurirajte pravilnik o zajedničkom korištenju za korisnika. Da biste to učiniti, slijedite ove korake:
    - Otvorite centar Exchange administratora.
    - Kliknite **Tvrtka ili** ustanova , a zatim dvokliknite pravilnik dodijeljen korisniku u odjeljku Pojedinačno zajedničko **korištenje**. To je pravilnik koji je vraćen u 2. koraku.
    - Na stranici Pravilo zajedničkog korištenja odaberite razinu zajedničkog korištenja kalendara koju želite dopustiti u odjeljku **Navedite koje podatke želite zajednički koristiti;** kliknite **Spremi**.

Dodatne informacije potražite u članku: [pogreška "Pravilnik](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)ne dopušta dodjelu dozvola na ovoj razini jednom ili više primatelja" kada korisnik pokuša zajednički koristiti kalendar .
