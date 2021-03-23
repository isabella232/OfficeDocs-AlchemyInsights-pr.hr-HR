---
title: Oslobađanje prostora na disku u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035217"
---
# <a name="free-up-drive-space-in-windows-10"></a>Oslobađanje prostora na disku u sustavu Windows 10

Postoje dvije mogućnosti za oslobađanje prostora na disku u sustavu Windows:

- Oslobodite prostora na disku u sustavu Windows 10.
- Oslobodite prostor za ažuriranja sustava Windows 10 s vanjskim uređajem za pohranu.

Ako i dalje imate nisko diskovni razmak nakon korištenja značajke čišćenja diska, moguće je da se mapa TEMP brzo ispunjava pomoću datoteka aplikacije (. Appx) koju koristi Microsoft Store. Da biste riješili taj problem, ponovno postavite trgovinu, poništite predmemoriranje pohrane, a zatim pokrenite alat za otklanjanje poteškoća sa servisom Windows Update. Provjerite je li Microsoft Store zatvoren prije nastavka ovih koraka.

**Prvi korak: ponovno postavljanje Microsoftove trgovine**

**Notes** Time se trajno brišu podaci o aplikaciji na uređaju, uključujući vaše preference i pojedinosti o prijavi.

1. Odaberite **Započni**  >  **Postavke**  >  **aplikacija za aplikacije**  >  **& značajki**.

1. Na popisu aplikacija pronađite i odaberite Microsoft Store.

1. Odaberite **Dodatne mogućnosti**.

1. Pomaknite se prema dolje pa odaberite **ponovno postavi**, a zatim **potvrdite ponovno postavi**.

**Drugi korak: poništite predmemoriranje Microsoftove trgovine**

1. Pritisnite tipku s logotipom sustava Windows + R da biste otvorili dijaloški okvir Pokreni.

1. Upišite wsreset.exe i odaberite **u redu**.

1. Otvorit će se prazan prozor naredbenog upita. Nakon približno 10 sekundi prozor će se zatvoriti, a trgovina će se automatski otvoriti.

**Treći korak: ponovno postavljanje servisa Windows Update**

1. Odaberite **Započni**  >    >  **Ažuriranje postavki & sigurnosnim**  >  **otklanjanjem poteškoća**.

1. Pomaknite se prema dolje pa na popisu odaberite **Windows Update** , a zatim **Pokrenite alat za otklanjanje poteškoća**.

1. Ponovno pokrenite računalo i provjerite jeste li još uvijek doživjeli problem.

