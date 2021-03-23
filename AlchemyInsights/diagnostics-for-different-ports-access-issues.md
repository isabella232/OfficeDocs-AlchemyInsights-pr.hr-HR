---
title: Dijagnostika za druge probleme s pristupom lukama
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035004"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Dijagnostika za druge probleme s pristupom lukama

Da biste riješili razne probleme s pristupom priključkom, slijedite sljedeće korake:

1. Stop/dealpronađite virtualni stroj (VM) s portala, ponovno pokrenite VM, a zatim ponovno testirajte. 
2. Provjerite imate li mrežne postavke za VM da biste utvrdili imate li mrežne sigurnosne grupe (NSGs) koji blokiraju promet. Možete koristiti i [alat za provjeru IP toka programa Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) da biste provjerili je li nsgs blokirao promet, User-Defined rute (UDRs) preusmjeravaju promet natrag na lokalno ("zadana ruta",, a) ili na mrežni uređaj.
Ako i dalje naiđete na probleme nakon pokušaja navedenih koraka, navedite VM naziv i TCP priključak na kojem pokušavate slati poštu radi daljnje dijagnoze.

**Preporučeni dokumenti**

[Ograničenja i preporuke za slanje odlaznih poruka e-pošte putem priključka 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)