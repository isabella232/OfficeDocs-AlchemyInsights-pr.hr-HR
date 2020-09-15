---
title: Otklanjanje poteškoća s otvaranjem programa Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659050"
---
# <a name="fix-problems-with-open-with-explorer"></a>Rješavanje problema s otvaranjem programa Explorer

Riješite česte probleme s otvaranjem biblioteke dokumenata u sustavu SharePoint ili servisa OneDrive pomoću naredbe **Otvori pomoću programa Explorer** : 
  
- Koristite Internet Explorer 10 ili Internet Explorer 11. **OpenBSD sa istraživač** nije kompatibilan sa Microsoft Edge, Google Chrome, Firefox i drugi. **Otvaranje programom Explorer** onemogućeno je u svim preglednicima osim u pregledniku Internet Explorer. 
    
- **Otvaranje programom Explorer** nije dostupno u modernom iskustvu za biblioteke sustava SharePoint. Umjesto toga koristite **Prikaz u eksploreru za datoteke** . Odaberite prikaz **mogućnosti prikaza** \> **u eksploreru za datoteke**. Prikaz u eksploreru za datoteke nije kompatibilan s programom Microsoft Edge, Google Chrome, Firefox i drugi. **Prikaz u eksploreru za datoteke** dostupan samo u pregledniku Internet Explorer. 
    
- Provjerite je li servis WebClient pokrenut. U okvir za pretraživanje sustava Windows upišite Pokreni pa odaberite Pokreni aplikaciju za stolna računala, upišite Services. msc, a zatim pritisnite ENTER. Pomaknite se prema dolje do web-klijentskog servisa i provjerite prikazuje li stupac **status** "pokrenut". Ako to ne učinite, dvokliknite servis, zatim kliknite **Start**, a potom **u redu**. (Možda ćete morati najprije omogućiti servis tako da odaberete **ručno** ili **Automatsko** u okviru **Vrsta pokretanja** .) 
    
> [!NOTE]
> Otvaranje biblioteke u eksploreru za datoteke korisno je ako jednom morate kopirati ili premještati više datoteka i mapa, no ako želite redovito raditi u biblioteci, preporučujemo da je sinkronizirate. Upute za otklanjanje poteškoća u eksploreru za datoteke potražite [u članku otvaranje u programu Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Informacije o postavljanju sinkronizacije potražite [u članku sinkronizacija datoteka sustava SharePoint s novim klijentom za sinkronizaciju servisa OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).
  
[Upute za otklanjanje poteškoća u sustavu SharePoint Online potražite u članku kako koristiti naredbu "Otvori sa eksplorerom" da biste](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) saznali više o problemima. 
  

