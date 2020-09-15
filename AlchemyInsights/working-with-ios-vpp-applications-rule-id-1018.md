---
title: Rad sa pravilom VPP aplikacija za iOS 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688938"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="563ad-102">Rad s aplikacijama sustava iOS VPP</span><span class="sxs-lookup"><span data-stu-id="563ad-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="563ad-103">Pročitajte [kako upravljati aplikacijama sustava iOS kupljene putem programa za nabavu u programu Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) da biste saznali više o značajkama, ograničenjima i koracima da biste koristili program Apple Volume Kupnja i podršku za nju u programu Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="563ad-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="563ad-104">**Česti problemi:** "Korisniku sam dodijelio aplikaciju iOS VPP, ali instalacija nije uspjela."</span><span class="sxs-lookup"><span data-stu-id="563ad-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="563ad-105">To se može dogoditi ako se na više davatelja mobilnih uređaja koristi jedan token VPP-a.</span><span class="sxs-lookup"><span data-stu-id="563ad-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="563ad-106">VPP tokeni iz Apple-a mogu se koristiti samo s jednim davatelja usluga.</span><span class="sxs-lookup"><span data-stu-id="563ad-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="563ad-107">Ako ste koristili VPP token s više davatelja usluga, morate ponovno prenijeti token na Intune.</span><span class="sxs-lookup"><span data-stu-id="563ad-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="563ad-108">Instalacija može uspjeti i ako ukupan broj instalacija premašuje broj licenci.</span><span class="sxs-lookup"><span data-stu-id="563ad-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="563ad-109">Da biste pregledali izvješće o korištenju licenci, otvorite stranicu licence za **aplikacije Intune za mobilne aplikacije** \> **App licenses** .</span><span class="sxs-lookup"><span data-stu-id="563ad-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="563ad-110">Da biste doznali kako povratiti licence koje se koriste, pročitajte [ovaj članak.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="563ad-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
