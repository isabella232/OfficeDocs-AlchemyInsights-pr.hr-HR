---
title: Rješavanje problema s pravilnikom klijenta (nadjačavanje akcije)
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
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326789"
---
# <a name="fix-tenant-policy-action-override"></a>Rješavanje problema s pravilnikom klijenta (nadjačavanje akcije)

Jedna od vaših pravilnika o neželjenoj pošti utjecala je na ovu poruku. Da biste pregledali pravilnike, učinite sljedeće:

1. Na portalu Microsoft 365 Defender e-pošte idite <https://security.microsoft.com/> **na e-pošta &** pravila suradnje & pravila Prijetnje pravilima protiv neželjene pošte u \>  \>  \>  **odjeljku Pravila.**

   Da biste se izravno idite na stranicu Pravilnika o **neželjenoj pošti,** koristite <https://security.microsoft.com/antispam> .

2. Na **stranici Pravilnika** o neželjenoj pošti odaberite pravilnik klikom na naziv pravilnika (**Vrsta** je Pravilnik o prilagođenoj neželjenoj pošti **ili** **Naziv** je pravilnik o ulasu neželjene **pošte (zadano).**
3. U brošuri s detaljima koja će se prikazati **odaberite Uređivanje akcija** u **odjeljku Akcije.**
4. U **odjeljku Akcije poruke** pregledajte presudu za neželjenu  **poštu,** neželjenu poštu visoke pouzdanosti,  **krađu** identiteta i krađu identiteta visoke pouzdanosti da biste vidjeli jesu li odabrane neke od sljedećih vrijednosti:
   - **Dodavanje X-zaglavlja**
   - **Predostrožan redak predmeta s tekstom**
   - **Preusmjeravanje poruke na adresu e-pošte**
   - **Brisanje poruke**
   - **Nema akcije**

   Moguće je da su standardne postavke **primijenjene na** sve korisnike Exchange Online Protection na poruku.

Dodatne informacije potražite u članku Konfiguriranje [pravilnika o neželjenoj pošti u programu EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies).
