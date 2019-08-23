---
title: Nije moguće dodati tijek rada za odobrenje 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 1f564c5d1e689dcf41b22fab5a05ab1b488c2b0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558609"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Nije moguće dodati tijek rada za odobrenje 2010

U zbirke web-mjesta Microsoft SharePoint globalno ponovno iskoristiv tijek rada (na primjer "odobrenje - SharePoint 2010") ne može dodati na popis ili biblioteku.
  
Da biste riješili taj problem, slijedite ove korake: 
  
1. Otvorite web-mjesto korijena zbirke web-mjesta SharePoint Designer 2013.
  
2. Pod **Objekti web-mjesta**odaberite **tijekova rada**. 
  
3. U sekciji **Novo** vrpce **tijekove rada** , odaberite **Tijek rada za ponovno iskoristiv**. 
  
4. **Stvaranje tijeka rada ponovno iskoristiv** obrascu unesite naziv ** *Repair2010* **. Za **Vrstu Platform**kliknite **Tijeka rada sustava SharePoint 2010**, a zatim kliknite **u redu**. 
  
1. U odjeljak **spremiti** vrpce **tijeka rada** odaberite **Objavi**. 
  
2. U odjeljku **Upravljanje** vrpce **tijeka rada** , odaberite **Objaviti globalno**. U dijaloškom okviru potvrda koja se pojavljuje odaberite **u redu**. 
  
3. U web-pregledniku, pronađite na web-mjestu korijena zbirke web-mjesta i pristup **Postavkama web-mjesta** \> **Značajke zbirke web-mjesta**. Preklopi značajka **tijekova rada** : 
  
· Značajka je *aktivirano* , kliknite **Deaktiviraj,** a zatim kliknite **Aktiviraj**. 
  
· Značajka je *Deactivated* , kliknite **Aktiviraj**. 
  
Za dodatne informacije pogledajte sljedeći [članak](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

