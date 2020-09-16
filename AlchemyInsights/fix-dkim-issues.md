---
title: Rješavanje problema s postavljanjem programa DEKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744942"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="58b70-102">Rješavanje problema s postavljanjem programa DEKIM</span><span class="sxs-lookup"><span data-stu-id="58b70-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="58b70-103">Ako naiđete na probleme s omogućivanjem servisa DEKIM za prilagođenu domenu, slijedite sljedeće korake:</span><span class="sxs-lookup"><span data-stu-id="58b70-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="58b70-104">Većina problema s postavljanjem programa di odnosi se na pogrešne DNS zapise.</span><span class="sxs-lookup"><span data-stu-id="58b70-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="58b70-105">Provjerite je li deformator CNAME zapisa (**ne** TXT zapis) pravilno oblikovan.</span><span class="sxs-lookup"><span data-stu-id="58b70-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="58b70-106">Dodatne informacije potražite u ovoj [temi](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="58b70-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="58b70-107">Kada stvorite ili ažurirate svoj DNS zapise u servisu DNS za hostiranje domene (tipično, registrar domene), pričekajte da se DNS zapisi propagiraju.</span><span class="sxs-lookup"><span data-stu-id="58b70-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="58b70-108">Ako ne možete stvoriti DKIM DNS zapise u centru za administratore, možete zamijeniti \<CustomDomain\> prilagođenu domenu (na primjer, contoso.com) i pokrenuti ovu naredbu u komponenti [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="58b70-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
