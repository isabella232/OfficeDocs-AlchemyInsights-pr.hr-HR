---
title: Preusmjeravanja servisa OneDrive za tvrtke web OneDrive u delve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 74151ed149c57ceebc841902796189f6638795a9
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571192"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="a166f-102">Preusmjereno na delve nakon klika na OneDrive</span><span class="sxs-lookup"><span data-stu-id="a166f-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="a166f-103">Pogledajte naš detaljni [Vodič za otklanjanje poteškoća](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="a166f-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="a166f-104">Da biste riješili taj problem, administrator sustava Office 365 mora dodijeliti korisnicima pravo stvaranja svojih web-mjesta moje web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="a166f-104">To resolve this problem, the Office 365 administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="a166f-105">To je zato što je stranica OneDrive za tvrtke stvorena na mojim web-lokacijama.</span><span class="sxs-lookup"><span data-stu-id="a166f-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="a166f-106">Da biste to ispravno odobrili, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="a166f-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="a166f-107">U centru za administraciju sustava SharePoint kliknite **korisnički profili**.</span><span class="sxs-lookup"><span data-stu-id="a166f-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="a166f-108">U odjeljku **osobe** kliknite **Upravljanje dozvolama korisnika**.</span><span class="sxs-lookup"><span data-stu-id="a166f-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="a166f-109">Dodajte korisnike kojima su potrebne dozvole za stvaranje web-mjesta moje web-lokacije.</span><span class="sxs-lookup"><span data-stu-id="a166f-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="a166f-110">Prema zadanim postavkama, ova postavka postavljena je na **sve osim za vanjske korisnike**.</span><span class="sxs-lookup"><span data-stu-id="a166f-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="a166f-111">Nakon što dodate korisnika, korisnike ili grupu, provjerite je li odabran dodani korisnik, korisnici ili grupa, pomaknite se do odjeljka **dozvole** , a zatim potvrdite okvir pored **Stvaranje osobnog web-mjesta (potrebno za osobnu pohranu, feed vijesti i praćeni sadržaj)**.</span><span class="sxs-lookup"><span data-stu-id="a166f-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="a166f-112">Kliknite **u redu**, a zatim neka korisnik Pretraži stranicu sa servisom OneDrive da bi stvorio web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="a166f-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
