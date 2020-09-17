---
title: Dvoklikom na datoteku sustava Office ne otvara se
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812071"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="ecce6-102">Dvoklikom na datoteku sustava Office ne otvara se</span><span class="sxs-lookup"><span data-stu-id="ecce6-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="ecce6-103">Nakon dvoklika na datoteku sustava Office možda će se program otvoriti, ali se sama datoteka ne otvara.</span><span class="sxs-lookup"><span data-stu-id="ecce6-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="ecce6-104">Ili vam se prikazuje pogreška: "došlo je do problema prilikom slanja naredbe u program."</span><span class="sxs-lookup"><span data-stu-id="ecce6-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="ecce6-105">Postoje mnogi razlozi za to, no dva najčešća rješenja:</span><span class="sxs-lookup"><span data-stu-id="ecce6-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="ecce6-106">U programu Excel provjerite je li mogućnost DDE nepotvrđena.</span><span class="sxs-lookup"><span data-stu-id="ecce6-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="ecce6-107">Mogućnost se može pronaći stvaranjem nove radne knjige, a zatim odabirom **mogućnosti datoteka > > Napredno**.</span><span class="sxs-lookup"><span data-stu-id="ecce6-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="ecce6-108">U odjeljku **Općenito** poništite okvir **Zanemari druge aplikacije koje koriste dinamičku razmjenu podataka (DDE)**.</span><span class="sxs-lookup"><span data-stu-id="ecce6-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="ecce6-109">Pokrenite mrežni popravak da biste vratili zadane postavke.</span><span class="sxs-lookup"><span data-stu-id="ecce6-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="ecce6-110">Kliknite gumb Start sustava Windows i potražite "Upravljačka ploča".</span><span class="sxs-lookup"><span data-stu-id="ecce6-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="ecce6-111">Otvorite **upravljačku ploču**, a zatim idite na **programe > programe i značajke**.</span><span class="sxs-lookup"><span data-stu-id="ecce6-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="ecce6-112">Zatim desnom tipkom miša kliknite **Microsoft Office [verzija]** pa odaberite **Promijeni > online Repair (popravak**).</span><span class="sxs-lookup"><span data-stu-id="ecce6-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="ecce6-113">Ako nijedna od tih rješenja ne funkcionira, u članku podrške možete pronaći potpuniji popis rješenja, [dvoklikom na datoteku sustava Office ne možete je otvoriti](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span><span class="sxs-lookup"><span data-stu-id="ecce6-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
