---
title: Pristup odbijen kada gledate tijeka rada
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28279815"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="76b1e-102">Pristup odbijen kada gledate tijeka rada</span><span class="sxs-lookup"><span data-stu-id="76b1e-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="76b1e-103">SharePoint 2013 tijekovi rada pokušati poslati poruku e-pošte SharePoint grupi može uspjeti s poruku o pogrešci "Pristup je odbijen" ako članstva SharePoint grupe ne postavite svima.</span><span class="sxs-lookup"><span data-stu-id="76b1e-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="76b1e-104">**Da biste riješili taj problem, učinite sljedeće korake:**</span><span class="sxs-lookup"><span data-stu-id="76b1e-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="76b1e-105">Dopusti svima da biste vidjeli članovi SharePoint grupe.</span><span class="sxs-lookup"><span data-stu-id="76b1e-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="76b1e-106">Uklonite SharePoint grupu iz Prima ili Kopija redak e-pošte.</span><span class="sxs-lookup"><span data-stu-id="76b1e-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="76b1e-107">Izričito dodati korisnike da Prima ili Kopija redak ako vidljivost članstva ne može promijeniti za SharePoint grupu.</span><span class="sxs-lookup"><span data-stu-id="76b1e-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="76b1e-108">Za prikaz više pojedinosti pogledajte [HTTP neovlašteno za /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="76b1e-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

