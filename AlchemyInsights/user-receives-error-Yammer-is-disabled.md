---
title: Korisnik prima pogrešku AADSTS7000112 Yammer je onemogućen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197794"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="4a5c0-102">Korisnik prima pogrešku AADSTS7000112 Yammer je onemogućen</span><span class="sxs-lookup"><span data-stu-id="4a5c0-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="4a5c0-103">Ako primite poruku o pogrešci "AADSTS7000112: aplikacija '00000005-0000-0ff1-ce00-00000000000000000000000000000000000000000000000000000"(Yammer) je onemogućena", postoji problem s glavnim servisom unutar Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4a5c0-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="4a5c0-104">Administrator je možda onemogućio glavnu servisnu karticu da bi blokirao pristup servisu Yammer.</span><span class="sxs-lookup"><span data-stu-id="4a5c0-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="4a5c0-105">Onemogućivanje principala servisa se ne preporučuje i može uzrokovati dodatne probleme.</span><span class="sxs-lookup"><span data-stu-id="4a5c0-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="4a5c0-106">Dodatne informacije o podržanom pristupu za blokiranje korisničkog pristupa servisu Yammer potražite u odjeljku [Isključivanje pristupa servisu Yammer za korisnike sustava Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="4a5c0-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="4a5c0-107">Da biste ispravili taj problem na portalu Azure i vratili korisnički pristup servisu Yammer:</span><span class="sxs-lookup"><span data-stu-id="4a5c0-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="4a5c0-108">Otvorite stranicu Azure Active Directory i odaberite **Enterprise aplikacije** u odjeljku **Upravljanje** u lijevom navigacijskom oknu.</span><span class="sxs-lookup"><span data-stu-id="4a5c0-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="4a5c0-109">U okvir za pretraživanje upišite **Office 365 Yammer** i odaberite naziv aplikacije da biste otvorili postavke.</span><span class="sxs-lookup"><span data-stu-id="4a5c0-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="4a5c0-110">U lijevom navigacijskom oknu odaberite **Svojstva** u odjeljku **Upravljanje.**</span><span class="sxs-lookup"><span data-stu-id="4a5c0-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="4a5c0-111">Postavite vrijednost **omogućeno za korisnike za prijavu ?** **Yes** **Save**</span><span class="sxs-lookup"><span data-stu-id="4a5c0-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="4a5c0-112">Ponovno se prijavite na Yammer.</span><span class="sxs-lookup"><span data-stu-id="4a5c0-112">Sign in to Yammer again.</span></span> <span data-ttu-id="4a5c0-113">Možda ćete morati očistiti kolačiće.</span><span class="sxs-lookup"><span data-stu-id="4a5c0-113">You might need to clear cookies.</span></span>

<span data-ttu-id="4a5c0-114">Umjesto toga pokrenite PowerShell naredbe da biste postavili vrijednost.</span><span class="sxs-lookup"><span data-stu-id="4a5c0-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="4a5c0-115">Dodatne informacije potražite [u odjeljku Pogreška "Nažalost, ali imamo poteškoća s prijavom" kada kliknete pločicu Yammer u sustavu Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="4a5c0-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 