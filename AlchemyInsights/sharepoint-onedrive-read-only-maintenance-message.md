---
title: Read-Only za održavanje prilikom pokušaja korištenja SharePoint ili OneDrive
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
ms.openlocfilehash: edcdea2f5c0647b92c230dd1d86549173e72997fc885195cde688b3b17710a2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910538"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only za održavanje prilikom pokušaja korištenja SharePoint ili OneDrive

Korisnici mogu primiti poruku **samo za čitanje za održavanje** prilikom pokušaja korištenja SharePoint ili OneDrive za jedan od sljedećih scenarija. 

-   Planirana ili aktivna aktivnost održavanja.  Provjerite ima li ih navigiranjem do [centra za poruke](https://portal.office.com/adminportal/home#/messagecenter).
-   Incident s aktivnim servisom visokog prioriteta koji se može pojaviti. Provjerite ima li kakvih savjetnika/incidenata navigiranjem do stanja [servisa](https://portal.office.com/adminportal/home#/servicehealth).
-   Scenarij manjeg oporavka automatskog iscjeljivanja koji se može dogoditi zbog neočekivanih događaja na poslužiteljima koji bi mogli trajati manje od 30 minuta. 
    
    Nema objava centra za poruke ni stanja servisa za ta manja oporavka, ali uskoro ćete se vratiti u normalu.

U nekoliko smo navrata primijetili da je uzrok jedan od tri navedena scenarija i da je servis vraćen, ali predmemorija preglednika korisnika nije izbrisana.

Prije navigacije do web-mjesta pokušajte očistiti predmemoriju preglednika.

1. U pregledniku Microsoft Edge odaberite **Postavke**, a zatim Privatnost **i sigurnost**.
2. U **odjeljku Čišćenje pregledavanja** **odaberite Odaberite što želite očistiti**.
3. Odaberite **Kolačići i spremljeni podaci web-mjesta** i odaberite **Očisti**.

>[!Note] 
> Ti se koraci mogu razlikovati kada koristite druge preglednike kao što su Mozilla Firefox ili Google Chrome.

>[!Note] 
> Druga mogućnost bila bi otvaranje web-SharePoint web-mjesta ili OneDrive u novom prozoru web-mjesta InPrivate.