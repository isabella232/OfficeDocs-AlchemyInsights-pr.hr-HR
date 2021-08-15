---
title: Dijagnostika za različite probleme s pristupom priključcima
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
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030894"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Dijagnostika za različite probleme s pristupom priključcima

Da biste riješili različite probleme s pristupom priključku, poduzmite sljedeće korake:

1. Zaustavljanje/deallocate virtualni stroj (VM) s portala, ponovno pokrenite VIRTUALNO računalo i ponovno testirajte. 
2. Provjerite mrežne postavke virtualnog računala da biste utvrdili imate li mrežne sigurnosne grupe (NSG-ovi) koje blokiraju promet. Možete koristiti i alat za provjeru [IP](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) toka mreže da biste provjerili blokiraju li NSG-ovi promet, User-Defined Rute (UDR-ovi) koji preusmjeravanje prometa natrag na lokalne ('Default Route' 0.0.0.0/0) ili na mrežni uređaj.
Ako se problemi i dalje pojave nakon što pokušate s gore navedenim koracima, navedite naziv virtualnog računala i TCP priključak na koji pokušavate poslati poštu radi daljnje dijagnostike.

**Preporučeni dokumenti**

[Ograničenja i preporuke za slanje odlazne e-pošte putem priključka 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)