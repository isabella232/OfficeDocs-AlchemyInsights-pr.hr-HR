---
title: OneDrive za tvrtke Web OneDrive preusmjerava na Delve
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
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799981"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="592cd-102">Preusmjereno na Delve nakon klika na OneDrive</span><span class="sxs-lookup"><span data-stu-id="592cd-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="592cd-103">Pogledajte naš detaljni vodič [za otklanjanje poteškoća](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="592cd-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="592cd-104">Da bi riješio taj problem, administrator korisnicima mora dodijeliti pravo stvaranja web-mjesta Moja web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="592cd-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="592cd-105">To je zato što se stranica servisa OneDrive za tvrtke stvara na web-mjestima Moja web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="592cd-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="592cd-106">Da biste dodijelili to pravo, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="592cd-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="592cd-107">U centru za administratore sustava SharePoint kliknite **korisnički profili**.</span><span class="sxs-lookup"><span data-stu-id="592cd-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="592cd-108">U **odjeljku** Osobe kliknite Upravljanje **korisničkim dozvolama**.</span><span class="sxs-lookup"><span data-stu-id="592cd-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="592cd-109">Dodajte korisnike kojima su potrebne dozvole za stvaranje web-mjesta Moja web-mjesta.</span><span class="sxs-lookup"><span data-stu-id="592cd-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="592cd-110">Ta je postavka po zadanom postavljena na **Svi osim vanjskih korisnika**.</span><span class="sxs-lookup"><span data-stu-id="592cd-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="592cd-111">Kada dodate korisnika, korisnike ili grupu, provjerite je li odabran dodani korisnik,  korisnici ili grupa, pomaknite se do odjeljka s dozvolama, a zatim potvrdite okvir pokraj mogućnosti Stvaranje osobnog web-mjesta (obavezno za osobni prostor za pohranu, sažetke sadržaja vijesti **i praćeni sadržaj).**</span><span class="sxs-lookup"><span data-stu-id="592cd-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="592cd-112">Kliknite **U redu**, a zatim neka korisnik otvori stranicu servisa OneDrive da biste stvorili web-mjesto.</span><span class="sxs-lookup"><span data-stu-id="592cd-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
