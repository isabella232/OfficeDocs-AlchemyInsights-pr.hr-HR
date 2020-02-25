---
title: Active Directory ne sinkronizira
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265153"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="51a52-102">Active Directory ne sinkronizira</span><span class="sxs-lookup"><span data-stu-id="51a52-102">Active Directory not syncing</span></span>

<span data-ttu-id="51a52-103">Ako primate pogreške pri sinkronizaciji, kao što je "bez nedavne sinkronizacije" ili primijetite status sinkronizacije direktorija na portalu za administratore sustava Office, kaže: "Zadnji put sinkroniziranprije više od 3 dana", možda AADConnect ima netočne postavke ili nedovoljne dozvole za izvođenje sinkronizacije.</span><span class="sxs-lookup"><span data-stu-id="51a52-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="51a52-104">Ponovna instalacija aadconnecta pomoću ekspresnih postavki može brzo riješiti problem:</span><span class="sxs-lookup"><span data-stu-id="51a52-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="51a52-105">[Preuzmite najnoviju verziju AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="51a52-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="51a52-106">[Slijedite upute za brzu instalaciju](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="51a52-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="51a52-107">Dodatne informacije o računima servisa AADConnect potražite u [odjeljku Povezivanje sa servisom Azure: Računi i dozvole](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="51a52-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
