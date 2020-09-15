---
title: Poruka o održavanju samo za čitanje prilikom pokušaja korištenja sustava SharePoint ili servisa OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670824"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Poruka o održavanju samo za čitanje prilikom pokušaja korištenja sustava SharePoint ili servisa OneDrive

Prilikom pokušaja korištenja sustava SharePoint ili servisa OneDrive za jedan od sljedećih scenarija korisnici mogu primiti poruku **samo za čitanje** . 

-   Planirana ili aktivna aktivnost održavanja.  Potražite ih tako da otvorite centar za [poruke](https://portal.office.com/adminportal/home#/messagecenter).
-   Problem s velikim prioritetom, aktivnim incidentom servisa koji se možda pojavljuje. Provjerite postoje li Savjeti/incidenti tako da odete na [zdravlje servisa](https://portal.office.com/adminportal/home#/servicehealth).
-   Manji scenario za automatsko ozdravljenje koji bi se mogao događati zbog neočekivanih događaja na poslužiteljima koji bi mogli trajati manje od 30 min ili više. 
    
    Nema centra za poruke ili zdravstvenih pošta za ove male oporavnice, no uskoro ćete se vratiti u normalu.

U vrlo malo navrata primijetili smo da je jedan od navedenih triju scenarija uzrok, a servis je vraćen, ali predmemorija korisnika preglednika nije očišćena.

Pokušajte izbrisati predmemoriranje preglednika prije nego što odete na web-mjesto.

1. U pregledniku Microsoft Edge odaberite **Postavke**, a zatim odaberite **privatnost i sigurnost**.
2. U odjeljku **čisto pregledavanje**odaberite **Odaberi što želite očistiti**.
3. Odaberite **Kolačići i spremite podatke o web-mjestu**, a zatim odaberite **Očisti**.

>[!Note] 
> Ovi se koraci mogu razlikovati prilikom korištenja drugih preglednika, kao što su Mozilla Firefox ili Google Chrome.

>[!Note] 
> Druga bi mogućnost bila otvaranje web-mjesta sustava SharePoint ili servisa OneDrive u novom prozoru weba InPrivate.