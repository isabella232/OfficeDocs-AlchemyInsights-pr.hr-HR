---
title: Postavljanje automatskih odgovora za poštanski sandučić
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820926"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="2ae51-102">Postavljanje automatskih odgovora za poštanski sandučić korisnika</span><span class="sxs-lookup"><span data-stu-id="2ae51-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="2ae51-103">**Metoda 1**</span><span class="sxs-lookup"><span data-stu-id="2ae51-103">**Method 1**</span></span>

1. <span data-ttu-id="2ae51-104">Prijavite se na portal sustava Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2ae51-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="2ae51-105">Idite na **Korisnici > Aktivni korisnici** (ili **Grupe > Zajednički poštanski sandučići** ako ga postavite na zajednički poštanski sandučić).</span><span class="sxs-lookup"><span data-stu-id="2ae51-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="2ae51-106">Odaberite korisnika s poštanskim sandučićem sustava Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ae51-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="2ae51-107">Na izborniku s potpaletom na desnoj strani idite na **Postavke pošte > Automatski odgovori** (ako se radi o zajedničkom poštanskom sandučiću, samo kliknite **Automatski odgovori** na potpaleti).</span><span class="sxs-lookup"><span data-stu-id="2ae51-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="2ae51-108">**Metoda 2**</span><span class="sxs-lookup"><span data-stu-id="2ae51-108">**Method 2**</span></span>

1. <span data-ttu-id="2ae51-109">Prijavite se na portal za administratore sustava Microsoft 365 pomoću administratorskih vjerodajnica.</span><span class="sxs-lookup"><span data-stu-id="2ae51-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="2ae51-110">Proširite mogućnost **Administratorski centri**, pa kliknite **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="2ae51-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="2ae51-111">Kliknite sliku u gornjem desnom kutu, kliknite **Drugi korisnik**, pa odaberite poštanski sandučić korisnika koji želite promijeniti.</span><span class="sxs-lookup"><span data-stu-id="2ae51-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="2ae51-112">Na lijevoj strani odaberite **Mogućnosti**, kliknite **Organiziranje e-pošte**, pa kliknite **Automatski odgovori.**</span><span class="sxs-lookup"><span data-stu-id="2ae51-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="2ae51-113">**Metoda 3**</span><span class="sxs-lookup"><span data-stu-id="2ae51-113">**Method 3**</span></span>

<span data-ttu-id="2ae51-114">Pokrenite sljedeći cmdlet u servisu PowerShell za Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="2ae51-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="2ae51-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="2ae51-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="2ae51-116">Dodatne informacije o tom cmdletu potražite u članku [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="2ae51-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
