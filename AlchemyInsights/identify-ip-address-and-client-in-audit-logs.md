---
title: Identificiranje IP adresu i klijent zapisnika nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539021"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="aa598-102">Identificiranje IP adresu i klijent zapisnika nadzora</span><span class="sxs-lookup"><span data-stu-id="aa598-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="aa598-103">IP adresa koja odgovara aktivnost korisnika Office 365 ili administrator je prikazan u zapisnike nadzora.</span><span class="sxs-lookup"><span data-stu-id="aa598-103">The IP address that corresponds to an activity by an Office 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="aa598-104">Klijent informacije također prijavljeni.</span><span class="sxs-lookup"><span data-stu-id="aa598-104">The client information is also logged.</span></span> <span data-ttu-id="aa598-105">Ovdje su koraci za označavanje takve informacije</span><span class="sxs-lookup"><span data-stu-id="aa598-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="aa598-106">Prijavite se u sustav [Office 365 sigurnosne & usklađenosti centar](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="aa598-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="aa598-107">Idi na **pretraživanje** > stranicu za**pretraživanje zapisnika nadzora** .</span><span class="sxs-lookup"><span data-stu-id="aa598-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="aa598-108">Ako vas zanima određenih aktivnosti, odaberite ga s popisa **aktivnosti** .</span><span class="sxs-lookup"><span data-stu-id="aa598-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="aa598-109">Ako nije, sve aktivnosti će biti vraćene za odabranog korisnika (Zadana postavka).</span><span class="sxs-lookup"><span data-stu-id="aa598-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="aa598-110">**Napomena**: određene aktivnosti možda neće biti dostupne u izborniku **aktivnosti** ; Međutim, one stavke nadzora će se vratiti ako je **Pokaži rezultate za sve aktivnosti** odabrane (Zadana postavka).</span><span class="sxs-lookup"><span data-stu-id="aa598-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="aa598-111">Navedite korisničko ime u polju **korisnicima** , odaberite odgovarajući datum raspon za aktivnost, a zatim **pretraživanje**.</span><span class="sxs-lookup"><span data-stu-id="aa598-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="aa598-112">U rezultatima pogledajte IP adresu za tu aktivnost u oknu rezultata.</span><span class="sxs-lookup"><span data-stu-id="aa598-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="aa598-113">Odaberite zapis nadzora da biste vidjeli detaljne informacije Potpaleta **detalje** (na primjer, klijent, korisnik izvršiti akciju, itd.).</span><span class="sxs-lookup"><span data-stu-id="aa598-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="aa598-114">Dodatne informacije potražite u [pronalaženju IP adresu računala koristiti za pristup compromised računa](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="aa598-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
