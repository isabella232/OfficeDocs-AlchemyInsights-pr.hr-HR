---
title: 1554 Winsock pogreška 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698854"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="c57a7-102">Poruka o pogrešci za Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="c57a7-102">Winsock error 10061</span></span>

<span data-ttu-id="c57a7-103">Ovaj kod pogreške znači da Microsoft ne može uspostaviti TCP utičnicu (veza) s odredišnim domaćinom.</span><span class="sxs-lookup"><span data-stu-id="c57a7-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="c57a7-104">Najvjerojatnije je uzrok te pogreške problem s konfiguracijom vatrozida.</span><span class="sxs-lookup"><span data-stu-id="c57a7-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="c57a7-105">Da biste riješili problem, provjerite sljedeće postavke:</span><span class="sxs-lookup"><span data-stu-id="c57a7-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="c57a7-106">Provjera konfiguracije vatrozida pomoću podataka u [URL-ovima programa Microsoft 365 i RASPONIMA IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="c57a7-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="c57a7-107">Ako je pogreška specifična za Exchange Online Protection (AOP), trebali ste prethodno biti obaviješteni o promjeni [IP adresa zaštite sustava Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="c57a7-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="c57a7-108">Provjerite nije li davatelj internetskih usluga (ISP) blokirao priključak.</span><span class="sxs-lookup"><span data-stu-id="c57a7-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="c57a7-109">Provjerite postavke pametnog glavnog računala i odredišnog poslužitelja u poveznicima.</span><span class="sxs-lookup"><span data-stu-id="c57a7-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="c57a7-110">Imajte na čemu da Microsoft 365 ne blokira *dolazne* veze na taj način.</span><span class="sxs-lookup"><span data-stu-id="c57a7-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
