---
title: Nestanak tijeka rada nije uspio aktivirati
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 3df1ddc1059c4cd6cc3f9f42dc157d20be79a63a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052605"
---
# <a name="missing-workflow-failed-to-activate"></a>Nestanak tijeka rada nije uspio aktivirati

U zbirci web-mjesta programa Microsoft SharePoint ne možete dodati globalni tijek rada koji se može ponovno koristiti (kao što je "odobrenje-SharePoint 2010") na popis ili biblioteku.
  
Da biste riješili taj problem, slijedite ove korake: 
  
1. Otvorite korijensku web-lokaciju zbirke web-mjesta u programu SharePoint Designer 2013.
  
2. U odjeljku **objekti web-mjesta**odaberite **tijekove rada**. 
  
3. U **novom** odjeljku vrpce **Tijekovi rada** odaberite **Ponovno iskoristiv tijek rada**. 
  
4. **Da biste** unijeli naziv * * *Repair2010* * *. Za **vrstu platforme**kliknite **SharePoint 2010 Workflow**, a zatim kliknite **u redu**. 
  
1. U odjeljku **Spremi** na vrpci **tijeka rada** odaberite **Objavi**. 
  
2. U odjeljku **Upravljanje** vrpcom **tijeka rada** odaberite **Objavi globalno**. U potvrdnom dijaloškom okviru koji se pojavi odaberite **u redu**. 
  
3. U web-pregledniku Pronađite korijensku web-lokaciju zbirke web-mjesta, a zatim pristupite **značajkama zbirke web**-mjesta za **postavku** \> web-mjesta. Zatim uključite značajku **tijekova rada** : 
  
· Ako je značajka *aktivirana* , kliknite " **Deaktiviraj",** a zatim kliknite " **Aktiviraj**". 
  
· Ako je značajka *deaktivirana* , kliknite **Aktiviraj**. 
  
Dodatne informacije potražite u sljedećem [članku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

