---
title: Ispravite probleme DKIM Postava
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764911"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="528b0-102">Ispravite probleme DKIM Postava</span><span class="sxs-lookup"><span data-stu-id="528b0-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="528b0-103">Ako se pojave problemi omogućavanja DKIM za prilagođene domene, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="528b0-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="528b0-104">Većinu problema Postava DKIM su povezani neispravna DNS zapisa.</span><span class="sxs-lookup"><span data-stu-id="528b0-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="528b0-105">Provjerite je li ispravno oblikovani zapisom DKIM CNAME (**ne** TXT zapisu).</span><span class="sxs-lookup"><span data-stu-id="528b0-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="528b0-106">Dodatne informacije potražite u ovoj [temi](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="528b0-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="528b0-107">Nakon što stvorite ili ažuriranje zapisa DKIM DNS na DNS domaćin usluge za domenu (obično vaše domene Registrator), pričekajte zapise DNS proširiti.</span><span class="sxs-lookup"><span data-stu-id="528b0-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="528b0-108">Ako ne možete stvoriti zapise DKIM DNS u centru za administraciju, možete zamijeniti \<CustomDomain\> s prilagođene domene (na primjer, contoso.com) i pokrenuti ovu naredbu [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="528b0-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
