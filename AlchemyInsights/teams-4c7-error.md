---
title: Ekipa 4c7 pogreška
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796008"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="998c0-102">4c7 pogreška u Microsoftovim timovima</span><span class="sxs-lookup"><span data-stu-id="998c0-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="998c0-103">Ta se pogreška pojavljuje jer Microsoft Teams zahtijeva provjeru autentičnosti obrazaca.</span><span class="sxs-lookup"><span data-stu-id="998c0-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="998c0-104">Kada implementirati Active Directory Federation Services (AD FS), provjera autentičnosti obrazaca nije omogućena za intranet prema zadanim postavkama.</span><span class="sxs-lookup"><span data-stu-id="998c0-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="998c0-105">Ako Integrirana provjera autentičnosti sustava Windows ne uspije, zatražit će se da se prijavite pomoću provjere autentičnosti obrazaca.</span><span class="sxs-lookup"><span data-stu-id="998c0-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="998c0-106">Da biste riješili taj problem, omogućite provjeru autentičnosti obrazaca pomoću dodatka AD FS Microsoftova konzola za upravljanje (MMC) na računalu s lokalnom kopijom servisa Active Directory.</span><span class="sxs-lookup"><span data-stu-id="998c0-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="998c0-107">Da biste to učinili, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="998c0-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="998c0-108">U navigacijskom oknu pregledajte **pravila provjere autentičnosti**.</span><span class="sxs-lookup"><span data-stu-id="998c0-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="998c0-109">U odjeljku **Akcije** u oknu s detaljima odaberite **Uređivanje globalne primarne provjere autentičnosti**.</span><span class="sxs-lookup"><span data-stu-id="998c0-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="998c0-110">Na kartici **intraneta** odaberite **provjeru autentičnosti obrazaca**.</span><span class="sxs-lookup"><span data-stu-id="998c0-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="998c0-111">Odaberite **u redu** (ili **Primijeni**).</span><span class="sxs-lookup"><span data-stu-id="998c0-111">Select **OK** (or **Apply**).</span></span>