---
title: Stvaranje web-mjesta u sustavu SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: hr-HR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732207"
---
# <a name="create-sharepoint-sites-using-templates"></a>Stvaranje web-mjesta sustava SharePoint pomoću predložaka

Mogućnost spremanja web-mjesta u obliku predloška nije podržana uz moderna komunikacija ili timska web-mjesta. Dodatne informacije o korištenju predložaka potražite u članku [Spremanje, preuzimanje i prijenos web-mjesta sustava SharePoint kao predloška](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Slijede neki Česti problemi/rješenja vezana uz spremanje web-mjesta ili popisa kao predloška u sustavu SharePoint online. 

**Gumb Spremi predložak web-mjesta/popisa nije dostupan ili nedostaje**

Administratorima će biti potrebno omogućiti prilagođenu skriptu za omogućivanje značajki predložaka. Detaljne upute, primjeri i razmatranja potražite u članku 

- [Omogućivanje i onemogućivanje prilagođene skripte](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Naredba Spremi web-mjesto kao predložak nije podržana i može uzrokovati probleme na web-mjestima koja koriste infrastrukturu za objavljivanje sustava SharePoint Server.

**Predložak web-mjesta nije moguće stvoriti ili ne funkcionira pravilno**

Predložak možda nema [značajku](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i neće se aktivirati. Ako značajka nije dostupna za aktivaciju u aktualnoj zbirci web-mjesta, ne možete stvoriti web-mjesto pomoću predloška web-mjesta.

- Provjerite prelazi li neki popisi ili biblioteke iznad [praga ograničenja prikaza popisa](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) od 5000 stavki jer to može blokirati stvaranje predloška web-mjesta.

- Web-mjesto možda koristi previše resursa, a predložak web-mjesta premašuje ograničenje od 50 MB.


- Postoje problemi s prikazom podataka s popisa koji koristi stupac za pretraživanje. Dodatne informacije potražite u članku [popis generirani predložak ne prikazuje podatke s odgovarajućeg popisa pretraživanja u sustavu SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Detaljne informacije o uobičajenim problemima i rješenjima potražite u odjeljku [Stvaranje i korištenje predložaka web-mjesta](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



