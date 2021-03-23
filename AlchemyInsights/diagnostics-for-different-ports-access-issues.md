---
title: Dijagnostika za druge probleme s pristupom lukama
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035004"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="a9108-102">Dijagnostika za druge probleme s pristupom lukama</span><span class="sxs-lookup"><span data-stu-id="a9108-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="a9108-103">Da biste riješili razne probleme s pristupom priključkom, slijedite sljedeće korake:</span><span class="sxs-lookup"><span data-stu-id="a9108-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="a9108-104">Stop/dealpronađite virtualni stroj (VM) s portala, ponovno pokrenite VM, a zatim ponovno testirajte.</span><span class="sxs-lookup"><span data-stu-id="a9108-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="a9108-105">Provjerite imate li mrežne postavke za VM da biste utvrdili imate li mrežne sigurnosne grupe (NSGs) koji blokiraju promet.</span><span class="sxs-lookup"><span data-stu-id="a9108-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="a9108-106">Možete koristiti i [alat za provjeru IP toka programa Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) da biste provjerili je li nsgs blokirao promet, User-Defined rute (UDRs) preusmjeravaju promet natrag na lokalno ("zadana ruta",, a) ili na mrežni uređaj.</span><span class="sxs-lookup"><span data-stu-id="a9108-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="a9108-107">Ako i dalje naiđete na probleme nakon pokušaja navedenih koraka, navedite VM naziv i TCP priključak na kojem pokušavate slati poštu radi daljnje dijagnoze.</span><span class="sxs-lookup"><span data-stu-id="a9108-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="a9108-108">**Preporučeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="a9108-108">**Recommended Documents**</span></span>

[<span data-ttu-id="a9108-109">Ograničenja i preporuke za slanje odlaznih poruka e-pošte putem priključka 25</span><span class="sxs-lookup"><span data-stu-id="a9108-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)