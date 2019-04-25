---
title: Pogreška Winsocka 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7651effc43cb0c4bc2fbbe5349bb72303943f493
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419972"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="97de6-102">Winsock pogreške 10061</span><span class="sxs-lookup"><span data-stu-id="97de6-102">Winsock error 10061</span></span>

<span data-ttu-id="97de6-103">Ta šifra pogreške znači da Office 365 nije mogao uspostaviti TCP utičnice (veza) s glavnog računala za cilj.</span><span class="sxs-lookup"><span data-stu-id="97de6-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="97de6-104">Najvjerojatniji uzrok te pogreške je problem s konfiguracijom vatrozid.</span><span class="sxs-lookup"><span data-stu-id="97de6-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="97de6-105">Da biste riješili problem, provjerite ove postavke:</span><span class="sxs-lookup"><span data-stu-id="97de6-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="97de6-106">Provjerite konfiguraciju vatrozida s informacijama u [Office 365 URL i raspone IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="97de6-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="97de6-107">Ako pogreška je specifičan za Exchange Online Protection (EOP), trebali ste primili prethodno obavijest promjenu [Exchange Online Protection IP adrese](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="97de6-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="97de6-108">Provjerite je li vaš davatelj internetskih usluga (ISP) blokira priključak.</span><span class="sxs-lookup"><span data-stu-id="97de6-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="97de6-109">Provjerite pametne glavnog i ciljnog postavke poslužitelja u vaše poveznike.</span><span class="sxs-lookup"><span data-stu-id="97de6-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="97de6-110">Imajte na umu Office 365 ne blokiraj *dolazne* veze na ovaj način.</span><span class="sxs-lookup"><span data-stu-id="97de6-110">Note that Office 365 doesn't block *incoming* connections in this manner.</span></span>
