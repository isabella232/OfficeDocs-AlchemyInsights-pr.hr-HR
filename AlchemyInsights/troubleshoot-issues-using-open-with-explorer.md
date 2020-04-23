---
title: Otklanjanje poteškoća s pomoću značajke Otvori pomoću programa Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: cb26876d93a110b3b0addd7821206215c783f959
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759684"
---
# <a name="fix-problems-with-open-with-explorer"></a>Rješavanje problema s otvori pomoću programa Explorer

Riješite uobičajene probleme s otvaranjem biblioteke dokumenata u sustavu SharePoint ili OneDrive pomoću naredbe **Otvori pomoću programa Explorer:** 
  
- Koristite Internet Explorer 10 ili Internet Explorer 11. **Otvoreno s preglednikom Explorer** nije kompatibilno s preglednikom Microsoft Edge, Google Chrome, Firefox i drugima. **Otvori s explorerom** onemogućen je u svim preglednicima osim preglednika Internet Explorer. 
    
- **Otvoreno pomoću programa Explorer** nije dostupno u modernom doživljaju za biblioteke sustava SharePoint. Umjesto toga koristite **Prikaz u eksploreru za datoteke.** Odaberite **Prikaz mogućnosti** \> **Prikaz u eksploreru za datoteke**. View in File Explorer nije kompatibilan s microsoft edge, Google Chrome, Firefox i drugima. **Prikaz u eksploreru za datoteke** dostupan je samo u pregledniku Internet Explorer. 
    
- Provjerite je li pokrenut servis WebClient. U okvir za pretraživanje u sustavu Windows upišite pokreni, odaberite aplikaciju Pokreni radnu površinu, upišite services.msc, a zatim pritisnite tipku Enter. Pomaknite se prema dolje do servisa WebClient i provjerite prikazuje li se u stupcu **Status** "Running". Ako se to ne događa, dvokliknite servis, kliknite **Start**, a zatim **U redu**. (Možda ćete prvo morati omogućiti uslugu tako da u okviru **Vrsta pokretanja** odaberete **Ručno** ili **Automatsko.)** 
    
> [!NOTE]
> Otvaranje biblioteke u eksploreru za datoteke praktično je ako morate jednom kopirati ili premjestiti više datoteka i mapa, ali ako želite redovito raditi u biblioteci, preporučujemo da je sinkronizirate. Da biste otklonili poteškoće s otvaranjem u eksploreru za datoteke, [pročitajte članak Otvori u programu Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Informacije o postavljanju sinkronizacije potražite u [odjeljku Sinkronizacija datoteka sustava SharePoint s novim klijentom za sinkronizaciju sa servisom OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).
  
Dodatne informacije potražite u članku [Korištenje naredbe "Otvori pomoću programa Explorer" za otklanjanje poteškoća u sustavu SharePoint Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) 
  

