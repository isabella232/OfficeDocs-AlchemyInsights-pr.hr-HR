---
title: Problem s jednim korisnikom
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429469"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="f1d05-102">Problem s jednim korisnikom</span><span class="sxs-lookup"><span data-stu-id="f1d05-102">Problem with single user</span></span>

- <span data-ttu-id="f1d05-103">Korisniku možda nije dodijeljena dodjela resursa jer servis još nije imao priliku procijeniti korisnika.</span><span class="sxs-lookup"><span data-stu-id="f1d05-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="f1d05-104">Pregledajte upute o tome koliko traje dodjela resursa, kao i traka tijeka na stranici Konfiguracija dodjele resursa.</span><span class="sxs-lookup"><span data-stu-id="f1d05-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="f1d05-105">Ako je stanje stanja koje je navedeno u odjeljku Dodatne pojedinosti prije datuma kada je korisnik stvoren/ažuriran/izbrisan, to znači da još nismo procijenili korisnika.</span><span class="sxs-lookup"><span data-stu-id="f1d05-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="f1d05-106">U ovom scenariju najbolje je čekati da servis za dodjelu resursa završi.</span><span class="sxs-lookup"><span data-stu-id="f1d05-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="f1d05-107">Imajte na umu da je naš servis svjestan samo promjena korisnika u izvornom sustavu (Cloud HR).</span><span class="sxs-lookup"><span data-stu-id="f1d05-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="f1d05-108">Mora postojati valjana promjena u izvornom sustavu za Azure AD za prepoznavanje promjene i njihovo strujanje u Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f1d05-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="f1d05-109">Servis za dodjelu resursa procijenio je korisnika i utvrdio da mu se ne treba dodijeliti:</span><span class="sxs-lookup"><span data-stu-id="f1d05-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="f1d05-110">Ako ste postavili filtar zasnovan na atributu, Provjerite zadovoljava li korisnik kriterij koji ste naveli.</span><span class="sxs-lookup"><span data-stu-id="f1d05-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="f1d05-111">Ako korisnici već postoje u ciljnom sustavu i stanju korisnika u izvoru i ciljnom podudaranju, nećemo poduzeti nikakve daljnje akcije.</span><span class="sxs-lookup"><span data-stu-id="f1d05-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="f1d05-112">Servis za dodjelu resursa pokušao je dodijeliti korisniku i nije uspio.</span><span class="sxs-lookup"><span data-stu-id="f1d05-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="f1d05-113">U tim scenarijima Pregledajte karticu Otklanjanje poteškoća i preporuke u zapisnicima za dodjelu resursa:</span><span class="sxs-lookup"><span data-stu-id="f1d05-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="f1d05-114">Potreban atribut na korisniku možda nema u lokalnom servisu Active Directory ili Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1d05-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="f1d05-115">Primjerice, pravila stvaranja userPrincipalName ili sAMAccountName ne stvaraju pravu vrijednost.</span><span class="sxs-lookup"><span data-stu-id="f1d05-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="f1d05-116">Podudarni atribut (obično IDZaposlenika) ne rješava jedinstven korisnik u lokalnom servisu Active Directory ili Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1d05-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="f1d05-117">Na primjer, postoje dva korisnika s istim Zaposlajnim osobama u aplikaciji AD, a servis vraća šifru pogreške koja označava duplicirane ciljne unose za isti izvorni unos.</span><span class="sxs-lookup"><span data-stu-id="f1d05-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="f1d05-118">Da biste pregledali zapisnike za pojedinačne korisnike i grupe, pročitajte članak [Pregled zapisnika dodjele resursa za problem s određenim korisnikom](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span><span class="sxs-lookup"><span data-stu-id="f1d05-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
