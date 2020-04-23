---
title: Rješavanje problema s DKIM postavljanjem
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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717554"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="e257d-102">Rješavanje problema s DKIM postavljanjem</span><span class="sxs-lookup"><span data-stu-id="e257d-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="e257d-103">Ako naiđete na probleme s omogućivanjem DKIM-a za prilagođenu domenu, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="e257d-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="e257d-104">Većina DKIM problema s postavljanjem povezana je s netočnim DNS zapisima.</span><span class="sxs-lookup"><span data-stu-id="e257d-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="e257d-105">Provjerite je li DKIM CNAME zapis **(ne** TXT zapis) ispravno oblikovan.</span><span class="sxs-lookup"><span data-stu-id="e257d-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="e257d-106">Dodatne informacije potražite u ovoj [temi](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="e257d-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="e257d-107">Nakon stvaranja ili ažuriranja DKIM DNS zapisa na servisu za hostiranje DNS-a za svoju domenu (obično registraru domene), pričekajte da se DNS zapisi propagire.</span><span class="sxs-lookup"><span data-stu-id="e257d-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="e257d-108">Ako ne možete stvoriti DKIM DNS zapise u centru \<za\> administratore, CustomDomain možete zamijeniti prilagođenom domenom (na `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`primjer, contoso.com) i pokrenuti ovu naredbu u programu Exchange Online [PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): .</span><span class="sxs-lookup"><span data-stu-id="e257d-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
