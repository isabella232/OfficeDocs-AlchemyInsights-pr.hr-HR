---
title: Nije moguće dodati tijek rada za odobrenje 2010
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: e74c842f8b4be321664f8c2f1f58c570d0724d80edb1264add0647bf313bc82f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020328"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Nije moguće dodati tijek rada za odobrenje 2010

U microsoftovoj zbirci SharePoint web-mjesta ne možete dodati globalni tijek rada koji se može ponovno koristiti (npr. "Odobrenje – SharePoint 2010") na popis ili u biblioteku.
  
Da biste riješili taj problem, slijedite ove korake: 
  
1. Otvorite korijensko web-mjesto zbirke web-mjesta u programu SharePoint Designer 2013.
  
2. U **odjeljku Objekti web-mjesta** **odaberite Tijekovi rada**. 
  
3. U **odjeljku Novo** na **vrpci Tijekovi** rada odaberite Tijek rada **koji se može ponovno koristiti**. 
  
4. Na obrascu **Stvaranje tijeka rada koji se može ponovno** koristiti unesite naziv ** *Repair2010* **. Za **vrstu platforme kliknite** SharePoint tijek rada **2010**, a zatim U **redu**. 
  
1. U **odjeljku Spremanje** na vrpci **Tijek rada** odaberite **Objavi**. 
  
2. U **odjeljku Upravljanje** na vrpci **Tijek rada** odaberite **Objavi globalno**. U dijaloškom okviru za potvrdu koji će se prikazati odaberite **U redu**. 
  
3. U web-pregledniku pronađite korijensko web-mjesto zbirke web-mjesta, a zatim pristupite **značajkama zbirke Postavke** \> **web-mjesta**. Uključivanje i isključivanje značajke **tijekova** rada: 
  
· Ako je značajka  *aktivirana*  , kliknite **Deaktiviraj,** a zatim **Aktiviraj**. 
  
· Ako je značajka  *deaktivirana*  , kliknite **Aktiviraj**. 
  
Dodatne informacije potražite u sljedećem [članku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

