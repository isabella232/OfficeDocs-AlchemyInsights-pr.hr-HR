---
title: Rješavanje problema s aplikacijama sustava Microsoft 365 Nije moglo pronaći povezanu poruku o licencama sustava Office
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
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816480"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="e8a79-102">Popravljanje poruke aplikacije Microsoft 365 "Nije bilo pridruženih licenci za office"</span><span class="sxs-lookup"><span data-stu-id="e8a79-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="e8a79-103">Ako primite ovu poruku, pokušajte sljedeće:</span><span class="sxs-lookup"><span data-stu-id="e8a79-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="e8a79-104">Provjerite postavke vatrozida, antivirusnog softvera i proxyja da biste potvrdili da ne blokiraju pristup internetu aplikacijama Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e8a79-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="e8a79-105">Pogledajte [URL-ove i raspone IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)adresa za Microsoft 365 .</span><span class="sxs-lookup"><span data-stu-id="e8a79-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="e8a79-106">Uklonite i [ponovno dodijelite licencu za Office za](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) zahvaćenog korisnika.</span><span class="sxs-lookup"><span data-stu-id="e8a79-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="e8a79-107">Otvorite aplikaciju sustava Office i [odjavite se](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) iz postojećih korisničkih računa.</span><span class="sxs-lookup"><span data-stu-id="e8a79-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="e8a79-108">Otvorite Postavke sustava Windows > **računi**  >  **e-& račune** i uklonite sve poslovne račune osim zahvaćenog računa.</span><span class="sxs-lookup"><span data-stu-id="e8a79-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="e8a79-109">Otvorite Postavke sustava Windows > **računima Pristup** poslovnoj ili  >  **školskoj** školi i prekinite vezu sa svim poslovnim računima osim zahvaćenog računa.</span><span class="sxs-lookup"><span data-stu-id="e8a79-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="e8a79-110">Ponovno postavite stanje aktivacije sustava Office.</span><span class="sxs-lookup"><span data-stu-id="e8a79-110">Reset the Office activation state.</span></span> <span data-ttu-id="e8a79-111">[Saznajte kako](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="e8a79-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="e8a79-112">[Prijavite se pomoću](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) zahvaćenog korisničkog računa.</span><span class="sxs-lookup"><span data-stu-id="e8a79-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="e8a79-113">Dodatna rješenja za otklanjanje poteškoća potražite u članku [Pogreške nelicencirani proizvod i aktivacija u sustavu Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="e8a79-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>