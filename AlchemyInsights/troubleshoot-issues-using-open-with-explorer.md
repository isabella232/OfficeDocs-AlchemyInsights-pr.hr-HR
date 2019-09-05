---
title: Rješavanje problema Otvori pomoću programa Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742725"
---
# <a name="fix-problems-with-open-with-explorer"></a>Riješite probleme s Otvori pomoću programa Explorer

Riješite uobičajene probleme s otvaranjem biblioteku dokumenata u SharePoint ili OneDrive koristeći naredbu **Otvori pomoću programa Explorer** : 
  
- Koristite Internet Explorer 10 ili Internet Explorer 11. **Otvori pomoću programa Explorer** nije kompatibilna s Microsoft Edge, vizualnog Google, Firefox i drugima. **Otvori pomoću programa Explorer** onemogućeno je u svim preglednicima osim preglednika Internet Explorer. 
    
- **Otvori pomoću programa Explorer** nije dostupna u modernom iskustvo za SharePoint biblioteke. Umjesto toga koristite **Prikaz Explorer datoteka** . Odaberite **Mogućnosti prikaza** \> **Prikaz Explorer datoteka**. Prikaz u programu Explorer datoteka nije kompatibilna s Microsoft Edge, vizualnog Google, Firefox i drugima. **Prikaz u programu Explorer datoteku** u dostupna samo u programu Internet Explorer. 
    
- Provjerite je li pokrenut servis WebClient. U okvir za pretraživanje Windows, vrsta pokretanja, odaberite Pokreni radne površine app, upišite services.msc i pritisnite tipku Enter. Pomaknite WebClient servisa i provjerite je li stupac **Stanje** prikazuje "Pokrenuto". Ako ne, dvaput kliknite servis, kliknite **Start**, a zatim kliknite **u redu**. (Možda ćete morati omogućiti servis odabirom **ručno** ili **Automatsko** u okviru **Vrsta pokretanja** .) 
    
> [!NOTE]
> Otvaranje biblioteke Explorer datoteka je praktičan ako trebate kopirati ili premjestiti više datoteka i mapa jednom, ali ako želite redovito raditi u biblioteci, preporučujemo da ga sinkroniziranje. Za rješavanje problema s otvaranjem datoteka Explorer vidjeti [otvorene u programu Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Info o postavljanju sinkronizacije potražite [SharePoint sinkronizaciju datoteke s novom klijentu sinkronizaciju OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).
  
Pogledajte članak [kako koristiti naredbu "Otvori s Explorer" otklanjanje poteškoća u SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) dodatne informacije. 
  

