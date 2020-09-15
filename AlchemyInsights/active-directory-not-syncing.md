---
title: Active Directory nije sinkroniziranje
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697621"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="c918e-102">Active Directory nije sinkroniziranje</span><span class="sxs-lookup"><span data-stu-id="c918e-102">Active Directory not syncing</span></span>

<span data-ttu-id="c918e-103">Ako primate pogreške pri sinkronizaciji, kao što je "Nema nedavne sinkronizacije" ili primijetite da status sinkronizacije direktorija na portalu za administratore sustava Office kaže: "zadnje sinkronizirano prije više od 3 dana", moguće je da AADConnect ima pogrešne postavke ili nedovoljne dozvole za izvođenje sinkronizacije.</span><span class="sxs-lookup"><span data-stu-id="c918e-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="c918e-104">Ponovnim instalacijom servisa AADConnect pomoću ekspresne postavke možete brzo razriješiti problem:</span><span class="sxs-lookup"><span data-stu-id="c918e-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="c918e-105">[Preuzmite najnoviju verziju servisa AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="c918e-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="c918e-106">[Slijedite upute za ekspresne instalacije](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="c918e-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="c918e-107">Dodatne informacije o računima servisa AADConnect potražite u članku [Azure ad Connect: računi i dozvole](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="c918e-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
