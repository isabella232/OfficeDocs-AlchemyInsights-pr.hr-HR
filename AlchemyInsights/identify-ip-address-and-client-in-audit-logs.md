---
title: Prepoznavanje IP adrese i klijenta u zapisnicima nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508908"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="f354f-102">Prepoznavanje IP adrese i klijenta u zapisnicima nadzora</span><span class="sxs-lookup"><span data-stu-id="f354f-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="f354f-103">IP adresa koja odgovara aktivnosti korisnika ili administratora sustava Microsoft 365 prikazana je u zapisnicima nadzora.</span><span class="sxs-lookup"><span data-stu-id="f354f-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="f354f-104">Podaci o klijentu također su prijavljeni.</span><span class="sxs-lookup"><span data-stu-id="f354f-104">The client information is also logged.</span></span> <span data-ttu-id="f354f-105">Evo koraka za utvrđivanje takvih informacija</span><span class="sxs-lookup"><span data-stu-id="f354f-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="f354f-106">Prijavite se u Centar za [usklađenost sa sigurnosnim & sustava Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="f354f-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="f354f-107">Idite **Search**na  >  stranicu za pretraživanje**zapisnika nadzora** pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="f354f-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="f354f-108">Ako vas zanima određena aktivnost, odaberite je na popisu **Aktivnosti.**</span><span class="sxs-lookup"><span data-stu-id="f354f-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="f354f-109">Ako nije, sve aktivnosti bit će vraćene za odabranog korisnika (zadana postavka).</span><span class="sxs-lookup"><span data-stu-id="f354f-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="f354f-110">**Napomena**: Određene aktivnosti možda neće biti dostupne u izborniku **Aktivnosti;** međutim, te stavke nadzora vratit će se ako je **odabrana prikazana prikazuje rezultata za sve aktivnosti** (zadana postavka).</span><span class="sxs-lookup"><span data-stu-id="f354f-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="f354f-111">Navedite korisničko ime u polju **Korisnici,** odaberite odgovarajući datumski raspon aktivnosti, a zatim kliknite **Pretraži**.</span><span class="sxs-lookup"><span data-stu-id="f354f-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="f354f-112">U rezultatima možete vidjeti IP adresu za tu aktivnost u oknu rezultata.</span><span class="sxs-lookup"><span data-stu-id="f354f-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="f354f-113">Odaberite zapis nadzora da biste vidjeli detaljne informacije u potpaleti **Detalji** (na primjer, Klijent, Korisnik koji je izvršio akciju itd.).</span><span class="sxs-lookup"><span data-stu-id="f354f-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="f354f-114">Dodatne informacije [potražite u odjeljku Pronalaženje IP adrese računala koje se koristi za pristup kompromitiranom računu](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="f354f-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
