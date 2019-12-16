---
title: Samo za čitanje za poruku održavanja prilikom pokušaja korištenja sustava SharePoint ili servisa OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051273"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Samo za čitanje za poruku održavanja prilikom pokušaja korištenja sustava SharePoint ili servisa OneDrive

Korisnici mogu primiti poruku **samo za čitanje za održavanje** kada pokušate koristiti SharePoint ili OneDrive za jedan od sljedećih scenarija. 

-   Planirana ili aktivna aktivnost održavanja.  Provjerite ih navigacijom do centra za [poruke](https://portal.office.com/adminportal/home#/messagecenter).
-   Incident s visokim prioritetom, aktivni servis koji se možda javlja. Provjerite ima li bilo kakvih savjetovanja/incidenata navigiranjem do [servisa Health](https://portal.office.com/adminportal/home#/servicehealth).
-   Manji scenarij oporavka iz automatskog ozdravljenja koji bi se mogao događati zbog neočekivanih događaja na poslužiteljima koji bi mogli trajati manje od 30 min. 
    
    Nema centra za poruke ni radnih mjesta za ova manja oporavka, ali biste se uskoro trebali vratiti u normalu.

U vrlo nekoliko navrata smo primijetili da je jedan od tri navedena scenarija bio uzrok, a servis je vraćen, ali korisnici cache preglednik nije očišćen.

Pokušajte izbrisati predmemoriju preglednika prije navigacije do web-mjesta.

1. U pregledniku Microsoft Edge odaberite **Postavke**, a zatim odaberite **privatnost i sigurnost**.
2. Pod **jasnim pregledavanjem**odaberite **Odaberite što želite očistiti**.
3. Odaberite **Kolačići i spremljeni podaci web-mjesta**i odaberite **Očisti**.

>[!Note] 
> Ovi koraci mogu se razlikovati prilikom korištenja drugih preglednika kao što su Mozilla Firefox ili Google Chrome.

>[!Note] 
> Druga bi mogućnost bila otvaranje SharePoint web-mjesta ili servisa OneDrive u novom prozoru InPrivate.