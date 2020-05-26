---
title: 618 Pravila zajedničkog korištenja kalendara
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/26/2020
ms.locfileid: "44372991"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="98280-102">Pogreška pravila prilikom zajedničkog korištenja kalendara</span><span class="sxs-lookup"><span data-stu-id="98280-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="98280-103">Učinite nešto od sljedećeg, ovisno o situaciji:</span><span class="sxs-lookup"><span data-stu-id="98280-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="98280-104">Povežite se sa sustavom Exchange Online pomoću udaljene ljuske PowerShell.</span><span class="sxs-lookup"><span data-stu-id="98280-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="98280-105">Dodatne informacije [potražite u odjeljku Povezivanje sa sustavom Exchange Online pomoću udaljene ljuske PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="98280-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="98280-106">Na lokalnom poslužitelju otvorite ljusku za upravljanje sustavom Exchange.</span><span class="sxs-lookup"><span data-stu-id="98280-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="98280-107">Odredite pravila zajedničkog korištenja koja su dodijeljena korisniku.</span><span class="sxs-lookup"><span data-stu-id="98280-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="98280-108">Da biste to učinili, pokrenite sljedeću naredbu i zabilježite vraćeno pravilo:</span><span class="sxs-lookup"><span data-stu-id="98280-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="98280-109">Ažurirajte pravila zajedničkog korištenja za korisnika.</span><span class="sxs-lookup"><span data-stu-id="98280-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="98280-110">Da biste to učinili, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="98280-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="98280-111">Otvorite centar za administratore sustava Exchange.</span><span class="sxs-lookup"><span data-stu-id="98280-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="98280-112">Kliknite **Organizacija**, a zatim dvokliknite pravilo koje je dodijeljeno korisniku u odjeljku **Pojedinačno zajedničko korištenje**.</span><span class="sxs-lookup"><span data-stu-id="98280-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="98280-113">Ovo je pravilo koje je vraćeno u koraku 2.</span><span class="sxs-lookup"><span data-stu-id="98280-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="98280-114">Na stranici Pravilo zajedničkog korištenja odaberite razinu zajedničkog korištenja kalendara koju želite dopustiti u **odjeljku Navedite koje informacije želite zajednički koristiti**; kliknite **Spremi**.</span><span class="sxs-lookup"><span data-stu-id="98280-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="98280-115">Dodatne informacije potražite [u odjeljku "Pravila ne dopuštaju dodjeljivanje dozvola na ovoj razini jednom ili više primatelja" kada korisnik pokuša zajednički koristiti kalendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="98280-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
