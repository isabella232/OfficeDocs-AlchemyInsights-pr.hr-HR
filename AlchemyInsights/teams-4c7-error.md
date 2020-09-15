---
title: Pogreška timova 4c7
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700195"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="3c63e-102">4c7 pogreška u Microsoftovim timovima</span><span class="sxs-lookup"><span data-stu-id="3c63e-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="3c63e-103">Ta se pogreška pojavljuje jer Microsoftovi timovi zahtijevaju provjeru autentičnosti obrazaca.</span><span class="sxs-lookup"><span data-stu-id="3c63e-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="3c63e-104">Kada implementirate Active Directory Federation Services (AD FS), provjera autentičnosti obrazaca nije omogućena za intranet prema zadanim postavkama.</span><span class="sxs-lookup"><span data-stu-id="3c63e-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="3c63e-105">Ako Integrirana provjera autentičnosti sustava Windows ne uspije, od vas će se zatražiti da se prijavite pomoću provjere autentičnosti obrazaca.</span><span class="sxs-lookup"><span data-stu-id="3c63e-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="3c63e-106">Da biste riješili taj problem, omogućite provjeru autentičnosti obrazaca pomoću dodatka AD FS Microsoftova konzola za upravljanje (MMC-a) na računalu koje sadrži lokalnu kopiju servisa Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3c63e-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="3c63e-107">Da biste to učinili, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="3c63e-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="3c63e-108">U navigacijskom oknu pronađite **pravila provjere autentičnosti**.</span><span class="sxs-lookup"><span data-stu-id="3c63e-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="3c63e-109">U odjeljku **Akcije** u oknu s detaljima odaberite **Uređivanje globalne primarne provjere autentičnosti**.</span><span class="sxs-lookup"><span data-stu-id="3c63e-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="3c63e-110">Na kartici **intranetu** odaberite **Provjera autentičnosti obrazaca**.</span><span class="sxs-lookup"><span data-stu-id="3c63e-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="3c63e-111">Odaberite **u redu** (ili **Primijeni**).</span><span class="sxs-lookup"><span data-stu-id="3c63e-111">Select **OK** (or **Apply**).</span></span>