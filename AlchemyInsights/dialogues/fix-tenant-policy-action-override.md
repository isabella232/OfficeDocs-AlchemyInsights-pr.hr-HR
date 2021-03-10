---
title: Rješavanje pravilnika o klijentu (prijelaz na akciju)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692799"
---
# <a name="fix-tenant-policy-action-override"></a>Rješavanje pravilnika o klijentu (prijelaz na akciju)

Pravilnik o suzbijanju neželjene pošte u vašem zakupcu utjecao je na ovu poruku. Da biste pregledali pravilnik, učinite sljedeće:

1. Idite na [centar za sigurnost & sustava Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143), a zatim otvorite pravilo za **Upravljanje prijetnjama** za  >    >  [zaštitu od neželjene pošte](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Provjerite prikazuje li **izvor pravilnika** sljedeće:  **Dodavanje-XHeader/Modifysubject/preusmjeravanje/Izbriši/bez akcije/Skrivena kopija poruka**

    Ako je tako, na kartici **Prilagođeno** provjerite postavke Pravilnika koja je utjecala na poruku. Moguće je da su **standardne postavke** primijenjene na sve klijente zaštite servisa Exchange Online utjecali na poruku.

Dodatne informacije o konfiguriranju pravilnika filtra za neželjenu poštu potražite u članku [Konfiguriranje pravilnika filtra za neželjenu poštu](https://go.microsoft.com/fwlink/?linkid=2101431).
