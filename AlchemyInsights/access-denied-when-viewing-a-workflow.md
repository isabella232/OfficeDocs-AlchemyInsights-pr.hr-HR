---
title: Pristup je odbijen prilikom pregledavanja tijeka rada
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687322"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="83848-102">Pristup je odbijen prilikom pregledavanja tijeka rada</span><span class="sxs-lookup"><span data-stu-id="83848-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="83848-103">Tijekovi rada sustava SharePoint 2013 koji pokušaju slanja e-pošte sharepoint grupi možda neće uspjeti s porukom o pogrešci "Pristup je odbijen" ako članstvo u sharepoint grupi nije postavljeno na Svi.</span><span class="sxs-lookup"><span data-stu-id="83848-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="83848-104">**Da biste riješili taj problem, učinite sljedeće:**</span><span class="sxs-lookup"><span data-stu-id="83848-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="83848-105">Dopustite svima da vide članove SharePoint grupe.</span><span class="sxs-lookup"><span data-stu-id="83848-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="83848-106">Uklonite sharepoint grupu iz retka Prima ili KOPIJA e-pošte.</span><span class="sxs-lookup"><span data-stu-id="83848-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="83848-107">Eksplicitno dodajte korisnike u redak Prima ili KOPIJA ako se vidljivost članstva ne može promijeniti za SharePoint grupu.</span><span class="sxs-lookup"><span data-stu-id="83848-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="83848-108">Da biste vidjeli više detalja, pogledajte [HTTP Neovlašteno na /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="83848-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  