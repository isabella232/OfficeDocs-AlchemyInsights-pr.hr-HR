---
title: Otvori pomoću programa Explorer ne funkcionira
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713026"
---
# <a name="open-with-explorer-isnt-working"></a>Otvaranje pomoću programa Explorer ne funkcionira

Ako **otvori pomoću programa Explorer** ili Prikaz u **eksploreru za datoteke** ne funkcionira, provjerite je li servis WebClient postavljen na **Pokrenut** slijedeći korake u nastavku. Na primjer, otvaranje biblioteke sustava SharePoint ili OneDrive može potrajati dok servis nije pokrenut. 
  
1. U okvir za pretraživanje u sustavu Windows upišite pokreni, odaberite aplikaciju Pokreni radnu površinu, upišite services.msc, a zatim odaberite **Enter**.
    
2. Pomaknite se prema dolje do servisa WebClient i provjerite stupac **Status.** Ako status web-klijentskog servisa nije **pokrenut,** dvokliknite servis, zatim **Start**, a potom **U redu**. Omogućite uslugu, ako je potrebno, odabirom **ručnog** ili **automatskog** u okviru **Vrsta pokretanja.** 
    
> [!NOTE]
> Da biste otklonili poteškoće s otvaranjem u eksploreru za datoteke, [pročitajte članak Otvori u programu Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Istražite sinkronizaciju kao bolju alternativu: [sinkronizirajte datoteke sustava SharePoint s novim klijentom za sinkronizaciju sa servisom OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

