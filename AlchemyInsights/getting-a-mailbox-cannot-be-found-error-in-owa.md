---
title: 126 Pogreška pri dobivanju poštanskog sandučića nije pronađena u aplikaciji OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426654"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="3b22c-102">Nije pronađena pogreška poštanskog sandučića u programu Outlook na webu?</span><span class="sxs-lookup"><span data-stu-id="3b22c-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="3b22c-103">Ako koristite Outlook na webu i  ne možete pronaći poštanski sandučić radi pogreške, račun koji ste koristili za povezivanje s programom Outlook na webu nema licencu za Exchange Online i stoga s računom nije povezan nijedan poštanski sandučić.</span><span class="sxs-lookup"><span data-stu-id="3b22c-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="3b22c-104">Administrator može dodijeliti licencu vašem računu na sljedeći način:</span><span class="sxs-lookup"><span data-stu-id="3b22c-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="3b22c-105">Otvorite centar za administratore sustava [Microsoft 365](https://portal.office.com/adminportal/home#/homepage) i otvorite **odjeljak** Aktivni korisnici u odjeljku Korisnici, a zatim odaberite korisnika koji vidi pogrešku. </span><span class="sxs-lookup"><span data-stu-id="3b22c-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="3b22c-106">Na stranici korisnika koja će  se otvoriti idite na  odjeljak Licence i aplikacije, odaberite odgovarajuću vrijednost Lokacije i dodijelite licencu koja sadrži Exchange Online (proširite licencu da biste vidjeli pojedinosti o njemu).</span><span class="sxs-lookup"><span data-stu-id="3b22c-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="3b22c-107">Kada završite, kliknite **Spremi promjene**.</span><span class="sxs-lookup"><span data-stu-id="3b22c-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="3b22c-108">U nekim slučajevima, ako je licenca već dodijeljena korisničkom računu, uklanjanje i ponovno dodjeljivanje licence pridonosi rješavanju problema i pravilnom dodjeljivanju resursa u sustavu:</span><span class="sxs-lookup"><span data-stu-id="3b22c-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="3b22c-109">Provjerite jesu li vaše pretplate na M365 Exchange Online (i druge, ako imate neku) trenutnu i nisu nedavno istekle.</span><span class="sxs-lookup"><span data-stu-id="3b22c-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="3b22c-110">Kada provjerite nije li vaša pretplata istekla i dodijeljena mu je valjana licenca, može biti potrebno do 24 sata da se licenca dodijeli, pa ćete možda morati pričekati da se problem riješi.</span><span class="sxs-lookup"><span data-stu-id="3b22c-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="3b22c-111">Dodatne informacije potražite u članku [Dodjela licenci i upravljanje njima.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="3b22c-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>