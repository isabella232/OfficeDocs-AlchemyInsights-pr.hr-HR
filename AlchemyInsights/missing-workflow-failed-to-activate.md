---
title: Aktivacija tijeka rada koji nedostaje nije uspio
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762093"
---
# <a name="missing-workflow-failed-to-activate"></a>Aktivacija tijeka rada koji nedostaje nije uspio

U zbirci web-mjesta sustava Microsoft SharePoint ne možete dodati globalno ponovno upotrebljiv tijek rada (kao što je "Odobrenje - SharePoint 2010") na popis ili biblioteku.
  
Da biste riješili taj problem, slijedite ove korake: 
  
1. Otvorite korijensko web-mjesto zbirke web-mjesta u programu SharePoint Designer 2013.
  
2. U **odjeljku Objekti web-mjesta**odaberite **Tijekovi rada**. 
  
3. U odjeljku **Novo** na **vrpci Tijekovi rada** odaberite **Ponovno upotrebljivtijek rada**. 
  
4. Na obrascu **Stvaranje ponovno upotrebljivog tijeka rada** unesite naziv ** *Repair2010* **. Za **vrstu platforme**kliknite Tijek rada sustava **SharePoint 2010**, a zatim U **redu**. 
  
1. U odjeljku **Spremi** na vrpci **tijeka rada** odaberite **Objavi**. 
  
2. U odjeljku **Upravljanje** na vrpci **Tijek rada** odaberite **Objavi globalno**. U dijaloškom okviru za potvrdu koji će se pojaviti odaberite **U redu**. 
  
3. U web-pregledniku pronađite korijensko web-mjesto zbirke web-mjesta, a zatim **pristupite značajkama** \> **zbirke web-mjesta**. Zatim uključite značajku **Tijekovi rada:** 
  
· Ako je značajka *aktivirana,* kliknite **Deaktiviraj,** a zatim **Aktiviraj**. 
  
· Ako je značajka *deaktivirana,* kliknite **Aktiviraj**. 
  
Dodatne informacije potražite u sljedećem [članku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

