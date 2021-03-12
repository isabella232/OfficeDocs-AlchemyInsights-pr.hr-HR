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
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="ec2c8-102">Nemogućnost slanja/primanja e-pošte u/iz sustava Office 365 zbog TLS 1,0 i TLS 1,1 onemogućivanje</span><span class="sxs-lookup"><span data-stu-id="ec2c8-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="ec2c8-103">Kao što je potvrdio pošta centar za poruke MC229914, TLS 1,0 i TLS 1,1 ukidanja započinjete provedbu za krajnje točke protoka pošte u sustavu Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="ec2c8-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="ec2c8-104">Uskoro Office 365 više neće prihvaćati TLS 1,0 i TLS 1,1 veze e-pošte iz vanjskih izvora.</span><span class="sxs-lookup"><span data-stu-id="ec2c8-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="ec2c8-105">Exchange Online nikada neće koristiti TLS 1,0 ni 1,1 za slanje odlaznih poruka e-pošte.</span><span class="sxs-lookup"><span data-stu-id="ec2c8-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="ec2c8-106">Ako se suočavate s pitanjima zbog TLS 1,0 ili 1,1 onemogućivanje, možda ćete doživjeti neku od sljedećih pogrešaka –</span><span class="sxs-lookup"><span data-stu-id="ec2c8-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="ec2c8-107">Pošiljatelj dobiva NDR odskočiti back-' 421, a veza je odbačena zbog SocketError '</span><span class="sxs-lookup"><span data-stu-id="ec2c8-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="ec2c8-108">Pogreška u pregledniku čekanja lokalnog poslužitelja koji šalje e-poštu službeniku 365-' 421, veza je odbačena zbog SocketError '</span><span class="sxs-lookup"><span data-stu-id="ec2c8-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="ec2c8-109">Pogreška prilikom [prijave protokola](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) Pošalji konektor na poslužitelju koji šalje e-poštu u Office 365 – TLS pregovori nisu uspjeli s pogreškom SocketError</span><span class="sxs-lookup"><span data-stu-id="ec2c8-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="ec2c8-110">Pogreška u log-u protokola za povezivanje s povezanjem ili primanje-' 451 5.7.3 mora najprije izdati naredbu STARTTLS '</span><span class="sxs-lookup"><span data-stu-id="ec2c8-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="ec2c8-111">Ako osjetite neku od gore navedenih pogrešaka, provjerite je li poslužitelj koji šalje ili primi e-poštu za TLS 1,2 omogućen tako da provjeri sljedeće ključeve registra-</span><span class="sxs-lookup"><span data-stu-id="ec2c8-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="ec2c8-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2 \ Client] **"Disabledebydefault" = d: 00000000 "enabled" = deword: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2 \ Server] **"Disabledebydefault" = daword: 00000000 "enabled" = deword: 00000001**</span><span class="sxs-lookup"><span data-stu-id="ec2c8-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="ec2c8-113">Ako napravite neku promjenu u gore navedenim ključevima registra da biste omogućili TLS 1,2, ponovno pokrenite poslužitelj da bi promjene stupile na kraj.</span><span class="sxs-lookup"><span data-stu-id="ec2c8-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="ec2c8-114">Provjerite i jesu li instalirana najnovija ažuriranja sustava Windows i Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec2c8-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="ec2c8-115">Dodatne informacije potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="ec2c8-115">For more information, see:</span></span>

- [<span data-ttu-id="ec2c8-116">Upute za Exchange Server TLS, Part 1: priprema za TLS 1,2 – Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="ec2c8-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="ec2c8-117">Exchange Server TLS smjernice 2. dio: Omogućivanje TLS 1,2 i identificiranje klijenata koji ga ne koriste – Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="ec2c8-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="ec2c8-118">Objašnjenje scenarija e-pošte ako se TLS-ove verzije ne mogu dogovoriti sa sustavom Exchange Online – Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="ec2c8-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
