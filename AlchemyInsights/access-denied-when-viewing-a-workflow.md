---
title: Pristup odbijen kada gledate tijeka rada
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747740"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="26340-102">Pristup odbijen kada gledate tijeka rada</span><span class="sxs-lookup"><span data-stu-id="26340-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="26340-103">SharePoint 2013 tijekovi rada pokušati poslati poruku e-pošte SharePoint grupi može uspjeti s poruku o pogrešci "Pristup je odbijen" ako članstva SharePoint grupe ne postavite svima.</span><span class="sxs-lookup"><span data-stu-id="26340-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="26340-104">**Da biste riješili taj problem, učinite sljedeće korake:**</span><span class="sxs-lookup"><span data-stu-id="26340-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="26340-105">Dopusti svima da biste vidjeli članovi SharePoint grupe.</span><span class="sxs-lookup"><span data-stu-id="26340-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="26340-106">Uklonite SharePoint grupu iz Prima ili Kopija redak e-pošte.</span><span class="sxs-lookup"><span data-stu-id="26340-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="26340-107">Izričito dodati korisnike da Prima ili Kopija redak ako vidljivost članstva ne može promijeniti za SharePoint grupu.</span><span class="sxs-lookup"><span data-stu-id="26340-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="26340-108">Za prikaz više pojedinosti pogledajte [HTTP neovlašteno za /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="26340-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  