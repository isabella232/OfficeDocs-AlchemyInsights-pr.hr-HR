---
title: Nije moguće dodati zadani tijek rada za odobrenje 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28279578"
---
# <a name="cant-add-default-2010-approval-workflow"></a>Nije moguće dodati zadani tijek rada za odobrenje 2010

U zbirke web-mjesta Microsoft SharePoint globalno ponovno iskoristiv tijek rada (na primjer "odobrenje - SharePoint 2010") ne može dodati na popis ili biblioteku.
  
Da biste riješili taj problem, slijedite ove korake: 
  
1. Otvorite web-mjesto korijena zbirke web-mjesta SharePoint Designer 2013.
  
2. Pod **Objekti web-mjesta**odaberite **tijekova rada**. 
  
3. U sekciji **Novo** vrpce **tijekove rada** , odaberite **Tijek rada za ponovno iskoristiv**. 
  
4. **Stvaranje tijeka rada ponovno iskoristiv** obrascu unesite naziv * **Repair2010***. Za **Vrstu Platform**odaberite **Tijeka rada sustava SharePoint 2010**, a zatim odaberite **u redu**. 
  
5. U odjeljak **spremiti** vrpce **tijeka rada** odaberite **Objavi**. 
  
6. U odjeljku **Upravljanje** vrpce **tijeka rada** , odaberite **Objaviti globalno**. U dijaloškom okviru potvrda koja se pojavljuje odaberite **u redu**. 
  
7. U web-pregledniku, pronađite na web-mjestu korijena zbirke web-mjesta i pristup **Postavkama web-mjesta** \> **Značajke zbirke web-mjesta**. Zatim, Preklopi značajka **tijekova rada** : 
  
· Značajka je *aktivirano* , kliknite **Deaktiviraj,** a zatim kliknite **Aktiviraj**. 
  
· Značajka je *Deactivated* , kliknite **Aktiviraj**. 
  
Za dodatne informacije pogledajte sljedeći [članak](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

