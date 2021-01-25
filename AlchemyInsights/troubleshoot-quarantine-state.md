---
title: Otklanjanje poteškoća s karantenom
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7853"
- "9004348"
ms.openlocfilehash: 3ee932b7788f4aff3c8bc762c5c917124edfe065
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949669"
---
# <a name="troubleshoot-quarantine-state"></a><span data-ttu-id="31ea0-102">Otklanjanje poteškoća s karantenom</span><span class="sxs-lookup"><span data-stu-id="31ea0-102">Troubleshoot quarantine state</span></span>

<span data-ttu-id="31ea0-103">Servis za dodjelu resursa za Azure Active Directory (AD) nadzire stanje vaše konfiguracije.</span><span class="sxs-lookup"><span data-stu-id="31ea0-103">The Azure Active Directory (AD) provisioning service monitors the health of your configuration.</span></span> <span data-ttu-id="31ea0-104">Ona također smješta nezdrave aplikacije u stanje **karantene** .</span><span class="sxs-lookup"><span data-stu-id="31ea0-104">It also places unhealthy apps in a **quarantine** state.</span></span> <span data-ttu-id="31ea0-105">Ako se većina ili svi pozivi koji se odnose na ciljni sustav dosljedno ne uspiju, zadatak dodjele resursa označit će se kao **u karanteni**.</span><span class="sxs-lookup"><span data-stu-id="31ea0-105">If most, or all, of the calls made against the target system consistently fail, then the provisioning job is marked as **in quarantine**.</span></span> <span data-ttu-id="31ea0-106">Primjer **pogreške je pogreška primljenih zbog nevaljanih administratorskih vjerodajnica**.</span><span class="sxs-lookup"><span data-stu-id="31ea0-106">An example of a failure is **an error received because of invalid admin credentials**.</span></span> <span data-ttu-id="31ea0-107">Dodatne informacije potražite u članku [Dodjela resursa aplikacijama u stanju karantene](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-quarantine-status).</span><span class="sxs-lookup"><span data-stu-id="31ea0-107">For more information, see [Application provisioning in quarantine status](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-quarantine-status).</span></span>

<span data-ttu-id="31ea0-108">Da biste otklonili poteškoće s sinkronizacijom u oblaku, pročitajte odjeljak [dodjeljivanje problema u karanteni](https://docs.microsoft.com/azure/active-directory/cloud-sync/how-to-troubleshoot#provisioning-quarantined-problems).</span><span class="sxs-lookup"><span data-stu-id="31ea0-108">To troubleshoot cloud sync, see [Provisioning quarantined problems](https://docs.microsoft.com/azure/active-directory/cloud-sync/how-to-troubleshoot#provisioning-quarantined-problems).</span></span> 
