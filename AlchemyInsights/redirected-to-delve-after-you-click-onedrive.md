---
title: Preusmjeravanje servisa OneDrive za tvrtke web-OneDrive na delve
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
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776371"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="04a1f-102">Preusmjereno na delve nakon klika na OneDrive</span><span class="sxs-lookup"><span data-stu-id="04a1f-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="04a1f-103">Pogledajte detaljan [Vodič za otklanjanje poteškoća](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="04a1f-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="04a1f-104">Da biste riješili taj problem, administrator mora dodijeliti korisnicima pravo na stvaranje web-mjesta moje web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="04a1f-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="04a1f-105">To je zato što se na mojim web-mjestima stvara stranica servisa OneDrive za tvrtke.</span><span class="sxs-lookup"><span data-stu-id="04a1f-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="04a1f-106">Da biste to ispravno dodijelili, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="04a1f-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="04a1f-107">U centru za administratore sustava SharePoint kliknite **korisnički profili**.</span><span class="sxs-lookup"><span data-stu-id="04a1f-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="04a1f-108">U odjeljku **osobe** kliknite **Upravljanje korisničkim dozvolama**.</span><span class="sxs-lookup"><span data-stu-id="04a1f-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="04a1f-109">Dodajte korisnike kojima su potrebne dozvole za stvaranje web-mjesta moje web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="04a1f-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="04a1f-110">Ta je postavka po zadanom postavljena na **sve osim za vanjske korisnike**.</span><span class="sxs-lookup"><span data-stu-id="04a1f-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="04a1f-111">Kada dodate korisnika, korisnike ili grupu, provjerite je li odabran dodani korisnik, korisnici ili grupa, pomaknite se do odjeljka **dozvole** , a zatim potvrdite okvir pokraj **stvaranja osobnog web-mjesta (obavezno za osobno skladištenje, sažetak sadržaja vijesti i praćeni sadržaj)**.</span><span class="sxs-lookup"><span data-stu-id="04a1f-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="04a1f-112">Kliknite **u redu**, a zatim neka korisnik potraži na stranici servisa OneDrive da bi stvorio web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="04a1f-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
