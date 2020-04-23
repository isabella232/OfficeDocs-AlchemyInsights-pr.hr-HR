---
title: 1554 Winsock pogreška 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766161"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="cd28c-102">Winsock pogreška 10061</span><span class="sxs-lookup"><span data-stu-id="cd28c-102">Winsock error 10061</span></span>

<span data-ttu-id="cd28c-103">Ovaj kôd pogreške znači da Microsoft nije mogao uspostaviti TCP utičnicu (vezu) s ciljnim glavnim računalom.</span><span class="sxs-lookup"><span data-stu-id="cd28c-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="cd28c-104">Najvjerojatniji uzrok ove pogreške je problem s konfiguracijom vatrozida.</span><span class="sxs-lookup"><span data-stu-id="cd28c-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="cd28c-105">Da biste riješili problem, provjerite sljedeće postavke:</span><span class="sxs-lookup"><span data-stu-id="cd28c-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="cd28c-106">Provjera konfiguracije vatrozida pomoću podataka u [URL-ovima i rasponima IP adresa sustava Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="cd28c-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="cd28c-107">Ako je pogreška specifična za Exchange Online Protection (EOP), trebali ste prethodno biti obaviješteni o promjeni [IP adresa exchange online protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="cd28c-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="cd28c-108">Provjerite blokira li davatelj internetskih usluga (ISP) priključak.</span><span class="sxs-lookup"><span data-stu-id="cd28c-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="cd28c-109">Provjerite postavke pametnog glavnog računala i ciljnog poslužitelja u konektorima.</span><span class="sxs-lookup"><span data-stu-id="cd28c-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="cd28c-110">Imajte na umu da Microsoft 365 na taj način ne blokira *dolazne* veze.</span><span class="sxs-lookup"><span data-stu-id="cd28c-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
