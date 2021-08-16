---
title: Rješavanje problema s pravilnikom veze
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988079"
---
# <a name="fix-connection-policy"></a>Rješavanje problema s pravilnikom veze

Poruka e-pošte označena je sigurnom i isporučena u korisnikov ulaznu poštu jer je IP adresa za slanje označena sigurnom u pravilniku Filtar veze. Da biste pregledali pravilnik, učinite sljedeće:

1. Idite na [centar Office 365 sigurnosti & usklađenosti](https://go.microsoft.com/fwlink/p/?linkid=2077143), a zatim idite na Zaštita od **neželjene**  >  **pošte pravilnika**  >  [za upravljanje prijetnjama](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Na kartici **Prilagođeno** odaberite pravilnik **filtara Veza**, a zatim Uređivanje **pravilnika**.
3. Pregledajte **popis dopuštenih IP** adresa. Pogledajte je **li Sef popis** omogućen.

    > [!NOTE]
    > Microsoft se pretplati na izvore pouzdanih pošiljatelja drugih proizvođača. Ako **Sef popis pouzdanih** pošiljatelja nije zabunom označen kao neželjena pošta. Preporučujem odabir te mogućnosti jer će se time smanjiti broj neistinitih pozitivnih poruka (dobra pošta koja se klasificira kao neželjena pošta) koje primate.
