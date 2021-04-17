---
title: Pokretanje dijagnostike memorije sustava Windows u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826659"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="2c849-102">Pokretanje dijagnostike memorije sustava Windows u sustavu Windows 10</span><span class="sxs-lookup"><span data-stu-id="2c849-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="2c849-103">Ako se Windows i aplikacije na PC-ju rušiju, smrzavaju ili djeluju na nestabilan način, možda imate problema s memorijom PC-ja (RAM-om).</span><span class="sxs-lookup"><span data-stu-id="2c849-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="2c849-104">Da biste provjerili ima li problema s RAM-om PC-ja, pokrenite dijagnostiku memorije sustava Windows.</span><span class="sxs-lookup"><span data-stu-id="2c849-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="2c849-105">U okvir za pretraživanje na programskoj traci upišite **dijagnostika** memorije , a zatim odaberite **Dijagnostika memorije u sustavu Windows**.</span><span class="sxs-lookup"><span data-stu-id="2c849-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="2c849-106">Da biste pokrenuli dijagnostiku, PC se mora ponovno pokrenuti.</span><span class="sxs-lookup"><span data-stu-id="2c849-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="2c849-107">Imate mogućnost da se odmah ponovno pokrenete (spremite svoje radne dokumente i najprije zatvorite otvorene dokumente i poruke e-pošte) ili zakažete automatsko pokretanje dijagnostike prilikom sljedećeg ponovnog pokretanja PC-ja:</span><span class="sxs-lookup"><span data-stu-id="2c849-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Dijagnostika memorije u sustavu Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="2c849-109">Kada se PC ponovno pokrene, automatski će se pokrenuti alat za **dijagnostiku memorije** u sustavu Windows.</span><span class="sxs-lookup"><span data-stu-id="2c849-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="2c849-110">Status i napredak prikazat će se kao pokretanje dijagnostike, a možete otkazati dijagnostiku tako da na tipkovnici ujete **tipku ESC.**</span><span class="sxs-lookup"><span data-stu-id="2c849-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="2c849-111">Kada se dijagnostika dovrši, Windows će se normalno pokrenuti.</span><span class="sxs-lookup"><span data-stu-id="2c849-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="2c849-112">Odmah nakon ponovnog pokretanja, kada se pojavi radna površina, pojavit će se obavijest (pokraj ikone **Akcijskog** centra na programskoj traci) da bi se naznačilo jesu li pronađene pogreške u memoriji.</span><span class="sxs-lookup"><span data-stu-id="2c849-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="2c849-113">Na primjer:</span><span class="sxs-lookup"><span data-stu-id="2c849-113">For example:</span></span>

<span data-ttu-id="2c849-114">Evo ikone Akcijskog centra:</span><span class="sxs-lookup"><span data-stu-id="2c849-114">Here's the Action Center icon:</span></span> ![Ikona akcijskog centra](media/action-center-icon.png) 

<span data-ttu-id="2c849-116">I ogledna obavijest:</span><span class="sxs-lookup"><span data-stu-id="2c849-116">And a sample notification:</span></span> ![Nema pogrešaka u memoriji](media/no-memory-errors.png)

<span data-ttu-id="2c849-118">Ako ste propustili obavijest, možete odabrati ikonu **Akcijskog** centra na programskoj traci da biste prikazali **akcijski** centar i vidjeli popis obavijesti koji se može pomicati.</span><span class="sxs-lookup"><span data-stu-id="2c849-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="2c849-119">Da biste pregledali detaljne informacije, **upišite** događaj u okvir za pretraživanje na programskoj traci, a zatim **odaberite Preglednik događaja**.</span><span class="sxs-lookup"><span data-stu-id="2c849-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="2c849-120">U lijevom **oknu preglednika** događaja otvorite zapisnike sustava **Windows > System**.</span><span class="sxs-lookup"><span data-stu-id="2c849-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="2c849-121">U desnom oknu pregledajte popis dok pregledavate stupac **Izvor** dok ne vidite događaje s izvorišnom vrijednošću **MemoryDiagnostics-Results**.</span><span class="sxs-lookup"><span data-stu-id="2c849-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="2c849-122">Isticanje svakog takvog događaja i prikaz informacija o rezultatima u okviru ispod **kartice** Općenito ispod popisa.</span><span class="sxs-lookup"><span data-stu-id="2c849-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
