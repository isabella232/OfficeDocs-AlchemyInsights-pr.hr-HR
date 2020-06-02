---
title: Rješavanje problema s dkim postavljanjem
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506766"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="15456-102">Rješavanje problema s dkim postavljanjem</span><span class="sxs-lookup"><span data-stu-id="15456-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="15456-103">Ako imate problema s omogućivanjem DKIM-a za prilagođenu domenu, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="15456-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="15456-104">Većina DKIM problema s postavljanjem povezana je s netočnim DNS zapisima.</span><span class="sxs-lookup"><span data-stu-id="15456-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="15456-105">Provjerite je li DKIM CNAME zapis **(ne** TXT zapis) ispravno oblikovan.</span><span class="sxs-lookup"><span data-stu-id="15456-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="15456-106">Dodatne informacije potražite u ovoj [temi](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="15456-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="15456-107">Nakon što stvorite ili ažurirate DKIM DNS zapise na servisu hostiranja DNS-a za svoju domenu (obično registrar domene), pričekajte da se DNS zapisi šire.</span><span class="sxs-lookup"><span data-stu-id="15456-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="15456-108">Ako ne možete stvoriti DKIM DNS zapise u centru za administratore, možete zamijeniti \<CustomDomain\> prilagođenom domenom (na primjer, contoso.com) i pokrenuti ovu naredbu u [powershellu sustava Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="15456-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
