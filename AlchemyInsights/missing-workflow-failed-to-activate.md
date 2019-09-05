---
title: Nedostaje tijek rada nije uspio aktivirati
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753788"
---
# <a name="missing-workflow-failed-to-activate"></a>Nedostaje tijek rada nije uspio aktivirati

U zbirke web-mjesta Microsoft SharePoint globalno ponovno iskoristiv tijek rada (na primjer "odobrenje - SharePoint 2010") ne može dodati na popis ili biblioteku.
  
Da biste riješili taj problem, slijedite ove korake: 
  
1. Otvorite web-mjesto korijena zbirke web-mjesta SharePoint Designer 2013.
  
2. Pod **Objekti web-mjesta**odaberite **tijekova rada**. 
  
3. U sekciji **Novo** vrpce **tijekove rada** , odaberite **Tijek rada za ponovno iskoristiv**. 
  
4. **Stvaranje tijeka rada ponovno iskoristiv** obrascu unesite naziv ** *Repair2010* **. Za **Vrstu Platform**kliknite **Tijeka rada sustava SharePoint 2010**, a zatim kliknite **u redu**. 
  
1. U odjeljak **spremiti** vrpce **tijeka rada** odaberite **Objavi**. 
  
2. U odjeljku **Upravljanje** vrpce **tijeka rada** , odaberite **Objaviti globalno**. U dijaloškom okviru potvrda koja se pojavljuje odaberite **u redu**. 
  
3. U web-pregledniku, pronađite na web-mjestu korijena zbirke web-mjesta i pristup **Postavkama web-mjesta** \> **Značajke zbirke web-mjesta**. Zatim, Preklopi značajka **tijekova rada** : 
  
· Značajka je *aktivirano* , kliknite **Deaktiviraj,** a zatim kliknite **Aktiviraj**. 
  
· Značajka je *Deactivated* , kliknite **Aktiviraj**. 
  
Za dodatne informacije pogledajte sljedeći [članak](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

