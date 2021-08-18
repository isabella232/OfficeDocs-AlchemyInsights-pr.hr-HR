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
ms.openlocfilehash: 376b653b18857103586e25edd0ad6801a7bbe0a1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329440"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only za održavanje prilikom pokušaja korištenja SharePoint ili OneDrive

Korisnici mogu primiti poruku **samo za čitanje za održavanje** prilikom pokušaja korištenja SharePoint ili OneDrive za jedan od sljedećih scenarija. 

-   Planirana ili aktivna aktivnost održavanja.  Provjerite ima li ih navigiranjem do [centra za poruke](https://portal.office.com/adminportal/home#/messagecenter).
-   Incident s aktivnim servisom visokog prioriteta koji se može pojaviti. Provjerite ima li kakvih savjetnika/incidenata navigiranjem do stanja [servisa](https://portal.office.com/adminportal/home#/servicehealth).
-   Scenarij manjeg oporavka automatskog iscjeljivanja koji se može dogoditi zbog neočekivanih događaja na poslužiteljima koji bi mogli trajati manje od 30 minuta. 
    
    Nema objava centra za poruke ni stanja servisa za ta manja oporavka, ali uskoro ćete se vratiti u normalu.

U vrlo smo nekoliko navrata primijetili da je uzrok jedan od tri navedena scenarija i da je servis vraćen, ali predmemorija preglednika korisnika nije izbrisana.

Prije navigacije do web-mjesta pokušajte očistiti predmemoriju preglednika.

1. U pregledniku Microsoft Edge odaberite **Postavke**, a zatim Privatnost **i sigurnost**.
2. U **odjeljku Čišćenje pregledavanja** **odaberite Odaberite što želite očistiti**.
3. Odaberite **Kolačići i spremljeni podaci web-mjesta** i odaberite **Očisti**.

**Napomena:** ti se koraci mogu razlikovati prilikom korištenja drugih preglednika kao što su Mozilla Firefox ili Google Chrome.

**Napomena:** druga mogućnost bila bi otvaranje web-SharePoint web-mjesta ili OneDrive u novom prozoru web-mjesta InPrivate.