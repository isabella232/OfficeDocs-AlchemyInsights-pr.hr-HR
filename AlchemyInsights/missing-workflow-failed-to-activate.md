---
title: Nije uspjelo Aktiviranje tijeka rada koji nema
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667078"
---
# <a name="missing-workflow-failed-to-activate"></a>Nije uspjelo Aktiviranje tijeka rada koji nema

U zbirci web-mjesta sustava Microsoft SharePoint ne možete dodati globalni tijek rada za ponovno korištenje (kao što je "odobrenje-SharePoint 2010") na popis ili u biblioteku.
  
Da biste riješili taj problem, slijedite ove korake: 
  
1. Otvorite korijensko web-mjesto zbirke web-mjesta u sustavu SharePoint Designer 2013.
  
2. U odjeljku **objekti web-mjesta**odaberite **Tijekovi rada**. 
  
3. U **novom** odjeljku vrpce **tijekova rada** odaberite **Ponovno iskoristiv tijek rada**. 
  
4. Na obrascu **Stvaranje ponovno iskoristivog tijeka rada** unesite naziv * * *Repair2010* * *. Za **vrstu platforme**kliknite **tijek rada sustava SharePoint 2010**, a zatim kliknite **u redu**. 
  
1. U odjeljku **Spremanje** na vrpci **tijeka rada** odaberite **Objavi**. 
  
2. U odjeljku **Upravljanje** na vrpci **tijeka rada** odaberite **Objavi globalno**. U dijaloškom okviru za potvrdu koji će se prikazati odaberite **u redu**. 
  
3. U web-pregledniku Pronađite korijensko web-mjesto zbirke web-mjesta, a zatim **Site Settings** \> **značajke zbirke web-mjesta**za postavljanje web-mjesta. Zatim preklopni značajku **tijekova rada** : 
  
· Ako je značajka  *aktivirana*  , kliknite **Deaktiviraj,** a zatim **Aktiviraj**. 
  
· Ako je značajka  *deaktivirana*  , kliknite **Aktiviraj**. 
  
Dodatne informacije potražite u sljedećem [članku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

