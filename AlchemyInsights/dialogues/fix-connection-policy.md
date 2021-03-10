---
title: Rješavanje pravilnika o povezivanju
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50692828"
---
# <a name="fix-connection-policy"></a>Rješavanje pravilnika o povezivanju

Poruka e-pošte označena je sigurnim i isporučena u korisničku ulaznu poštu jer je IP adresa slanja označena kao sigurna u pravilima filtra veze. Da biste pregledali pravilnik, učinite sljedeće:

1. Idite na [centar za sigurnost & sustava Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143), a zatim otvorite pravilo za **Upravljanje prijetnjama** za  >    >  [zaštitu od neželjene pošte](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Na kartici **Prilagođena** odaberite **pravilnik o filtriranju veze**, a zatim odaberite **Uređivanje pravilnika**.
3. Pregledajte popis **dozvola za IP** . Pogledajte je li omogućen **popis sigurnih popisa** .

    > [!NOTE]
    > Microsoftovi pretplatnici na izvore drugih davatelja pouzdanih pošiljatelja. Ako je omogućen **popis sigurnog popisa** , ti pouzdani pošiljatelji nisu pogrešno označeni kao neželjena pošta. Preporučujem vam da odaberete tu mogućnost, jer će to smanjiti broj FALSE pozitivnih (dobra pošta koja je klasificirana kao spam) koju primate.
