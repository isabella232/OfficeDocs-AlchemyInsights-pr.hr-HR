---
title: Slanje prilagođenih obavijesti pomoću Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886849"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="9071e-102">Kako slati prilagođene obavijesti korisnicima upravljanih iOS i Android uređaja</span><span class="sxs-lookup"><span data-stu-id="9071e-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="9071e-103">Prilagođene obavijesti za Intune obrađuju aplikacija Portal tvrtke na korisnikovom uređaju.</span><span class="sxs-lookup"><span data-stu-id="9071e-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="9071e-104">Aplikacija zatim stvara push obavijest na tom uređaju.</span><span class="sxs-lookup"><span data-stu-id="9071e-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="9071e-105">Sljedeći su preduvjeti za uređaj za podršku primitka prilagođenih obavijesti, a za aplikaciju zatim stvoriti push obavijest:</span><span class="sxs-lookup"><span data-stu-id="9071e-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="9071e-106">Uređaj mora imati instaliran aplikaciju Portal tvrtke.</span><span class="sxs-lookup"><span data-stu-id="9071e-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="9071e-107">Uređaj mora dopustiti aplikaciji Portal tvrtke za slanje push obavijesti.</span><span class="sxs-lookup"><span data-stu-id="9071e-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="9071e-108">Kada je aplikacija instalirana ili ažurirana, ona će zatražiti od korisnika da dopusti obavijesti.</span><span class="sxs-lookup"><span data-stu-id="9071e-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="9071e-109">Android uređaji moraju imati instalirane usluge Google Play.</span><span class="sxs-lookup"><span data-stu-id="9071e-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="9071e-110">Uređaj mora biti upisan s Intune.</span><span class="sxs-lookup"><span data-stu-id="9071e-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="9071e-111">Dodatne informacije, uključujući kako poslati poruku, potražite u [dokumentaciji značajke](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="9071e-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
