---
title: Pokretanje dijagnostike memorije u sustavu Windows u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: f2b8306d0cd604b144b82275243c5a84580bc609
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720782"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="54bd8-102">Pokretanje dijagnostike memorije u sustavu Windows u sustavu Windows 10</span><span class="sxs-lookup"><span data-stu-id="54bd8-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="54bd8-103">Ako se prozori i aplikacije na PC-ju raspada, zamrzavaju ili djeluju na nestabilan način, možda ćete imati problema s memorijom (RAM-om) PC-ja.</span><span class="sxs-lookup"><span data-stu-id="54bd8-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="54bd8-104">Možete pokrenuti dijagnostiku memorije sustava Windows da biste provjerili ima li problema s RAM-om PC-ja.</span><span class="sxs-lookup"><span data-stu-id="54bd8-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="54bd8-105">U okvir za pretraživanje na programskoj traci upišite **Dijagnostika memorije**, a zatim odaberite **Dijagnostika memorije u sustavu Windows**.</span><span class="sxs-lookup"><span data-stu-id="54bd8-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="54bd8-106">Da biste pokrenuli dijagnostiku, potrebno je ponovno pokrenuti PC.</span><span class="sxs-lookup"><span data-stu-id="54bd8-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="54bd8-107">Imate mogućnost odmah ponovno pokrenuti (spremite svoj rad i zatvorite otvorene dokumente i e-poštu) ili zakazivanje automatskog pokretanja PC-ja prilikom sljedećeg ponovnog pokretanja računala:</span><span class="sxs-lookup"><span data-stu-id="54bd8-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Dijagnostika memorije u sustavu Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="54bd8-109">Kada se PC ponovno pokrene, **alat za dijagnostiku memorije u sustavu Windows** pokrenut će se automatski.</span><span class="sxs-lookup"><span data-stu-id="54bd8-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="54bd8-110">Status i tijek prikazat će se kao dijagnostički pokrenuti, a možete i poništiti dijagnostiku tako da kliknete tipku **Esc** na tipkovnici.</span><span class="sxs-lookup"><span data-stu-id="54bd8-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="54bd8-111">Kada se dijagnostika dovrši, Windows će se normalno pokrenuti.</span><span class="sxs-lookup"><span data-stu-id="54bd8-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="54bd8-112">Odmah nakon ponovnog pokretanja, kada se pojavi radna površina, prikazat će se obavijest (uz ikonu **akcijskog centra** na programskoj traci) da biste naznačili jesu li pronađene pogreške u memoriji.</span><span class="sxs-lookup"><span data-stu-id="54bd8-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="54bd8-113">Na primjer:</span><span class="sxs-lookup"><span data-stu-id="54bd8-113">For example:</span></span>

<span data-ttu-id="54bd8-114">Evo ikone akcijskog centra:</span><span class="sxs-lookup"><span data-stu-id="54bd8-114">Here's the Action Center icon:</span></span> ![Ikona akcijskog centra](media/action-center-icon.png) 

<span data-ttu-id="54bd8-116">I oglednu obavijest:</span><span class="sxs-lookup"><span data-stu-id="54bd8-116">And a sample notification:</span></span> ![Nema pogrešaka u memoriji](media/no-memory-errors.png)

<span data-ttu-id="54bd8-118">Ako ste propušteni obavijest, možete odabrati ikonu **akcijskog centra** na programskoj traci da biste prikazali **akcijski centar** i pogledali popis obavijesti koji se mogu kretati.</span><span class="sxs-lookup"><span data-stu-id="54bd8-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="54bd8-119">Da biste pregledali detaljne informacije, upišite **Event** u okvir za pretraživanje na programskoj traci, a zatim odaberite **preglednik događaja**.</span><span class="sxs-lookup"><span data-stu-id="54bd8-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="54bd8-120">U lijevom oknu **preglednika događaja**dođite do **zapisnika > sustava Windows**.</span><span class="sxs-lookup"><span data-stu-id="54bd8-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="54bd8-121">U desnom oknu Skenirajte popis dok pogledate **izvorni** stupac dok ne vidite događaje s **memorijalnom dijagnostom**izvorne vrijednosti (rezultati).</span><span class="sxs-lookup"><span data-stu-id="54bd8-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="54bd8-122">Istaknite svaki takav događaj i pogledajte informacije o rezultatu u okviru na kartici **Općenito** ispod popisa.</span><span class="sxs-lookup"><span data-stu-id="54bd8-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
