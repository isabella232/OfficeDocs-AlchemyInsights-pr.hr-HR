---
title: Rad s ID-om pravila za aplikacije za iOS VPP 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719949"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="c2fbf-102">Rad s vpp aplikacijama za iOS</span><span class="sxs-lookup"><span data-stu-id="c2fbf-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="c2fbf-103">Pročitajte [kako upravljati aplikacijama sustava iOS kupljenima putem programa za kupnju jedinice pomoću](https://docs.microsoft.com/intune/vpp-apps-ios) servisa Microsoft Intune da biste saznali više o značajkama, ograničenjima i koracima za korištenje Appleovog programa za kupnju glasnoće i podrške za njega u programu Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="c2fbf-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="c2fbf-104">**Uobičajeni problemi:** "Korisnicima sam dodijelio iOS VPP aplikaciju, ali instalacija nije uspjela."</span><span class="sxs-lookup"><span data-stu-id="c2fbf-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="c2fbf-105">To se može dogoditi ako se jedan VPP token koristi u više davatelja usluga upravljanja mobilnim uređajima.</span><span class="sxs-lookup"><span data-stu-id="c2fbf-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="c2fbf-106">VPP tokeni tvrtke Apple smiju se koristiti samo s jednim davateljem usluga.</span><span class="sxs-lookup"><span data-stu-id="c2fbf-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="c2fbf-107">Ako ste koristili VPP token s više davatelja usluga, morate ga ponovno prenijeti na Intune.</span><span class="sxs-lookup"><span data-stu-id="c2fbf-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="c2fbf-108">Instalacija također može uspjeti ako ukupan broj instalacija premašuje broj licenci.</span><span class="sxs-lookup"><span data-stu-id="c2fbf-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="c2fbf-109">Da biste pregledali izvješće o korištenju za licence, idite na stranicu Licence **aplikacije Intune za mobilne** \> **aplikacije.**</span><span class="sxs-lookup"><span data-stu-id="c2fbf-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="c2fbf-110">Da biste saznali kako povratiti licence koje se koriste, pogledajte [ovaj članak.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="c2fbf-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
