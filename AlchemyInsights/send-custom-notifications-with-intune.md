---
title: Slanje prilagođenih obavijesti pomoću aplikacije Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720638"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="73f55-102">Upute za slanje prilagođenih obavijesti korisnicima upravljanih uređaja sa sustavom iOS i uređajima sa sustavom Android</span><span class="sxs-lookup"><span data-stu-id="73f55-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="73f55-103">Prilagođene obavijesti za Intune obrađuju aplikacija Portal tvrtke na korisnikovom uređaju.</span><span class="sxs-lookup"><span data-stu-id="73f55-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="73f55-104">Aplikacija zatim stvara obavijesti o pritiskom na tom uređaju.</span><span class="sxs-lookup"><span data-stu-id="73f55-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="73f55-105">Slijede preduvjeti za uređaj da biste podržali primitak prilagođenih obavijesti, a da bi aplikacija stvorila obavijest o pritisku:</span><span class="sxs-lookup"><span data-stu-id="73f55-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="73f55-106">Uređaj mora imati instaliranu aplikaciju Portal tvrtke.</span><span class="sxs-lookup"><span data-stu-id="73f55-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="73f55-107">Uređaj mora dopustiti aplikaciji Portal tvrtke da šalje obavijesti o pritiskom.</span><span class="sxs-lookup"><span data-stu-id="73f55-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="73f55-108">Kada je aplikacija instalirana ili ažurirana, ona će zatražiti od korisnika da dozvoli obavijesti.</span><span class="sxs-lookup"><span data-stu-id="73f55-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="73f55-109">Uređaji sa sustavom Android moraju imati instaliran Google Reproduciraj servise.</span><span class="sxs-lookup"><span data-stu-id="73f55-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="73f55-110">Uređaj mora biti upisan pomoću aplikacije Intune.</span><span class="sxs-lookup"><span data-stu-id="73f55-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="73f55-111">Dodatne informacije, uključujući način slanja poruke, potražite u [dokumentaciji značajki](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="73f55-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
