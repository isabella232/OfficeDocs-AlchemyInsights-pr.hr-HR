---
title: Uklanjanje prethodnih verzija sustava Office MSI
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680660"
---
# <a name="remove-prior-msi-versions-of-office"></a><span data-ttu-id="3e86f-102">Uklanjanje prethodnih verzija sustava Office MSI</span><span class="sxs-lookup"><span data-stu-id="3e86f-102">Remove prior MSI versions of Office</span></span>

<span data-ttu-id="3e86f-103">Preporučujemo da prije instalacije sustava Office 365 ProPlus uklonite prethodne verzije sustava Office Windows Installer (MSI).</span><span class="sxs-lookup"><span data-stu-id="3e86f-103">I recommend removing prior Windows Installer (MSI) versions of Office before installing Office 365 ProPlus.</span></span> <span data-ttu-id="3e86f-104">Evo kako to učiniti:</span><span class="sxs-lookup"><span data-stu-id="3e86f-104">Here's how to do this:</span></span>

1. <span data-ttu-id="3e86f-105">Ako ste koristili MSI za instalaciju sustava Office, možete koristiti alat za implementaciju sustava Office (ODT) da biste deinstalirali Office.</span><span class="sxs-lookup"><span data-stu-id="3e86f-105">If you used MSI to install Office, you can use the Office Deployment Tool (ODT) to uninstall Office.</span></span> <span data-ttu-id="3e86f-106">U datoteci **configuration.xml** možete koristiti element RemoveMSI.</span><span class="sxs-lookup"><span data-stu-id="3e86f-106">You can use the RemoveMSI element in your **configuration.xml** file.</span></span>
1. <span data-ttu-id="3e86f-107">Slijedite upute u ovom članku: [centar za sigurnost & sustava Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="3e86f-107">Follow the instruction in this article: [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span></span>