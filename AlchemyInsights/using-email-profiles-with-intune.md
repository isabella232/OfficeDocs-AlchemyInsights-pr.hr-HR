---
title: Korištenje profila e-pošte s intuneom
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554775"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="a27ee-102">Korištenje profila e-pošte s intuneom</span><span class="sxs-lookup"><span data-stu-id="a27ee-102">Using email profiles with Intune</span></span>

<span data-ttu-id="a27ee-103">Intune se može koristiti za stvaranje i implementaciju profila e-pošte za izvorni (ugrađeni) klijent e-pošte na više platformi uređaja.</span><span class="sxs-lookup"><span data-stu-id="a27ee-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="a27ee-104">Informacije o nekim ograničenjima povezanima s profilima e-pošte, uključujući način rukovanja prisutnošću postojećih profila i uklanjanje profila [e-pošte, potražite u članku Dodavanje postavki e-pošte uređajima koji koriste Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="a27ee-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="a27ee-105">Dodatne informacije o stvaranju profila e-pošte za svaku platformu uređaja potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="a27ee-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="a27ee-106">Postavke Android uređaja za konfiguriranje e-pošte, provjere autentičnosti i sinkronizacije u aplikaciji Intune</span><span class="sxs-lookup"><span data-stu-id="a27ee-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="a27ee-107">Dodavanje postavki e-pošte za iOS i iPadOS uređaje u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a27ee-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="a27ee-108">Postavke profila e-pošte u programu Microsoft Intune za uređaje sa sustavom Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="a27ee-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="a27ee-109">Postavke profila e-pošte za uređaje sa sustavom Windows 10 u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a27ee-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="a27ee-110">**Uobičajeni problem sa sinkronizacijom**</span><span class="sxs-lookup"><span data-stu-id="a27ee-110">**Common syncing issue**</span></span>

<span data-ttu-id="a27ee-111">**Knox na Profilu e-pošte androida sprječava sinkronizaciju korisničkih kontakata, kalendara i zadataka s korisničkim uređajima.**</span><span class="sxs-lookup"><span data-stu-id="a27ee-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="a27ee-112">Knox na Android KNOX profilu e-pošte nudi administratoru mogućnost da odluči koje se vrste sadržaja sinkroniziraju s uređajem postavljanjem svakog na omogućeno.</span><span class="sxs-lookup"><span data-stu-id="a27ee-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="a27ee-113">Ako je postavka za bilo koju vrstu sadržaja postavljena na **Nije konfigurirano (zadano),** ta se vrsta sadržaja ne sinkronizira automatski.</span><span class="sxs-lookup"><span data-stu-id="a27ee-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="a27ee-114">Korisnik može omogućiti vrstu sadržaja koju žele izravno na uređaju ručno, ali tu konfiguraciju prebriše postavka pravila Intune, a sinkronizacija prestaje s tom vrstom sadržaja.</span><span class="sxs-lookup"><span data-stu-id="a27ee-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

