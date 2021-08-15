---
title: Otvaranje pomoću programa Explorer ne funkcionira
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
ms.openlocfilehash: 164d5fe8c992df825d1f52f19792e1623526c35c58ff2f1e1ab601fdcf5f0f53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011328"
---
# <a name="open-with-explorer-isnt-working"></a>Otvaranje pomoću preglednika Explorer ne funkcionira

Ako **Otvori pomoću preglednika Explorer** ili Prikaz u **eksploreru** za datoteke ne funkcionira, provjerite je li servis WebClient postavljen **na Pokrenut** slijedeći korake u nastavku. Možda će, primjerice, dugo trajati otvaranje SharePoint ili OneDrive kada servis nije pokrenut. 
  
1. U okvir Windows pretraživanje upišite pokreni, odaberite aplikaciju Pokreni radnu površinu, upišite services.msc, a zatim odaberite **Enter**.
    
2. Pomaknite se prema dolje do servisa WebClient i provjerite **stupac** Stanje. Ako status servisa WebClient nije **pokrenut**, dvokliknite servis, zatim **Start**, a zatim U **redu**. Po potrebi omogućite servis tako  da  u okviru Vrsta pokretanja odaberete Ručno ili **Automatski.** 
    
> [!NOTE]
> Da biste otklonili poteškoće prilikom otvaranja u eksploreru za datoteke, [pogledajte otvaranje u eksploreru](https://go.microsoft.com/fwlink/?linkid=871665). Istražite sinkronizaciju kao bolju alternativu: [sinkronizacija SharePoint datoteka s novim Sinkronizacija sa servisom OneDrive klijentom](https://go.microsoft.com/fwlink/?linkid=871666). 
  

