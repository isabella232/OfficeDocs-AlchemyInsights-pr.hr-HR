---
title: Pristup je odbijen prilikom pregledavanja tijeka rada
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688794"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="0ef4a-102">Pristup je odbijen prilikom pregledavanja tijeka rada</span><span class="sxs-lookup"><span data-stu-id="0ef4a-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="0ef4a-103">Tijekovi rada sustava SharePoint 2013 koji pokušaju poslati poruku e-pošte u grupu sustava SharePoint ne uspijevaju s porukom o pogrešci "Access denied" ako članstvo u grupi sustava SharePoint nije postavljeno na sve.</span><span class="sxs-lookup"><span data-stu-id="0ef4a-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="0ef4a-104">**Da biste riješili taj problem, učinite sljedeće:**</span><span class="sxs-lookup"><span data-stu-id="0ef4a-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="0ef4a-105">Dopusti svima da vide članove grupe sustava SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0ef4a-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="0ef4a-106">Uklonite grupu sustava SharePoint iz retka prima ili kopija poruke e-pošte.</span><span class="sxs-lookup"><span data-stu-id="0ef4a-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="0ef4a-107">Eksplicitno Dodajte korisnike u redak Prima ili kopija ako se vidljivost članstva ne može promijeniti za grupu sustava SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0ef4a-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="0ef4a-108">Da biste pogledali više detalja, pogledajte [http neovlašten za/_vti_bin/Client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="0ef4a-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  