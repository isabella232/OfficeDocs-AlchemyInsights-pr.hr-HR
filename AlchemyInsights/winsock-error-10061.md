---
title: Pogreška Winsocka 1554 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e82e90b670235848105636fb2039ed60d3b93c67
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364905"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="9bbc2-102">Winsock pogreške 10061</span><span class="sxs-lookup"><span data-stu-id="9bbc2-102">Winsock error 10061</span></span>

<span data-ttu-id="9bbc2-103">Ta šifra pogreške znači da Office 365 nije mogao uspostaviti TCP utičnice (veza) s glavnog računala za cilj.</span><span class="sxs-lookup"><span data-stu-id="9bbc2-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="9bbc2-104">Najvjerojatniji uzrok te pogreške je problem s konfiguracijom vatrozid.</span><span class="sxs-lookup"><span data-stu-id="9bbc2-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="9bbc2-105">Da biste riješili problem, provjerite ove postavke:</span><span class="sxs-lookup"><span data-stu-id="9bbc2-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="9bbc2-106">Provjerite konfiguraciju vatrozida s informacijama u [Office 365 URL i raspone IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="9bbc2-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="9bbc2-107">Ako pogreška je specifičan za Exchange Online Protection (EOP), trebali ste primili prethodno obavijest promjenu [Exchange Online Protection IP adrese](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="9bbc2-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="9bbc2-108">Provjerite je li vaš davatelj internetskih usluga (ISP) blokira priključak.</span><span class="sxs-lookup"><span data-stu-id="9bbc2-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="9bbc2-109">Provjerite pametne glavnog i ciljnog postavke poslužitelja u vaše poveznike.</span><span class="sxs-lookup"><span data-stu-id="9bbc2-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="9bbc2-110">Imajte na umu Office 365 ne blokiraj *dolazne* veze na ovaj način.</span><span class="sxs-lookup"><span data-stu-id="9bbc2-110">Note that Office 365 doesn't block *incoming* connections in this manner.</span></span>
