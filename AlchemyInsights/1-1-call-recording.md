---
title: Snimanje poziva 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696914"
---
# <a name="11-call-recording"></a><span data-ttu-id="13d56-102">Snimanje poziva 1:1</span><span class="sxs-lookup"><span data-stu-id="13d56-102">1:1 call recording</span></span>

<span data-ttu-id="13d56-103">Ako je **gumb Pokreni** snimanje zasivljen u pozivu u 1:1, morate promijeniti postavke pravilnika za utjecajnog korisnika.</span><span class="sxs-lookup"><span data-stu-id="13d56-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="13d56-104">Počevši od 31. svibnja 2021., započinjemo s novim pravilnikom Teams *pozivanja AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="13d56-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="13d56-105">Prije te promjene snimanje poziva 1:1 kontrolira *AllowCloudRecording Teams* sastanaka.</span><span class="sxs-lookup"><span data-stu-id="13d56-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="13d56-106">Ta je promjena dokumentirana u objavi Centra za poruke: [(Ažurirano) 1:1 Uvod pravilnika za snimanje poziva](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span><span class="sxs-lookup"><span data-stu-id="13d56-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="13d56-107">*AllowCloudRecordingForCalls*   Mogućnost pravilnika pozivanja postavljena **je na $False po** zadanom.</span><span class="sxs-lookup"><span data-stu-id="13d56-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="13d56-108">Ako želite svim korisnicima blokirati snimanje poziva u 1:1, ne morate ništa poduzeti.</span><span class="sxs-lookup"><span data-stu-id="13d56-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="13d56-109">Da biste omogućili snimanje poziva za sve korisnike u 1:1 pozivima, Teams PowerShell za pokretanje sljedećeg cmdleta:</span><span class="sxs-lookup"><span data-stu-id="13d56-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="13d56-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="13d56-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="13d56-111">Možete i stvoriti novi pravilnik i postaviti **-AllowCloudRecordingForCalls** **tako da $true** i dodijeliti taj pravilnik korisnicima.</span><span class="sxs-lookup"><span data-stu-id="13d56-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="13d56-112">Dodatne informacije potražite u članku Kontrole pravila snimanja poziva [1:1 Jesu (gotovo!) Ovdje .](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)</span><span class="sxs-lookup"><span data-stu-id="13d56-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
