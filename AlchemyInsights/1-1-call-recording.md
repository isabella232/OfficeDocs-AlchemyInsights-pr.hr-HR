---
title: 1:1 poziva na snimanje
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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733841"
---
# <a name="11-call-recording"></a><span data-ttu-id="32e52-102">1:1 poziva na snimanje</span><span class="sxs-lookup"><span data-stu-id="32e52-102">1:1 call recording</span></span>

<span data-ttu-id="32e52-103">Administratori sada moraju poduzeti akciju da bi korisnicima omogućili snimanje 1:1 poziva.</span><span class="sxs-lookup"><span data-stu-id="32e52-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="32e52-104">Počevši od travnja 12, 2021, počet ćemo provoditi nove grupe za pozivanje pravilnika *Allowclouderecordingforpoziv*.</span><span class="sxs-lookup"><span data-stu-id="32e52-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="32e52-105">Trenutno 1:1 mogućnosti snimanja poziva kontroliraju se pomoću mogućnosti *Allowcloudesnimanje* u pravilima sastanka timova.</span><span class="sxs-lookup"><span data-stu-id="32e52-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="32e52-106">Ako je korisnicima dopušteno snimati sastanke timova, možete snimati i 1:1 poziva.</span><span class="sxs-lookup"><span data-stu-id="32e52-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="32e52-107">Ako želite onemogućiti svim korisnicima snimanje 1:1 poziva, ne morate poduzeti nikakve akcije.</span><span class="sxs-lookup"><span data-stu-id="32e52-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="32e52-108">Mogućnost *Allowclouderecordingforza* pozivanje pravilnika bit će $FALSE po zadanom.</span><span class="sxs-lookup"><span data-stu-id="32e52-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="32e52-109">Ta je promjena dokumentirana u sljedećoj pošti u centru za poruke: [(obnovljeno) 1:1 Pozivanje pravilnika za snimanje poziva](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) da biste postavili mogućnost pravilnika za timove koje morate koristiti u [timovima PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="32e52-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="32e52-110">**Da biste omogućili snimanje poziva u programu 1:1 pozivi:** Set-CsTeamsCallingPolicy-Identity Global-Allowcloud Recordingforpoziv $True</span><span class="sxs-lookup"><span data-stu-id="32e52-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="32e52-111">**Da biste onemogućili snimanje poziva u programu 1:1 pozivi:** Set-CsTeamsCallingPolicy-Identity Global-Allowcloud Recordingforpoziv $FALSE</span><span class="sxs-lookup"><span data-stu-id="32e52-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

