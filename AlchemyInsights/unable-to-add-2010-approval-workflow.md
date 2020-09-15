---
title: Tijek rada za odobrenje 2010 nije moguće dodati
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699727"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Tijek rada za odobrenje 2010 nije moguće dodati

U zbirci web-mjesta sustava Microsoft SharePoint ne možete dodati globalni tijek rada za ponovno korištenje (kao što je "odobrenje-SharePoint 2010") na popis ili u biblioteku.
  
Da biste riješili taj problem, slijedite ove korake: 
  
1. Otvorite korijensko web-mjesto zbirke web-mjesta u sustavu SharePoint Designer 2013.
  
2. U odjeljku **objekti web-mjesta**odaberite **Tijekovi rada**. 
  
3. U **novom** odjeljku vrpce **tijekova rada** odaberite **Ponovno iskoristiv tijek rada**. 
  
4. Na obrascu **Stvaranje ponovno iskoristivog tijeka rada** unesite naziv * * *Repair2010* * *. Za **vrstu platforme**kliknite **tijek rada sustava SharePoint 2010**, a zatim kliknite **u redu**. 
  
1. U odjeljku **Spremanje** na vrpci **tijeka rada** odaberite **Objavi**. 
  
2. U odjeljku **Upravljanje** na vrpci **tijeka rada** odaberite **Objavi globalno**. U dijaloškom okviru za potvrdu koji će se prikazati odaberite **u redu**. 
  
3. U web-pregledniku Pronađite korijensko web-mjesto zbirke web-mjesta, a zatim **Site Settings** \> **značajke zbirke web-mjesta**za postavljanje web-mjesta. Uključivanje/isključivanje značajke **tijekova rada** : 
  
· Ako je značajka  *aktivirana*  , kliknite **Deaktiviraj,** a zatim **Aktiviraj**. 
  
· Ako je značajka  *deaktivirana*  , kliknite **Aktiviraj**. 
  
Dodatne informacije potražite u sljedećem [članku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

