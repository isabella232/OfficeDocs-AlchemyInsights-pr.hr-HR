---
title: Rad s iOS VPP aplikacije pravilo Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917488"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="cacfe-102">Rad s iOS VPP aplikacija</span><span class="sxs-lookup"><span data-stu-id="cacfe-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="cacfe-103">Čitanje [kako upravljati apps iOS kupili putem glasnoće nabave program s Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) da biste saznali više o značajki, ograničenja i korake da bi koristiti Apple glasnoće nabave Program i podrška za njega u Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="cacfe-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="cacfe-104">**Uobičajene probleme:** "Dodijeljeni app VPP je iOS Moje korisnici, ali instalacija nije uspjela."</span><span class="sxs-lookup"><span data-stu-id="cacfe-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="cacfe-p101">To se može dogoditi ako se koristi jedan token VPP preko višestruke davatelje usluga upravljanja mobilnog uređaja. VPP tokeni iz Apple se može koristiti samo s jednog davatelja. Koristi VPP token s višestruke davatelje usluga, morate ponovo prenesite token Intune.</span><span class="sxs-lookup"><span data-stu-id="cacfe-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="cacfe-p102">Instalacija također neće uspeti ako ukupan broj instalacijama prijeći broj licenci. Prikaz izvješća o korištenju licence, idite na **apps Intune Mobile** \> stranici **App licence** . Da biste saznali kako oslobodio licenci koristi pogledajte [Ovaj članak.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="cacfe-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

