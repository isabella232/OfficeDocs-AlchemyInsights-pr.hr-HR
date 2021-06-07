---
title: Nije moguće aktivirati Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798672"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="d9b18-102">Nije moguće aktivirati Office</span><span class="sxs-lookup"><span data-stu-id="d9b18-102">Unable to activate Office</span></span>

<span data-ttu-id="d9b18-103">**Napomena:** ako koristite stariju verziju programa Windows (npr. Windows 7), provjerite je li TLS 1.2 omogućen kao zadani.</span><span class="sxs-lookup"><span data-stu-id="d9b18-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="d9b18-104">Dodatne informacije potražite u članku Ažuriranje radi omogućivanja [TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)kao zadanih sigurnih protokola u aplikaciji WinHTTP u Windows .</span><span class="sxs-lookup"><span data-stu-id="d9b18-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="d9b18-105">Provjerite je li status vaše pretplate istekao.</span><span class="sxs-lookup"><span data-stu-id="d9b18-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="d9b18-106">Provjerite imate li pretplatu koja omogućuje klijentske licence, kao što su Office 365 Business ili Business premium, te provjerite je [li korisniku dodijeljena licenca](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="d9b18-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="d9b18-107">Provjerite je li se korisnik prijavljuje u Office s pomoću istog računa na koji je dodijeljena licenca.</span><span class="sxs-lookup"><span data-stu-id="d9b18-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="d9b18-108">Da biste saznali postoje li poznati problemi sa servisom, pogledajte članak [Stranica o stanju servisa za Office 365](/office365/enterprise/view-service-health).</span><span class="sxs-lookup"><span data-stu-id="d9b18-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="d9b18-109">Provjerite vatrozid, antivirusni softver i postavke proxyja da biste provjerili ne blokiraju li Microsoft 365 aplikacijama pristup internetu.</span><span class="sxs-lookup"><span data-stu-id="d9b18-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="d9b18-110">Pogledajte [URL-ovi i rasponi IP adresa za Office 365](/office365/enterprise/urls-and-ip-address-ranges "URL-ovi i rasponi IP adresa za Office 365").</span><span class="sxs-lookup"><span data-stu-id="d9b18-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="d9b18-111">**Savjet** Na Windows uređajima možemo dijagnosticirati i automatski riješiti nekoliko uobičajenih problema Office za prijavu.</span><span class="sxs-lookup"><span data-stu-id="d9b18-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="d9b18-112">Preuzmite i pokrenite **[Microsoftovu pomoćnik za podršku i oporavak da](https://aka.ms/SaRA-OfficeSignInScenario)** biste koristili naš automatizirani alat.</span><span class="sxs-lookup"><span data-stu-id="d9b18-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="d9b18-113">Primijenite sljedeće radnje uklanjanja poteškoća:</span><span class="sxs-lookup"><span data-stu-id="d9b18-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="d9b18-114">Otvorite aplikaciju sustava Office i [odjavite se](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) s postojećih korisničkih računa.</span><span class="sxs-lookup"><span data-stu-id="d9b18-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="d9b18-115">[Uklonite](/microsoft-365/admin/manage/remove-licenses-from-users) i [ponovno dodijelite](/microsoft-365/admin/manage/assign-licenses-to-users) licencu sustava Office, a zatim se [prijavite u Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) s pomoću zahvaćenog korisničkog računa.</span><span class="sxs-lookup"><span data-stu-id="d9b18-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="d9b18-116">Pokrenite [alat za otklanjanje poteškoća s aktivacijom](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="d9b18-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="d9b18-117">Resetirajte stanje aktivacije sustava Office</span><span class="sxs-lookup"><span data-stu-id="d9b18-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Ponovno postavljanje Office aktivacijskog stanja")
- [<span data-ttu-id="d9b18-118">Provedite internetski popravak sustava Office</span><span class="sxs-lookup"><span data-stu-id="d9b18-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="d9b18-119">Dodatne rješenja za otklanjanje poteškoća potražite u sljedećim člancima:</span><span class="sxs-lookup"><span data-stu-id="d9b18-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="d9b18-120">Pogreške zbog nelicenciranog proizvoda i pogreške s aktivacijom u sustavu Office</span><span class="sxs-lookup"><span data-stu-id="d9b18-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="d9b18-121">Pogreška „Nažalost, ne možemo se povezati s vašim računom. Pokušajte ponovo kasnije” prilikom aktivacije sustava Office</span><span class="sxs-lookup"><span data-stu-id="d9b18-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)