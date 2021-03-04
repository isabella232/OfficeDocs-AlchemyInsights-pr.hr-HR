---
title: Pronalaženje IP adrese u zapisniku nadzora
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429291"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="db9a0-102">Pronalaženje IP adrese u zapisniku nadzora</span><span class="sxs-lookup"><span data-stu-id="db9a0-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="db9a0-103">IP adresa koja odgovara aktivnosti koju izvršava korisnik ili administrator prikazat će se u evidenciji nadzora.</span><span class="sxs-lookup"><span data-stu-id="db9a0-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="db9a0-104">Prijavljeni su i podaci o klijentu.</span><span class="sxs-lookup"><span data-stu-id="db9a0-104">The client information is also logged.</span></span> <span data-ttu-id="db9a0-105">Slijede upute za identifikaciju IP adrese:</span><span class="sxs-lookup"><span data-stu-id="db9a0-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="db9a0-106">Otvorite centar za [sigurnost & sustava Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="db9a0-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="db9a0-107">Odaberite **Pretraži pretragu**  >  **[zapisnika nadzora](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span><span class="sxs-lookup"><span data-stu-id="db9a0-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="db9a0-108">Ako vam se prikaže obavijest da morate uključiti nadzor, nastavite i uključite ga odmah.</span><span class="sxs-lookup"><span data-stu-id="db9a0-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="db9a0-109">Ako ta značajka nije omogućena, rezultati pretraživanja neće moći povući podatke iz prethodnih datuma.</span><span class="sxs-lookup"><span data-stu-id="db9a0-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="db9a0-110">Ako ste zainteresirani za određenu aktivnost, odaberite je na popisu **aktivnosti** . u suprotnom će se po zadanom vratiti sve aktivnosti za odabranog korisnika.</span><span class="sxs-lookup"><span data-stu-id="db9a0-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="db9a0-111">Primjetite da određene aktivnosti možda neće biti dostupne za odabir na izborniku **aktivnosti** ; No te će se stavke u reviziji vratiti ako je odabrano **Prikaz rezultata za sve aktivnosti** (zadana postavka).</span><span class="sxs-lookup"><span data-stu-id="db9a0-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="db9a0-112">Navedite raspon datuma, a zatim u polju **korisnici** odaberite korisničko ime za korisnika koje želite istražiti.</span><span class="sxs-lookup"><span data-stu-id="db9a0-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="db9a0-113">Odaberite **Pretraživanje**.</span><span class="sxs-lookup"><span data-stu-id="db9a0-113">Select **Search**.</span></span> <span data-ttu-id="db9a0-114">Aktivnosti se prikazuju u odjeljku **Rezultati**.</span><span class="sxs-lookup"><span data-stu-id="db9a0-114">The activities appear under **Results**.</span></span> <span data-ttu-id="db9a0-115">Možete vidjeti IP adresu za svaku aktivnost.</span><span class="sxs-lookup"><span data-stu-id="db9a0-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="db9a0-116">Da biste pogledali detalje, odaberite aktivnost, a zatim odaberite **Dodatne informacije**.</span><span class="sxs-lookup"><span data-stu-id="db9a0-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="db9a0-117">Dodatne informacije potražite u članku pretraživanje [zapisnika nadzora sustava Office 365 radi otklanjanja običnih scenarija](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="db9a0-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>