---
title: Otklanjanje poteškoća s korištenjem programa Open with Explorer
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
ms.openlocfilehash: 0cbcfb506295d5732f7109be7a103bbdef530a529c7408c6d9d45a7b38a89915
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048148"
---
# <a name="fix-problems-with-open-with-explorer"></a>Rješavanje problema s programom Open with Explorer

Rješavanje uobičajenih problema s otvaranjem biblioteke dokumenata u SharePoint ili OneDrive pomoću naredbe **Otvori pomoću eksplorera:** 
  
- Koristite Internet Explorer 10 ili Internet Explorer 11. **Otvaranje pomoću preglednika Explorer** nije kompatibilno s Microsoft Edge, preglednikom Google Chrome, Firefox i drugima. **Otvaranje pomoću preglednika Explorer** onemogućeno je u svim preglednicima osim u pregledniku Internet Explorer. 
    
- **Otvaranje pomoću preglednika Explorer** nije dostupno u modernom SharePoint bibliotekama. Umjesto toga **koristite Prikaz u eksploreru** za datoteke. Odaberite **Prikaz mogućnosti Prikaz** u \> **eksploreru za datoteke**. Prikaz u eksploreru za datoteke nije kompatibilan s Microsoft Edge, preglednikom Google Chrome, Firefox i drugima. **Prikaz u eksploreru za datoteke** dostupan je samo u pregledniku Internet Explorer. 
    
- Provjerite je li pokrenut servis WebClient. U okvir Windows pretraživanje upišite pokreni, odaberite aplikaciju Pokreni radnu površinu, upišite services.msc, a zatim pritisnite Enter. Pomaknite se prema dolje do servisa WebClient i provjerite **prikazuje li stupac Stanje** "Pokrenuto". Ako ne, dvokliknite servis, zatim Start **,** a zatim U **redu**. (Možda ćete morati najprije omogućiti servis  tako da u okviru Vrsta **pokretanja** odaberete Ručno ili **Automatski.)** 
    
> [!NOTE]
> Otvaranje biblioteke u eksploreru za datoteke praktično je ako morate kopirati ili premjestiti više datoteka i mapa jednom, ali ako želite redovito raditi u biblioteci, preporučujemo da je sinkronizirate. Da biste otklonili poteškoće prilikom otvaranja u eksploreru za datoteke, [pogledajte otvaranje u eksploreru](https://go.microsoft.com/fwlink/?linkid=871665). Informacije o postavljanju sinkronizacije potražite u članku [Sinkronizacija SharePoint datoteka s novim Sinkronizacija sa servisom OneDrive klijenta](https://go.microsoft.com/fwlink/?linkid=871666).
  
Dodatne informacije potražite u [članku Kako koristiti naredbu "Otvori pomoću eksplorera"](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) za otklanjanje poteškoća SharePoint online. 
  

