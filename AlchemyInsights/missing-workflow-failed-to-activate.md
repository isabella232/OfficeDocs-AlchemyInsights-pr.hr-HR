---
title: Nije uspjelo aktiviranje tijeka rada koji nedostaje
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: d703e87f355f05bf4a1d71e5daddce96db988380bb48accc81c95f1ba91fbb2b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065420"
---
# <a name="missing-workflow-failed-to-activate"></a>Nije uspjelo aktiviranje tijeka rada koji nedostaje

U microsoftovoj zbirci SharePoint web-mjesta ne možete dodati globalni tijek rada koji se može ponovno koristiti (npr. "Odobrenje – SharePoint 2010") na popis ili u biblioteku.
  
Da biste riješili taj problem, slijedite ove korake: 
  
1. Otvorite korijensko web-mjesto zbirke web-mjesta u programu SharePoint Designer 2013.
  
2. U **odjeljku Objekti web-mjesta** **odaberite Tijekovi rada**. 
  
3. U **odjeljku Novo** na **vrpci Tijekovi** rada odaberite Tijek rada **koji se može ponovno koristiti**. 
  
4. Na obrascu **Stvaranje tijeka rada koji se može ponovno** koristiti unesite naziv ** *Repair2010* **. Za **vrstu platforme kliknite** SharePoint tijek rada **2010**, a zatim U **redu**. 
  
1. U **odjeljku Spremanje** na vrpci **Tijek rada** odaberite **Objavi**. 
  
2. U **odjeljku Upravljanje** na vrpci **Tijek rada** odaberite **Objavi globalno**. U dijaloškom okviru za potvrdu koji će se prikazati odaberite **U redu**. 
  
3. U web-pregledniku pronađite korijensko web-mjesto zbirke web-mjesta, a zatim pristupite **značajkama zbirke Postavke** \> **web-mjesta**. Zatim prebacite značajku **tijekova** rada: 
  
· Ako je značajka  *aktivirana*  , kliknite **Deaktiviraj,** a zatim **Aktiviraj**. 
  
· Ako je značajka  *deaktivirana*  , kliknite **Aktiviraj**. 
  
Dodatne informacije potražite u sljedećem [članku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

