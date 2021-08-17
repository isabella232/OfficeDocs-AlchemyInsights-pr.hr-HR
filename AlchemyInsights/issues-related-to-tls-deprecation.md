---
title: Nemogućnost slanja/primanja e-pošte u/iz Office 365 zbog onemogućivanja TLS 1.0 i TLS 1.1
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
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054898"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Nemogućnost slanja/primanja e-pošte u/iz Office 365 zbog onemogućivanja TLS 1.0 i TLS 1.1

Kao što je potvrđeno u centru za poruke, mc229914, TLS 1.0 i TLS 1.1 deprecation započeli su s Exchange Online krajnjim točkama tijeka pošte. Uskoro Office 365 više neće prihvatiti veze e-pošte TLS 1.0 i TLS 1.1 iz vanjskih izvora. Osim toga, Exchange Online koristiti TLS 1.0 ili 1.1 za slanje izlazne e-pošte. Ako imate problema zbog onemogućivanja TLS 1.0 ili 1.1, možda ćete naići na jednu od sljedećih pogrešaka:

- Pošiljatelj dobiva NDR odskočiti natrag - '421 4.4.2 Veza je ispuštena zbog SocketError'
- Pogreška u pregledniku reda čekanja lokalnog poslužitelja koji šalje poruku e-pošte službeniku 365- '421 4.4.2 Veza je ispuštena zbog SocketError'
- Pogreška u zapisniku protokola za [slanje poveznika](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) na poslužitelju koji šalje poruku e-pošte Office 365- TLS nije uspjelo s pogreškom SocketError
- Pogreška u zapisniku protokola za slanje ili primanje poveznika – '451 5.7.3 Najprije morate izdati naredbu STARTTLS'

Ako se pojavi neka od gore navedenih pogrešaka, provjerite je li poslužitelj koji šalje ili prima e-poštu omogućio TLS 1.2 tako da provjeri sljedeće ključeve registra–

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**

Ako promijenite gore navedene ključeve registra da biste omogućili TLS 1.2, ponovno pokrenite poslužitelj da bi promjene stupjele na snagu. Provjerite jesu li instalirana najnovija Windows i Exchange ažuriranja.

Dodatne informacije potražite u sljedećim člancima:

- [Exchange Server Smjernice za TLS, prvi dio: Priprema za TLS 1.2 – Microsoftova tehnička zajednica](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Objašnjenje scenarija e-pošte ako se verzije TLS-a ne mogu dogovoriti s Exchange Online – Microsoftova tehnička zajednica](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
