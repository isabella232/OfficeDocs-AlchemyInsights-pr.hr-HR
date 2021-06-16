---
title: Active Directory se ne sinkronizira
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930967"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="e4dfd-102">Active Directory se ne sinkronizira</span><span class="sxs-lookup"><span data-stu-id="e4dfd-102">Active Directory not syncing</span></span>

<span data-ttu-id="e4dfd-103">Ako primate pogreške sinkronizacije, kao što je "bez nedavne sinkronizacije" ili primijetite status sinkronizacije direktorija na portalu za administratore sustava Office kaže: "Last synced more than 3 days ago" (Zadnje sinkronizirano prije više od 3 dana) možda AADConnect ima netočne postavke ili nedovoljne dozvole za izvođenje sinkronizacije.</span><span class="sxs-lookup"><span data-stu-id="e4dfd-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="e4dfd-104">Ponovna instalacija AADConnect pomoću ekspresnih postavki može brzo riješiti problem:</span><span class="sxs-lookup"><span data-stu-id="e4dfd-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="e4dfd-105">[Preuzmite najnoviju verziju servisa AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="e4dfd-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="e4dfd-106">[Slijedite upute za ekspresne instalacije](/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="e4dfd-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="e4dfd-107">Servis Azure AD Connect mora biti instaliran na poslužitelju Windows Server 2012 ili novijoj verziji.</span><span class="sxs-lookup"><span data-stu-id="e4dfd-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="e4dfd-108">Ovaj poslužitelj mora biti spojen na domenu i može biti kontroler domene ili poslužitelj člana.</span><span class="sxs-lookup"><span data-stu-id="e4dfd-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="e4dfd-109">Potpuni popis preduvjeta za Azure AD Povezivanje preduvjeta i preduvjeta pregledajte [Preduvjeti](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)za Azure AD Povezivanje .</span><span class="sxs-lookup"><span data-stu-id="e4dfd-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="e4dfd-110">Dodatne informacije o računima servisa AADConnect potražite u članku [Azure AD Povezivanje: Računi i dozvole](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="e4dfd-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
