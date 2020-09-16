---
title: Korištenje profila e-pošte s dodatkom Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653280"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="eae22-102">Korištenje profila e-pošte s dodatkom Intune</span><span class="sxs-lookup"><span data-stu-id="eae22-102">Using email profiles with Intune</span></span>

<span data-ttu-id="eae22-103">Intune se može koristiti za stvaranje i implementaciju profila e-pošte za urođenik (ugrađeno) klijenta e-pošte na više platformi uređaja.</span><span class="sxs-lookup"><span data-stu-id="eae22-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="eae22-104">Informacije o nekim od ograničenja povezanih s profilima e-pošte, uključujući način na koji se obrađuju prisutnost postojećih profila i kako ukloniti profile e-pošte potražite [u članku Dodavanje postavki e-pošte na uređaje pomoću aplikacije Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="eae22-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="eae22-105">Dodatne informacije o stvaranju profila e-pošte za svaku platformu uređaja potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="eae22-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="eae22-106">Postavke uređaja sa sustavom Android za konfiguriranje e-pošte, provjere autentičnosti i sinkronizacije u programu Intune</span><span class="sxs-lookup"><span data-stu-id="eae22-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="eae22-107">Dodavanje postavki e-pošte za iOS i iPadOS uređaje u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="eae22-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="eae22-108">Postavke profila e-pošte u aplikaciji Microsoft Intune za uređaje sa sustavom Windows Phone 8,1</span><span class="sxs-lookup"><span data-stu-id="eae22-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="eae22-109">Postavke profila za e-poštu za uređaje sa sustavom Windows 10 u programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="eae22-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="eae22-110">**Zajednički problem s sinkronizacijom**</span><span class="sxs-lookup"><span data-stu-id="eae22-110">**Common syncing issue**</span></span>

<span data-ttu-id="eae22-111">**KNOX na servisu Android profile za e-poštu onemogućuje sinkronizaciju korisnika, kalendara i zadataka s korisničkim uređajima.**</span><span class="sxs-lookup"><span data-stu-id="eae22-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="eae22-112">KNOX na Android KNOX profilu e-pošte nudi administratore mogućnost odluke o tome koje se vrste sadržaja sinkroniziraju s uređajem tako da se svaki od njih omogući.</span><span class="sxs-lookup"><span data-stu-id="eae22-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="eae22-113">Ako je postavka za neku vrstu sadržaja postavljena na **nekonfiguriranu** (zadano), ta se vrsta sadržaja ne sinkronizira automatski.</span><span class="sxs-lookup"><span data-stu-id="eae22-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="eae22-114">Korisnik može omogućiti ručno umetanje vrste sadržaja na uređaj, ali ta je konfiguracija prebrijela postavku pravilnika Intune, a sinkronizacija prestaje za tu vrstu sadržaja.</span><span class="sxs-lookup"><span data-stu-id="eae22-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

