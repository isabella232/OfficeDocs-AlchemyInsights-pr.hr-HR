---
title: Prepoznavanje IP adresa i klijenta u evidenciji nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668302"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="202c5-102">Prepoznavanje IP adresa i klijenta u evidenciji nadzora</span><span class="sxs-lookup"><span data-stu-id="202c5-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="202c5-103">IP adresa koja odgovara aktivnosti korisnika sustava Microsoft 365 ili administratora prikazuje se u evidenciji nadzora.</span><span class="sxs-lookup"><span data-stu-id="202c5-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="202c5-104">Prijavljeni su i podaci o klijentu.</span><span class="sxs-lookup"><span data-stu-id="202c5-104">The client information is also logged.</span></span> <span data-ttu-id="202c5-105">Evo koraka za identifikaciju takvih informacija</span><span class="sxs-lookup"><span data-stu-id="202c5-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="202c5-106">Prijavite se u [centar za sigurnost & sustava Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="202c5-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="202c5-107">Idite na stranicu **Search**  >  **pretraživanja zapisnika nadzora** pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="202c5-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="202c5-108">Ako ste zainteresirani za određenu aktivnost, odaberite je na popisu **aktivnosti** .</span><span class="sxs-lookup"><span data-stu-id="202c5-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="202c5-109">Ako ne, sve će se aktivnosti vratiti odabranom korisniku (zadana postavka).</span><span class="sxs-lookup"><span data-stu-id="202c5-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="202c5-110">**Pažnja**: određene aktivnosti možda neće biti dostupne na izborniku **aktivnosti** ; No te će se stavke u reviziji vratiti ako je odabrano **Prikaz rezultata za sve aktivnosti** (zadana postavka).</span><span class="sxs-lookup"><span data-stu-id="202c5-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="202c5-111">Navedite korisničko ime u polju **korisnici** , odaberite odgovarajući raspon datuma za aktivnost, a zatim kliknite **Pretraži**.</span><span class="sxs-lookup"><span data-stu-id="202c5-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="202c5-112">U rezultatima možete vidjeti IP adresu za tu aktivnost u oknu rezultata.</span><span class="sxs-lookup"><span data-stu-id="202c5-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="202c5-113">Odaberite zapis nadzora da biste vidjeli detaljne informacije u nastavku za **detalje** (na primjer, klijent, korisnik koji je izvršio akciju, itd.).</span><span class="sxs-lookup"><span data-stu-id="202c5-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="202c5-114">Dodatne informacije potražite u članku [Pronalaženje IP adrese računala koje se koristi za pristup kompromitiranom računu](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="202c5-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
