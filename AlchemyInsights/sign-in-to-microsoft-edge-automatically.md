---
title: Automatska prijava u Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398721"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="977a4-102">Automatska prijava u Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="977a4-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="977a4-103">Microsoft Edge koristi zadani račun operacijskog sustava za automatsku prijavu korisnika u skladu s konfiguracijom korisnikova uređaja.</span><span class="sxs-lookup"><span data-stu-id="977a4-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="977a4-104">Scenariji svake vrste konfiguracije uređaja i postupka prijave zavisnog korisnika opisani su u nastavku:</span><span class="sxs-lookup"><span data-stu-id="977a4-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="977a4-105">**Uređaj je hibridni/AAD-J:** ta je mogućnost dostupna u sustavima Windows 10, sustavu Windows i odgovarajućim verzijama poslužitelja.</span><span class="sxs-lookup"><span data-stu-id="977a4-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="977a4-106">Korisnici se automatski prijave pomoću računa servisa Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="977a4-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="977a4-107">**Uređaj je pridružen domeni: ta** je mogućnost dostupna u sustavima Windows 10, sustavu Windows nižu razinu i odgovarajućim verzijama poslužitelja.</span><span class="sxs-lookup"><span data-stu-id="977a4-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="977a4-108">Korisnici s računima domene po zadanom se ne prijave automatski; da biste omogućili automatsku prijavu za njih, koristite **pravilnik ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="977a4-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="977a4-109">Da biste korisnicima omogućili automatsku prijavu s računima za Azure AD, razmislite o hibridnom pridruživanju svojim uređajima.</span><span class="sxs-lookup"><span data-stu-id="977a4-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="977a4-110">**Zadani je račun** operacijskog sustava Microsoftov račun: ta je mogućnost dostupna u sustavu Windows 10 RS3 (verzija 1709, međuverzija 10.0.16299) i novijim verzijama.</span><span class="sxs-lookup"><span data-stu-id="977a4-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="977a4-111">Scenarij nije vjerojatno da će se pojaviti na poslovnim uređajima.</span><span class="sxs-lookup"><span data-stu-id="977a4-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="977a4-112">No ako je zadani račun za OS Microsoftov račun, Microsoft Edge će se automatski prijaviti korisniku pomoću Microsoftova računa.</span><span class="sxs-lookup"><span data-stu-id="977a4-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
