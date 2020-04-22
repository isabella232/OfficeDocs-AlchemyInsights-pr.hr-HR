---
title: Prepoznavanje IP adrese i klijenta u zapisnikima nadzora
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
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716380"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="26933-102">Prepoznavanje IP adrese i klijenta u zapisnikima nadzora</span><span class="sxs-lookup"><span data-stu-id="26933-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="26933-103">IP adresa koja odgovara aktivnosti korisnika ili administratora sustava Microsoft 365 prikazana je u zapisnikima nadzora.</span><span class="sxs-lookup"><span data-stu-id="26933-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="26933-104">Podaci o klijentu također su prijavljeni.</span><span class="sxs-lookup"><span data-stu-id="26933-104">The client information is also logged.</span></span> <span data-ttu-id="26933-105">Evo koraka za utvrđivanje takvih informacija</span><span class="sxs-lookup"><span data-stu-id="26933-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="26933-106">Prijavite se u Centar za [sigurnost sustava Microsoft 365 & .](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="26933-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="26933-107">Idite na stranicu **za** > **pretraživanje zapisnika nadzora** pretraživanja.</span><span class="sxs-lookup"><span data-stu-id="26933-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="26933-108">Ako ste zainteresirani za određenu aktivnost, odaberite je s popisa **Aktivnosti.**</span><span class="sxs-lookup"><span data-stu-id="26933-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="26933-109">Ako nije, sve aktivnosti bit će vraćene za odabranog korisnika (zadana postavka).</span><span class="sxs-lookup"><span data-stu-id="26933-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="26933-110">**Napomena**: Određene aktivnosti možda neće biti dostupne u izborniku **Aktivnosti;** međutim, te će stavke nadzora biti vraćene ako je **odabrana mogućnost Prikaži rezultate za sve aktivnosti** (zadana postavka).</span><span class="sxs-lookup"><span data-stu-id="26933-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="26933-111">Navedite korisničko ime u polju **Korisnici,** odaberite odgovarajući datumski raspon aktivnosti, a zatim kliknite **Pretraži**.</span><span class="sxs-lookup"><span data-stu-id="26933-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="26933-112">U rezultatima možete vidjeti IP adresu za tu aktivnost u oknu s rezultatima.</span><span class="sxs-lookup"><span data-stu-id="26933-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="26933-113">Odaberite zapis nadzora da biste vidjeli detaljne informacije u potpaleti **Detalji** (na primjer, Klijent, Korisnik koji je izvršio akciju itd.).</span><span class="sxs-lookup"><span data-stu-id="26933-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="26933-114">Dodatne informacije [potražite u odjeljku Pronalaženje IP adrese računala koje se koristi za pristup ugroženom računu](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="26933-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
