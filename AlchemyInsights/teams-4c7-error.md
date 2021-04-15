---
title: Pogreška u aplikaciji Teams 4c7
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
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786661"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="10b83-102">Pogreška 4c7 u aplikaciji Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="10b83-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="10b83-103">Ta se pogreška pojavljuje jer je za Microsoft Teams potrebna provjera autentičnosti obrazaca.</span><span class="sxs-lookup"><span data-stu-id="10b83-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="10b83-104">Prilikom implementacije servisa Active Directory Federation Services (AD FS), provjera autentičnosti obrazaca po zadanom nije omogućena za intranet.</span><span class="sxs-lookup"><span data-stu-id="10b83-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="10b83-105">Ako integrirana provjera autentičnosti u sustavu Windows ne uspije, od vas će se zatražiti da se prijavite pomoću provjere autentičnosti obrazaca.</span><span class="sxs-lookup"><span data-stu-id="10b83-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="10b83-106">Da biste riješili taj problem, omogućite provjeru autentičnosti obrazaca pomoću alata AD FS Microsoft Management Console (MMC) na računalu koje sadrži lokalnu kopiju servisa Active Directory.</span><span class="sxs-lookup"><span data-stu-id="10b83-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="10b83-107">Da biste to učiniti, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="10b83-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="10b83-108">U navigacijskom oknu idite na Pravila **provjere autentičnosti**.</span><span class="sxs-lookup"><span data-stu-id="10b83-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="10b83-109">U **odjeljku Akcije** u oknu s detaljima **odaberite Uređivanje globalne primarne provjere autentičnosti**.</span><span class="sxs-lookup"><span data-stu-id="10b83-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="10b83-110">Na kartici **Intranet odaberite** Provjera **autentičnosti obrazaca**.</span><span class="sxs-lookup"><span data-stu-id="10b83-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="10b83-111">Odaberite **U** redu (ili **Primijeni).**</span><span class="sxs-lookup"><span data-stu-id="10b83-111">Select **OK** (or **Apply**).</span></span>