---
title: Problem s usmjerivačem ispisa riješen je
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088287"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="a432f-102">Problem s usmjerivačem ispisa riješen je</span><span class="sxs-lookup"><span data-stu-id="a432f-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="a432f-103">Ako je vaš uređaj ažuriran pomoću značajke Windows **10 OS Build 19041.329**, možda ste primijetili problem zbog kojeg se određeni pisači ne ispisuju.</span><span class="sxs-lookup"><span data-stu-id="a432f-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="a432f-104">Usmjerivač ispisa može baciti pogrešku ili se neočekivano zatvoriti prilikom pokušaja ispisa, a izlaz ne dolazi s zahvaćenog pisača.</span><span class="sxs-lookup"><span data-stu-id="a432f-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="a432f-105">Ovaj je problem riješen u međuverziji **OS-a 19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="a432f-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="a432f-106">**Istraga koja je u tijeku**</span><span class="sxs-lookup"><span data-stu-id="a432f-106">**Ongoing investigation**</span></span>

<span data-ttu-id="a432f-107">Datoteka servisa podsustava lokalne sigurnosne ovlasti (LSASS)\*\* (Isass.exe\*\*) možda neće uspjeti na nekim uređajima s porukom o pogrešci "Kritični sistemski proces, C:\WINDOWS\system32\Isass.exe, nije uspio s kodom stanja c0000008.</span><span class="sxs-lookup"><span data-stu-id="a432f-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="a432f-108">Aparat se sada mora ponovno pokrenuti".</span><span class="sxs-lookup"><span data-stu-id="a432f-108">The machine must now be restarted".</span></span>  <span data-ttu-id="a432f-109">**Microsoft radi na rješenju i pružit će ažuriranje u nadolazećem izdanju.**</span><span class="sxs-lookup"><span data-stu-id="a432f-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="a432f-110">Dodatne informacije potražite u [poznatim problemima verzije 2004 sustava Windows 10](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="a432f-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>