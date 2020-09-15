---
title: Problem s spoolerom pri ispisu je riješen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801833"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="165bb-102">Problem s spoolerom pri ispisu je riješen</span><span class="sxs-lookup"><span data-stu-id="165bb-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="165bb-103">Ako je vaš uređaj ažuriran sa sustavom Windows 10  **OS međuverzija 19041,329**, možda ste primijetili problem u kojem neki pisači ne mogu ispisati.</span><span class="sxs-lookup"><span data-stu-id="165bb-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="165bb-104">Usmjerivač ispisa mogao bi slučajno baciti pogrešku ili se neočekivano zatvarati prilikom pokušaja ispisa, a izlaz ne dolazi s izvještačenog pisača.</span><span class="sxs-lookup"><span data-stu-id="165bb-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="165bb-105">Taj je problem riješen u sustavu OS međuverzija  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="165bb-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="165bb-106">**Istraživanje u tijeku**</span><span class="sxs-lookup"><span data-stu-id="165bb-106">**Ongoing investigation**</span></span>

<span data-ttu-id="165bb-107">Datoteka lokalnog sigurnosnog autoriteta podsustava (LSASS) (**Isass.exe**) može pogriješiti na nekim uređajima s porukom o pogrešci "kritični Sistemski proces, C:\WINDOWS\system32\Isass.exe, nije uspio s kodom statusa c0000008.</span><span class="sxs-lookup"><span data-stu-id="165bb-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="165bb-108">Stroj se sada mora ponovno pokrenuti ".</span><span class="sxs-lookup"><span data-stu-id="165bb-108">The machine must now be restarted".</span></span>  <span data-ttu-id="165bb-109">**Microsoft radi na rezoluciji i osigurat će ažuriranje u predstojećem izdanju.**</span><span class="sxs-lookup"><span data-stu-id="165bb-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="165bb-110">Dodatne informacije potražite u odjeljku  [poznati problemi u sustavu Windows 10 verzije 2004](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="165bb-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>