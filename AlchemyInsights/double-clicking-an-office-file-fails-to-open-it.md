---
title: Dvoklikom na datoteku sustava Office ne uspijeva se otvoriti
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814797"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="2fa02-102">Dvoklikom na datoteku sustava Office ne uspijeva se otvoriti</span><span class="sxs-lookup"><span data-stu-id="2fa02-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="2fa02-103">Kada dvoklikom na datoteku sustava Office vidite da je program otvoren, ali se sama datoteka ne otvara.</span><span class="sxs-lookup"><span data-stu-id="2fa02-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="2fa02-104">Ili vam se može pojaviti pogreška: "Došlo je do problema prilikom slanja naredbe programu".</span><span class="sxs-lookup"><span data-stu-id="2fa02-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="2fa02-105">Za to postoji mnogo uzroka, ali dva su najčešće rješenja:</span><span class="sxs-lookup"><span data-stu-id="2fa02-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="2fa02-106">U programu Excel provjerite je li mogućnost DDE poništena.</span><span class="sxs-lookup"><span data-stu-id="2fa02-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="2fa02-107">Mogućnost se može pronaći stvaranjem nove radne knjige, a zatim odabirom mogućnosti **datoteka > mogućnosti > Dodatno**.</span><span class="sxs-lookup"><span data-stu-id="2fa02-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="2fa02-108">U **odjeljku Općenito** poništite okvir Zanemari **ostale aplikacije koje koriste dinamičku razmjenu podataka (DDE).**</span><span class="sxs-lookup"><span data-stu-id="2fa02-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="2fa02-109">Pokrenite mrežni popravak da biste vratili zadane postavke.</span><span class="sxs-lookup"><span data-stu-id="2fa02-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="2fa02-110">Kliknite gumb Start sustava Windows i potražite "Upravljačka ploča".</span><span class="sxs-lookup"><span data-stu-id="2fa02-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="2fa02-111">Otvorite **upravljačku ploču** i otvorite **Programi > Programi i značajke**.</span><span class="sxs-lookup"><span data-stu-id="2fa02-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="2fa02-112">Zatim desnom tipkom miša **kliknite Microsoft Office [Verzija]** pa **odaberite Promijeni > popravak putem interneta**.</span><span class="sxs-lookup"><span data-stu-id="2fa02-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="2fa02-113">Ako nijedno od tih rješenja ne funkcionira, potpuniji popis rješenja može se pronaći u članku podrške, [dvoklikom](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)na datoteku sustava Office ne možete je otvoriti .</span><span class="sxs-lookup"><span data-stu-id="2fa02-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
