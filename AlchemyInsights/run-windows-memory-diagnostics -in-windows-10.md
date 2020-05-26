---
title: Pokretanje dijagnostike memorije u sustavu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44357311"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="66548-102">Pokretanje dijagnostike memorije u sustavu Windows 10</span><span class="sxs-lookup"><span data-stu-id="66548-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="66548-103">Ako se Sustav Windows i aplikacije na PC-ju ruše, smrzavaju ili djeluju na nestabilan način, možda imate problema s memorijom PC-ja (RAM-om).</span><span class="sxs-lookup"><span data-stu-id="66548-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="66548-104">Možete pokrenuti dijagnostiku memorije sustava Windows da biste provjerili ima li problema s RAM-om PC-ja.</span><span class="sxs-lookup"><span data-stu-id="66548-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="66548-105">U okvir pretraživanja na programskoj traci upišite **dijagnostika memorije,** a zatim odaberite **Dijagnostika memorije sustava Windows**.</span><span class="sxs-lookup"><span data-stu-id="66548-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="66548-106">Da biste pokrenuli dijagnostiku, PC se mora ponovno pokrenuti.</span><span class="sxs-lookup"><span data-stu-id="66548-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="66548-107">Imate mogućnost odmah ponovno gimnastike (spremite svoj rad i zatvorite otvorene dokumente i e-mailove) ili zakažite automatsko pokretanje dijagnostike prilikom sljedećeg ponovnog pokretanja računala:</span><span class="sxs-lookup"><span data-stu-id="66548-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Dijagnostika memorije u sustavu Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="66548-109">Kada se PC ponovno pokrene, **dijagnostički alat za memoriju sustava Windows** automatski će se pokrenuti.</span><span class="sxs-lookup"><span data-stu-id="66548-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="66548-110">Status i napredak prikazat će se tijekom pokretanja dijagnostike, a imate mogućnost otkazivanja dijagnostike tako da pritisnete **tipku ESC** na tipkovnici.</span><span class="sxs-lookup"><span data-stu-id="66548-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="66548-111">Kada se dijagnostika dovrši, Windows će se normalno pokrenuti.</span><span class="sxs-lookup"><span data-stu-id="66548-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="66548-112">Odmah nakon ponovnog pokretanja, kada se pojavi radna površina, pojavit će se obavijest (pored ikone **Akcijskog centra** na programskoj traci) da biste naznačili jesu li pronađene pogreške u memoriji.</span><span class="sxs-lookup"><span data-stu-id="66548-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="66548-113">Na primjer:</span><span class="sxs-lookup"><span data-stu-id="66548-113">For example:</span></span>

<span data-ttu-id="66548-114">Evo ikone akcijskog centra:</span><span class="sxs-lookup"><span data-stu-id="66548-114">Here's the Action Center icon:</span></span> ![Ikona akcijskog centra](media/action-center-icon.png) 

<span data-ttu-id="66548-116">I oglednu obavijest:</span><span class="sxs-lookup"><span data-stu-id="66548-116">And a sample notification:</span></span> ![Nema pogrešaka u memoriji](media/no-memory-errors.png)

<span data-ttu-id="66548-118">Ako ste propustili obavijest, možete odabrati ikonu **Akcijskog centra** na programskoj traci za prikaz **akcijskog centra** i prikaz popisa obavijesti koji se može pomicati.</span><span class="sxs-lookup"><span data-stu-id="66548-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="66548-119">Da biste pregledali detaljne informacije, u okvir za pretraživanje na programskoj traci upišite **događaj,** a zatim odaberite **Preglednik događaja**.</span><span class="sxs-lookup"><span data-stu-id="66548-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="66548-120">U lijevom oknu **preglednika događaja**idite na **Windows Logs > System**.</span><span class="sxs-lookup"><span data-stu-id="66548-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="66548-121">U desnom oknu skenirajte popis dok gledate stupac **Izvor** dok ne vidite događaje s izvornom vrijednošću **MemoryDiagnostics-Results**.</span><span class="sxs-lookup"><span data-stu-id="66548-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="66548-122">Označite svaki takav događaj i pogledajte informacije o rezultatima u okviru na kartici **Općenito** ispod popisa.</span><span class="sxs-lookup"><span data-stu-id="66548-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
