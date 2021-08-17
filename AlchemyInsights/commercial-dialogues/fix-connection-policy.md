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
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888398"
---
# <a name="fix-connection-policy"></a>Rješavanje problema s pravilnikom veze

Poruka e-pošte označena je sigurnom i isporučena u korisnikov ulaznu poštu jer je izvorna IP adresa označena kao sigurna u zadanom pravilniku filtra veze. Da biste pregledali pravilnik, učinite sljedeće:

1. Na portalu Microsoft 365 Defender u odjeljku E-pošta & pravila suradnje & Pravila Prijetnje pravilnika o zaštiti od neželjene pošte <https://security.microsoft.com/>  \>  \>  \>  **u odjeljku Pravila.**

   Da biste se izravno idite na stranicu Pravilnika o **neželjenoj pošti,** koristite <https://security.microsoft.com/antispam> .

2. Na **stranici Pravilnika o neželjenoj** pošti odaberite pravilnik pod nazivom Pravilnik filtra veze **(Zadano)** klikom na naziv pravilnika.

3. U brošuri s pojedinostima koja će se prikazati kliknite **Uređivanje pravilnika** filtra veze u **odjeljku Filtriranje** veze.

4. Pregledajte unose u **odjeljku Uvijek dopusti poruke sa** sljedećih IP adresa ili raspona adresa i pogledajte je li odabran **popis** Uključi sigurno.

   > [!NOTE]
   > Microsoft se pretplati na izvore pouzdanih pošiljatelja drugih proizvođača. Ako je siguran popis omogućen, ti pouzdani pošiljatelji nisu zabunom označeni kao neželjena pošta. Preporučujemo da odaberete tu mogućnost jer će se time smanjiti broj neistinitih pozitivnih poruka (dobra pošta koja se klasificira kao neželjena pošta) koje primate.

Dodatne informacije potražite u članku [Konfiguriranje filtriranja veze](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy).
