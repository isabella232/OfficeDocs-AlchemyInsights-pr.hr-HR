---
title: Nemogućnost slanja/primanja e-pošte u/iz sustava Office 365 zbog TLS 1,0 i TLS 1,1 onemogućivanje
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743451"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Nemogućnost slanja/primanja e-pošte u/iz sustava Office 365 zbog TLS 1,0 i TLS 1,1 onemogućivanje

Kao što je potvrdio pošta centar za poruke MC229914, TLS 1,0 i TLS 1,1 ukidanja započinjete provedbu za krajnje točke protoka pošte u sustavu Exchange Online. Uskoro Office 365 više neće prihvaćati TLS 1,0 i TLS 1,1 veze e-pošte iz vanjskih izvora. Exchange Online nikada neće koristiti TLS 1,0 ni 1,1 za slanje odlaznih poruka e-pošte. Ako se suočavate s pitanjima zbog TLS 1,0 ili 1,1 onemogućivanje, možda ćete doživjeti neku od sljedećih pogrešaka –

- Pošiljatelj dobiva NDR odskočiti back-' 421, a veza je odbačena zbog SocketError '
- Pogreška u pregledniku čekanja lokalnog poslužitelja koji šalje e-poštu službeniku 365-' 421, veza je odbačena zbog SocketError '
- Pogreška prilikom [prijave protokola](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) Pošalji konektor na poslužitelju koji šalje e-poštu u Office 365 – TLS pregovori nisu uspjeli s pogreškom SocketError
- Pogreška u log-u protokola za povezivanje s povezanjem ili primanje-' 451 5.7.3 mora najprije izdati naredbu STARTTLS '

Ako osjetite neku od gore navedenih pogrešaka, provjerite je li poslužitelj koji šalje ili primi e-poštu za TLS 1,2 omogućen tako da provjeri sljedeće ključeve registra-

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2 \ Client] **"Disabledebydefault" = d: 00000000 "enabled" = deword: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2 \ Server] **"Disabledebydefault" = daword: 00000000 "enabled" = deword: 00000001**

Ako napravite neku promjenu u gore navedenim ključevima registra da biste omogućili TLS 1,2, ponovno pokrenite poslužitelj da bi promjene stupile na kraj. Provjerite i jesu li instalirana najnovija ažuriranja sustava Windows i Exchange.

Dodatne informacije potražite u članku:

- [Upute za Exchange Server TLS, Part 1: priprema za TLS 1,2 – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS smjernice 2. dio: Omogućivanje TLS 1,2 i identificiranje klijenata koji ga ne koriste – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Objašnjenje scenarija e-pošte ako se TLS-ove verzije ne mogu dogovoriti sa sustavom Exchange Online – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
