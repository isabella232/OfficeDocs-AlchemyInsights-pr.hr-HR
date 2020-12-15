---
title: Automatsko prijavljivanje u Microsoft Edge
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676965"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="71d2e-102">Automatsko prijavljivanje u Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="71d2e-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="71d2e-103">Microsoft Edge koristi zadani račun OS-a da bi se automatski prijavljujem u korisnika prema načinu na koji je korisnički uređaj konfiguriran.</span><span class="sxs-lookup"><span data-stu-id="71d2e-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="71d2e-104">Scenariji svake vrste konfiguracije uređaja i njenog ovisnog korisničkog postupka prijave opisani su u nastavku:</span><span class="sxs-lookup"><span data-stu-id="71d2e-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="71d2e-105">**Uređaj je Hybrid/AAD-J**: ta je mogućnost dostupna u sustavu Windows 10, sustavu Windows i pripadajućim poslužiteljskim verzijama.</span><span class="sxs-lookup"><span data-stu-id="71d2e-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="71d2e-106">Korisnici se automatski prijave pomoću računa za Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="71d2e-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="71d2e-107">**Uređaj je spojen na domenu**: ta je mogućnost dostupna u sustavu Windows 10, Windows i pripadajućim poslužiteljskim verzijama.</span><span class="sxs-lookup"><span data-stu-id="71d2e-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="71d2e-108">Korisnici s računima domena po zadanom nisu prijavljeni automatski; Da biste omogućili automatsko prijavljivanje za njih, koristite pravilnik **Configureonpremisasaccountautosignin** .</span><span class="sxs-lookup"><span data-stu-id="71d2e-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="71d2e-109">Da biste omogućili automatsko prijavljivanje za korisnike s računima za Azure AD, razmotrite hibridno spajanje na njihove uređaje.</span><span class="sxs-lookup"><span data-stu-id="71d2e-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="71d2e-110">**Zadani račun OS-a jest Microsoftov račun**: ta je mogućnost dostupna u sustavu Windows 10 RS3 (verzija 1709, izgradnja 10.0.16299) i novije verzije.</span><span class="sxs-lookup"><span data-stu-id="71d2e-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="71d2e-111">Scenarij se vjerojatno neće pojaviti na poslovnim uređajima.</span><span class="sxs-lookup"><span data-stu-id="71d2e-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="71d2e-112">No ako je zadani račun OS-a Microsoftov račun, Microsoft Edge automatski će se prijaviti korisniku pomoću Microsoftova računa.</span><span class="sxs-lookup"><span data-stu-id="71d2e-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
