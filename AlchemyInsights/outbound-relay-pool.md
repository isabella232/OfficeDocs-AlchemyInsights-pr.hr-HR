---
title: Odlazni relej
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: 7e5bb1fda1dec0c0f72d1944d54b6f2747a6e909
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326069"
---
# <a name="outbound-relay-pool"></a>Odlazni relej

Microsoft mijenja konfiguraciju za prijenos ili prosljeđivanje e-pošte putem Microsoft 365. Poruke u određenim scenarijima prosljeđuju se ili prenose putem Microsoft 365 pomoću posebnog releja. Poruke poslane pomoću releja mogu završiti u mapi bezvrijedne pošte primatelja. Dodatne informacije potražite u članku Grupe [izlazne isporuke](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Da biste izbjegli scenarij pomoću releja, provjerite zadovoljavaju li proslijeđene/proslijeđene poruke jedan od sljedećih kriterija:

- Odlazni pošiljatelj prihvaćena je domena klijenta.
- SPF (Sender Policy Framework) prosljeđuje se kada se poruka Microsoft 365.
- DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.
 
Poruke koje zadovoljavaju gore navedene kriterije ne prenose se putem releja.

Ako se MX zapis za vašu domenu usmjeri na poslužitelj drugih proizvođača ili lokalnog poslužitelja, pomoću poboljšanog filtriranja provjerite je li SPF provjera valjanosti točna za ulaznu e-poštu i da biste izbjegli slanje e-pošte putem releja.

**Kako možemo znati utječe li na nas relej?**

Ako proslijeđene ili proslijeđene poruke e-pošte koriste jedan od gore navedenih kriterija, poruke se neće prenijeti putem releja. No ako se poruka pošalje putem releja, IP odlaznog poslužitelja nalazi se u rasponu 40.95.0.0/16, a naziv izlaznog poslužitelja sadrži **rly** u naziv.

