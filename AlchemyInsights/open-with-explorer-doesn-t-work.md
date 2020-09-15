---
title: Otvori pomoću programa Explorer ne funkcionira
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694448"
---
# <a name="open-with-explorer-isnt-working"></a>Otvaranje pomoću programa Explorer ne funkcionira

Ako je u eksploreru **za datoteke** **otvoreno pomoću programa Explorer** ili prikaz, provjerite je li web-klijent poslužitelj postavljen na **pokretanje** slijedeći korake u nastavku. Možda će, primjerice, trebati dugo vremena za otvaranje biblioteke sustava SharePoint ili servisa OneDrive kada servis nije pokrenut. 
  
1. U okvir za pretraživanje sustava Windows upišite Pokreni, odaberite Pokreni aplikaciju za stolna računala, upišite Services. msc, a zatim odaberite **Enter**.
    
2. Pomaknite se prema dolje do web-klijentskog servisa i provjerite stupac **status** . Ako status servisa WebClient nije **pokrenut**, dvokliknite servis, zatim kliknite **Start**, a potom **u redu**. Ako je potrebno, omogućite servis tako da odaberete **ručno** ili **Automatsko** u okviru **Vrsta pokretanja** . 
    
> [!NOTE]
> Upute za otklanjanje poteškoća u eksploreru za datoteke potražite [u članku otvaranje u programu Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Istražite sinkronizaciju kao bolju alternativu: [Sinkronizacija datoteka sustava SharePoint s novim klijentom za sinkronizaciju servisa OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

