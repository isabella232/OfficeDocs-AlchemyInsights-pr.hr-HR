---
title: Identificiranje IP adresu i klijent zapisnika nadzora
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 7e30a638de5926aa11b8ae637613a48076d7bdc9
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/23/2019
ms.locfileid: "32416930"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="8cb8a-102">Identificiranje IP adresu i klijent zapisnika nadzora</span><span class="sxs-lookup"><span data-stu-id="8cb8a-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="8cb8a-103">IP adresa koja odgovara aktivnost korisnik ili administrator je prikazan u zapisnike nadzora.</span><span class="sxs-lookup"><span data-stu-id="8cb8a-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="8cb8a-104">Klijent informacije također prijavljeni.</span><span class="sxs-lookup"><span data-stu-id="8cb8a-104">The client information is also logged.</span></span> <span data-ttu-id="8cb8a-105">Ovdje su koraci za označavanje takve informacije</span><span class="sxs-lookup"><span data-stu-id="8cb8a-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="8cb8a-106">Prijavite se u sustav [Office 365 sigurnosne & usklađenosti centar](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="8cb8a-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="8cb8a-107">Kliknite **za pretraživanje i istraživanja** i odaberite **Pretraživanje zapisnika nadzora**.</span><span class="sxs-lookup"><span data-stu-id="8cb8a-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="8cb8a-108">Ako vas zanima određenih aktivnosti, odaberite ga s popisa **aktivnosti** .</span><span class="sxs-lookup"><span data-stu-id="8cb8a-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="8cb8a-109">Ako nije, sve aktivnosti će biti vraćene za odabranog korisnika (Zadana postavka).</span><span class="sxs-lookup"><span data-stu-id="8cb8a-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="8cb8a-110">**Napomena**: određene aktivnosti možda neće biti dostupne u izborniku **aktivnosti** ; Međutim, one stavke nadzora će se vratiti ako je **Pokaži rezultate za sve aktivnosti** odabrane (Zadana postavka).</span><span class="sxs-lookup"><span data-stu-id="8cb8a-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="8cb8a-111">Navedite korisničko ime u polju **korisnicima** , odaberite odgovarajući datum raspon za aktivnost, a zatim **pretraživanje**.</span><span class="sxs-lookup"><span data-stu-id="8cb8a-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="8cb8a-112">U rezultatima pogledajte IP adresu za tu aktivnost u oknu rezultata.</span><span class="sxs-lookup"><span data-stu-id="8cb8a-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="8cb8a-113">Odaberite zapis nadzora da biste vidjeli detaljne informacije Potpaleta **detalje** (na primjer, klijent, korisnik izvršiti akciju, itd.).</span><span class="sxs-lookup"><span data-stu-id="8cb8a-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="8cb8a-114">Dodatne informacije potražite u [pronalaženju IP adresu računala koristiti za pristup compromised računa](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="8cb8a-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
