---
title: Nije moguće aktivirati Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 3a42c221047e7be6a173694cd45136baa6bff39a
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704922"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="32832-102">Nije moguće aktivirati Office</span><span class="sxs-lookup"><span data-stu-id="32832-102">Unable to activate Office</span></span>

- <span data-ttu-id="32832-103">Provjerite je li status vaše pretplate istekao.</span><span class="sxs-lookup"><span data-stu-id="32832-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="32832-104">Provjerite imate li pretplatu koja omogućuje klijentske licence, kao što je Office 365 Business ili Business Premium te [Provjerite je li korisnik dodijelio licencu](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="32832-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="32832-105">Provjerite je li se korisnik prijavljuje u Office s pomoću istog računa na koji je dodijeljena licenca.</span><span class="sxs-lookup"><span data-stu-id="32832-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="32832-106">Da biste saznali postoje li poznati problemi sa servisom, pogledajte članak [Stranica o stanju servisa za Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health).</span><span class="sxs-lookup"><span data-stu-id="32832-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="32832-107">Provjerite vatrozid, antivirusni softver i postavke proxy poslužitelja da biste potvrdili da ne blokiraju pristup aplikacijama programa Microsoft 365 na Internet.</span><span class="sxs-lookup"><span data-stu-id="32832-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="32832-108">Pogledajte [URL-ovi i rasponi IP adresa za Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "URL-ovi i rasponi IP adresa za Office 365").</span><span class="sxs-lookup"><span data-stu-id="32832-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="32832-109">**Savjet** Na uređajima sa sustavom Windows možemo dijagnosticirati i automatski riješiti nekoliko običnih problema s prijavom u Office.</span><span class="sxs-lookup"><span data-stu-id="32832-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="32832-110">Preuzmite i pokrenite  **[Microsoftov pomoćnik za podršku i oporavak](https://aka.ms/SaRA-OfficeSignInScenario)** da biste koristili naš automatizirani alat.</span><span class="sxs-lookup"><span data-stu-id="32832-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="32832-111">Primijenite sljedeće radnje uklanjanja poteškoća:</span><span class="sxs-lookup"><span data-stu-id="32832-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="32832-112">Otvorite aplikaciju sustava Office i [odjavite se](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) s postojećih korisničkih računa.</span><span class="sxs-lookup"><span data-stu-id="32832-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="32832-113">[Uklonite](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) i [ponovno dodijelite](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licencu sustava Office, a zatim se [prijavite u Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) s pomoću zahvaćenog korisničkog računa.</span><span class="sxs-lookup"><span data-stu-id="32832-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="32832-114">Pokrenite [alat za otklanjanje poteškoća s aktivacijom](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="32832-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="32832-115">Resetirajte stanje aktivacije sustava Office</span><span class="sxs-lookup"><span data-stu-id="32832-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Ponovno postavljanje stanja aktivacije sustava Office")
- [<span data-ttu-id="32832-116">Provedite internetski popravak sustava Office</span><span class="sxs-lookup"><span data-stu-id="32832-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="32832-117">Dodatne rješenja za otklanjanje poteškoća potražite u sljedećim člancima:</span><span class="sxs-lookup"><span data-stu-id="32832-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="32832-118">Pogreške zbog nelicenciranog proizvoda i pogreške s aktivacijom u sustavu Office</span><span class="sxs-lookup"><span data-stu-id="32832-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="32832-119">Pogreška „Nažalost, ne možemo se povezati s vašim računom. Pokušajte ponovo kasnije” prilikom aktivacije sustava Office</span><span class="sxs-lookup"><span data-stu-id="32832-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)